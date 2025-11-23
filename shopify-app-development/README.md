# Shopify App Development - Claude Code Plugin

A comprehensive Claude Code plugin marketplace for building full-stack Shopify apps with specialized agents for database, API, and UI development.

## 🎯 Overview

This plugin provides specialized agents and skills for Shopify app development using modern tools:

- **Polaris Web Components** - Shopify's official UI framework
- **Shopify Admin GraphQL API** - Product, metafield, and store data management
- **Prisma ORM** - Type-safe database operations
- **React 19** - Modern UI with SSR support
- **Remix Framework** - Full-stack React framework

## 📦 Included Plugins

### 1. **shopify-app-orchestrator**
Multi-agent task coordinator for complex full-stack features.

**Use for:**
- Building complete features spanning DB + API + UI
- Major refactoring across multiple layers
- Complex integrations requiring multiple agents

**Example:**
```
Use shopify-app-orchestrator to implement a bulk product import feature
```

### 2. **shopify-polaris-ui**
Polaris Web Components expert for building Shopify app UIs.

**Use for:**
- Creating new UI pages and components
- Fixing Polaris component issues
- Implementing Shopify app design patterns

**Example:**
```
Use shopify-polaris-ui to create a product index page with filters
```

### 3. **shopify-database-specialist**
Database and Prisma expert for schema design and migrations.

**Use for:**
- Modifying database schema
- Creating migrations
- Optimizing queries and data modeling

**Example:**
```
Use shopify-database-specialist to add a ProductTag model
```

### 4. **shopify-api-integration**
Shopify Admin GraphQL API expert for integrations.

**Use for:**
- Creating GraphQL queries and mutations
- Handling webhooks and rate limiting
- Managing metafields and bulk operations

**Example:**
```
Use shopify-api-integration to create a product sync query
```

### 5. **shopify-design-system**
Design system compliance expert for visual consistency.

**Use for:**
- Reviewing UI code for design system compliance
- Ensuring consistent use of Polaris tokens
- Auditing screens for visual consistency

**Example:**
```
Use shopify-design-system to review the dashboard for consistency
```

### 6. **shopify-pattern-enforcer**
Pattern consistency checker for codebase-wide quality.

**Use for:**
- Ensuring fixes are applied consistently
- Identifying similar code patterns
- Pattern-based refactoring

**Example:**
```
Use shopify-pattern-enforcer after fixing the event handler issue
```

## 🛠️ Installation

1. Clone or download this repository
2. Place in your project's `claude-plugins/` directory
3. Invoke agents by name in your Claude Code session

## 📚 Documentation

Each plugin includes:
- Detailed agent instructions
- Code examples and patterns
- Best practices and guidelines
- Skills for auto-invoked knowledge

## 🚀 Quick Start

### For Full-Stack Features
```
Use shopify-app-orchestrator to build [feature name]
```

### For UI Work
```
Use shopify-polaris-ui to create [page/component name]
```

### For Database Changes
```
Use shopify-database-specialist to [database task]
```

### For API Integration
```
Use shopify-api-integration to [API task]
```

## 📖 Learning Resources

- [Shopify App Development](https://shopify.dev/docs/apps)
- [Polaris Web Components](https://polaris.shopify.com/components)
- [Shopify Admin API](https://shopify.dev/docs/api/admin-graphql)
- [Prisma Documentation](https://www.prisma.io/docs)

## 🤝 Contributing

Contributions welcome! Please ensure agents follow the established patterns and include proper documentation.

## 📄 License

MIT License - See LICENSE file for details

---

**Built for Claude Code** | [Report Issues](https://github.com/yourname/shopify-app-development/issues)
