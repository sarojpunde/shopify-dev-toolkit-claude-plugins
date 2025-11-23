# Shopify Development Toolkit - Claude Code Agent

This is a comprehensive Claude Code agent system for Shopify development with 16 specialized agents organized into three categories.

## 🎯 Agent System Overview

You have access to **16 specialized agents** across three development domains:

### 🎨 Theme Development Agents (5)
- **shopify-liquid-specialist** - Liquid templating expert
- **shopify-section-builder** - Shopify 2.0 sections with schemas
- **shopify-global-settings** - Theme settings management
- **shopify-snippet-library** - Reusable Liquid snippets
- **shopify-translation-manager** - Multi-language support

### 🚀 App Development Agents (6)
- **shopify-app-orchestrator** - Multi-agent coordinator for full-stack features
- **shopify-polaris-ui** - Polaris Web Components for app UIs
- **shopify-database-specialist** - Prisma schema and migrations
- **shopify-api-integration** - Shopify Admin GraphQL API
- **shopify-design-system** - Design consistency and Polaris tokens
- **shopify-pattern-enforcer** - Codebase pattern consistency

### 🎭 Polaris UI Agents (5)
- **polaris-component-expert** - Full component library access
- **polaris-forms-specialist** - Form components and validation
- **polaris-layout-specialist** - Page layouts and structure
- **polaris-patterns-expert** - Composition patterns and templates
- **polaris-app-bridge-specialist** - Native Shopify app integration

## 🚦 Agent Selection Guidelines

### When Building Shopify Themes

**For Liquid Templating:**
```
Use shopify-liquid-specialist for Liquid syntax and template structure
```

**For Sections:**
```
Use shopify-section-builder to create sections with schemas
```

**For Theme Settings:**
```
Use shopify-global-settings to manage settings_schema.json
```

**For Reusable Components:**
```
Use shopify-snippet-library to create snippets
```

**For Multi-Language:**
```
Use shopify-translation-manager for translation files
```

### When Building Shopify Apps

**For Full-Stack Features:**
```
Use shopify-app-orchestrator to coordinate DB + API + UI implementation
```

**For Database:**
```
Use shopify-database-specialist for Prisma schema and migrations
```

**For Shopify API:**
```
Use shopify-api-integration for GraphQL queries and mutations
```

**For UI:**
```
Use shopify-polaris-ui to build Polaris-based interfaces
```

**For Design Consistency:**
```
Use shopify-design-system to ensure Polaris token compliance
```

**For Code Quality:**
```
Use shopify-pattern-enforcer to maintain consistent patterns
```

### When Working with Polaris

**For General Components:**
```
Use polaris-component-expert for component selection and usage
```

**For Forms:**
```
Use polaris-forms-specialist to build forms with validation
```

**For Layouts:**
```
Use polaris-layout-specialist for page structure and grids
```

**For Page Patterns:**
```
Use polaris-patterns-expert for index, settings, dashboard layouts
```

**For App Integration:**
```
Use polaris-app-bridge-specialist for native Shopify features
```

## 🎓 Skills (Auto-Invoked)

The following skills activate automatically based on task context:

**Theme Development:**
- shopify-liquid-fundamentals
- shopify-section-patterns
- shopify-schema-design
- shopify-snippet-library
- shopify-i18n-basics
- shopify-workflow-tools

**App Development:**
- shopify-api-patterns
- polaris-ui-patterns
- database-best-practices

**Polaris UI:**
- polaris-fundamentals
- polaris-compositions

## 📚 Documentation Access

Agents have access to:
- `shopify-theme-development/` - Theme agent implementations and skills
- `shopify-app-development/` - App agent implementations, skills, and patterns
- `shopify-polaris/` - Polaris agent implementations and skills
- `polaris-web-components/` - Full Polaris component library (if available in parent directory)

## 🔄 Multi-Agent Workflows

### Example: Building a Product Feature

**Theme Development:**
1. `shopify-section-builder` - Create product grid section
2. `shopify-snippet-library` - Create product card snippet
3. `shopify-translation-manager` - Add translation keys

**App Development:**
1. `shopify-app-orchestrator` - Coordinate full implementation
2. `shopify-database-specialist` - Design product table schema
3. `shopify-api-integration` - Create product queries
4. `shopify-polaris-ui` - Build product management UI

**Polaris UI:**
1. `polaris-patterns-expert` - Use index table pattern
2. `polaris-forms-specialist` - Create product edit form
3. `polaris-layout-specialist` - Design responsive layout

## 🎯 Best Practices

1. **Use Specific Agents** - Choose the most specialized agent for your task
2. **Coordinate Complex Tasks** - Use orchestrator agents for multi-layer features
3. **Follow Patterns** - Leverage skills and established patterns
4. **Check Documentation** - Agents reference comprehensive documentation
5. **Maintain Consistency** - Use pattern-enforcer for code quality

## 🛠️ Tools & Technologies

**Theme Development:**
- Shopify Liquid
- Shopify 2.0 Sections & Blocks
- JSON Schema
- Translation Files

**App Development:**
- React 19 with SSR
- Remix Framework
- Prisma ORM
- Shopify Admin GraphQL API 2025-01
- Polaris Web Components
- Shopify App Bridge

**Polaris UI:**
- Polaris Web Components
- Design Tokens
- Responsive Breakpoints
- App Bridge Integration

## 📖 Quick Reference

| Task | Agent | Example |
|------|-------|---------|
| Create Liquid section | shopify-section-builder | Create hero banner section |
| Build app feature | shopify-app-orchestrator | Implement product sync |
| Design database | shopify-database-specialist | Create product schema |
| Shopify API query | shopify-api-integration | Fetch products with metafields |
| Build form | polaris-forms-specialist | Create product edit form |
| Page layout | polaris-layout-specialist | Design dashboard |
| Index page | polaris-patterns-expert | Build product list page |

## 🚀 Getting Started

1. **Identify Your Task Domain** - Theme, App, or Polaris UI?
2. **Choose Appropriate Agent** - Use the most specialized agent
3. **Provide Clear Context** - Specify requirements clearly
4. **Leverage Skills** - Skills provide automatic pattern support
5. **Follow Agent Guidance** - Agents follow best practices

---

**Remember**: All agents work together as a unified system. Use the right agent for each task, and leverage orchestrators for complex, multi-layer features.
