# Database Operations Safety Pattern

## Core Principle
**When in doubt about destructive database operations, ALWAYS ask for clarification before proceeding.**

Deleting specific data is reversible through re-running scripts or re-importing. Deleting configuration, schemas, or entire databases is catastrophic.

## The Rule of Specificity

### ALWAYS Assume Minimal Scope
When a user says "clear the db" or similar ambiguous phrases:
- **Default interpretation**: Clear only the data they're currently working with
- **NOT**: Wipe the entire database, delete all tables, or destroy configuration

### Context Clues for Scope

#### Phrases that indicate LIMITED scope:
- "for testing" → preserve configuration, clear only test data
- "to test the [feature]" → clear only data related to that feature
- "start fresh with [X]" → clear only X-related data
- "reset the [specific thing]" → clear only that specific thing
- After implementing a new feature → likely want to test with fresh data for THAT feature only

#### Phrases that indicate FULL scope:
- "completely reset everything"
- "start from scratch with the entire database"
- "delete the database file"
- "I want to rebuild the whole schema"
- "nuke it all"

## Decision Tree for Database Operations

```
User requests database "clearing" or "resetting"
│
├─ Is the request specific? (e.g., "clear the products table")
│  └─ YES → Proceed with DELETE FROM [specific_table]
│
├─ Is the request ambiguous? (e.g., "clear the db", "reset it")
│  └─ YES → STOP and ask:
│            "To clarify, do you want me to:
│             1. Delete data from specific tables (which ones?)
│             2. Reset the entire database including all configuration
│             3. Drop and recreate specific tables
│             Please specify which tables or data should be cleared."
│
└─ Is the request explicitly destructive? (e.g., "delete dev.db")
   └─ YES → STILL confirm what they're trying to achieve:
            "This will delete [X, Y, Z]. Is that what you need, or
             would clearing specific tables be sufficient?"
```

## Safe Deletion Patterns

### 1. Specific Table Data (SAFE)
```typescript
// Clear specific table data only
await db.product.deleteMany({
  where: { shopId: shop.id },
});
console.log("Cleared products for current shop");
```

### 2. Test Data Only (SAFE)
```typescript
// Clear test/development data
await db.product.deleteMany({
  where: {
    shopId: shop.id,
    OR: [
      { title: { contains: "TEST" } },
      { createdAt: { gte: new Date("2024-01-01") } },
    ],
  },
});
```

### 3. Multiple Related Tables (ASK FIRST)
```typescript
// ⚠️ CONFIRM before running
await db.$transaction([
  db.product.deleteMany({ where: { shopId: shop.id } }),
  db.order.deleteMany({ where: { shopId: shop.id } }),
]);
```

### 4. Schema Reset (DANGEROUS - ALWAYS CONFIRM)
```bash
# ⚠️⚠️⚠️ NEVER run without explicit confirmation
npx prisma migrate reset
```

## Examples of Safe Interpretations

### Example 1: "Clear the database for testing"

**User says**: "clear the database for testing"

**WRONG interpretation**:
```bash
rm prisma/dev.db  # ❌ Deletes entire database
npx prisma migrate reset  # ❌ Resets everything
```

**CORRECT interpretation**:
```typescript
// Clear only the data being tested
await db.product.deleteMany({
  where: { shopId: shop.id },
});
```

**OR ask**: "Which tables should I clear? Products, orders, or all shop data?"

### Example 2: "Reset the products"

**User says**: "reset the products"

**CORRECT interpretation**:
```typescript
// Clear only products table
await db.product.deleteMany({
  where: { shopId: shop.id },
});
console.log("Products cleared for current shop");
```

### Example 3: "Start fresh with the sync"

**User says**: "start fresh with the sync"

**CORRECT interpretation**:
```typescript
// Clear only sync-related data
await db.backgroundJob.deleteMany({
  where: {
    shopId: shop.id,
    jobType: "sync",
  },
});
console.log("Cleared sync jobs for current shop");
```

## Confirmation Templates

### For Ambiguous Requests
```
"To clarify, do you want me to:
1. Delete [specific data type] (e.g., products, orders)
2. Clear all data for the current shop
3. Reset the entire database including schema

Please specify which option."
```

### For Potentially Destructive Operations
```
"This operation will:
- Delete [X records] from [Y tables]
- Remove [configuration/settings]
- [Other impacts]

Is this what you intended? If you just need to test [feature],
I can clear only the [specific table] instead."
```

## Safe Operations Checklist

Before executing any delete operation:
- [ ] Understand the scope (specific table, shop data, or entire database)
- [ ] Confirm the target (which tables, which records)
- [ ] Check for dependencies (cascade deletes)
- [ ] Verify backup exists (for production)
- [ ] Use transactions (for multi-table operations)
- [ ] Log the operation (for audit trail)
- [ ] Confirm with user (if ambiguous)

## Best Practices

1. **Default to Minimal Scope** - When in doubt, delete less, not more
2. **Ask Questions** - Better to clarify than to destroy important data
3. **Use Transactions** - For multi-table deletes, use transactions
4. **Add Where Clauses** - Always filter by shopId for shop-specific data
5. **Log Operations** - Log what was deleted for debugging
6. **Test in Development** - Never test destructive operations in production
7. **Confirm Explicitly** - For destructive operations, get explicit confirmation

---

**Remember**: It's better to ask for clarification than to accidentally delete production data. When in doubt, ask!
