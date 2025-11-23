# Shopify Development Toolkit - Claude Code Plugins

A comprehensive Claude Code plugin marketplace for Shopify development with 16 specialized agents covering theme development, app development, and Polaris UI.

## 🎯 Overview

This unified marketplace provides expert agents and skills for all aspects of Shopify development:

- **Theme Development** - Pure Shopify Liquid themes without framework dependencies
- **App Development** - Full-stack Shopify apps with Polaris, Prisma, and GraphQL
- **Polaris UI** - Complete Polaris Web Components reference and patterns

## 📦 Plugin Categories

### 🎨 Theme Development (5 Plugins)

Build Shopify themes with pure Liquid, no frameworks required.

1. **shopify-liquid-specialist** - Liquid templating expert
2. **shopify-section-builder** - Shopify 2.0 sections with schemas
3. **shopify-global-settings** - Theme settings management
4. **shopify-snippet-library** - Reusable Liquid snippets
5. **shopify-translation-manager** - Multi-language support

**Use for:**
- Creating sections, snippets, and templates
- Managing theme settings and customization
- Implementing internationalization

### 🚀 App Development (6 Plugins)

Build full-stack Shopify apps with modern tools.

6. **shopify-app-orchestrator** - Multi-agent coordinator for full-stack features
7. **shopify-polaris-ui** - Polaris Web Components for app UIs
8. **shopify-database-specialist** - Prisma schema and migrations
9. **shopify-api-integration** - Shopify Admin GraphQL API
10. **shopify-design-system** - Design consistency and Polaris tokens
11. **shopify-pattern-enforcer** - Codebase pattern consistency

**Use for:**
- Building complete Shopify apps
- Database design and API integration
- Ensuring code quality and consistency

### 🎭 Polaris UI (5 Plugins)

Master Polaris Web Components with expert guidance.

12. **polaris-component-expert** - Full component library access
13. **polaris-forms-specialist** - Form components and validation
14. **polaris-layout-specialist** - Page layouts and structure
15. **polaris-patterns-expert** - Composition patterns and templates
16. **polaris-app-bridge-specialist** - Native Shopify app integration

**Use for:**
- Building Polaris-based UIs
- Implementing common page patterns
- Integrating with Shopify Admin

## 🛠️ Installation

1. Clone this repository
2. Place in your project's directory
3. Invoke agents by name in your Claude Code session

## 🚀 Quick Start

### Theme Development
```
Use shopify-liquid-specialist to create a product grid section
Use shopify-section-builder to build a hero banner with schema
Use shopify-translation-manager to add multi-language support
```

### App Development
```
Use shopify-app-orchestrator to implement a bulk product update feature
Use shopify-database-specialist to design the database schema
Use shopify-api-integration to create GraphQL queries
```

### Polaris UI
```
Use polaris-component-expert to explain how to use badges
Use polaris-forms-specialist to create a product edit form
Use polaris-patterns-expert to build an index page with filters
```

## 📚 Documentation Structure

```
claude-plugins/
├── .claude-plugin/
│   └── marketplace.json          # Unified marketplace (16 plugins)
├── shopify-theme-development/
│   ├── agents/                   # 5 theme agents
│   └── skills/                   # 6 theme skills
├── shopify-app-development/
│   ├── agents/                   # 6 app agents
│   ├── skills/                   # 3 app skills
│   └── patterns/                 # Safety patterns
└── shopify-polaris/
    ├── agents/                   # 5 Polaris agents
    └── skills/                   # 2 Polaris skills
```

## 🎓 Skills

Auto-invoked knowledge bases that activate based on task context:

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

## 📖 Learning Paths

### New to Shopify Themes?
1. Start with `shopify-liquid-specialist`
2. Build sections with `shopify-section-builder`
3. Add translations with `shopify-translation-manager`

### Building Shopify Apps?
1. Use `shopify-app-orchestrator` for project coordination
2. Design database with `shopify-database-specialist`
3. Integrate API with `shopify-api-integration`
4. Build UI with `shopify-polaris-ui`

### Learning Polaris?
1. Start with `polaris-component-expert` for fundamentals
2. Build forms with `polaris-forms-specialist`
3. Create layouts with `polaris-layout-specialist`
4. Use patterns from `polaris-patterns-expert`

## 🎯 Use Cases

### Theme Development
- Creating custom sections and snippets
- Building product grids and filters
- Implementing theme settings
- Adding multi-language support
- Following Shopify best practices

### App Development
- Full-stack feature development
- Database schema design
- Shopify API integration
- Polaris UI implementation
- Code quality and consistency

### Polaris UI
- Learning Polaris components
- Building common page layouts
- Implementing design system
- App Bridge integration
- Responsive design

## 🔧 Tools & Technologies

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
- PostgreSQL/MySQL/SQLite

**Polaris UI:**
- Polaris Web Components
- Shopify App Bridge
- Design Tokens
- Responsive Breakpoints

## 🤝 Contributing

Contributions welcome! Please ensure:
- Agents follow established patterns
- Documentation is comprehensive
- Examples are practical and tested
- Skills provide actionable guidance

## 📄 License

MIT License - See LICENSE file for details

## 🔗 Resources

- [Shopify Theme Development](https://shopify.dev/docs/storefronts/themes)
- [Shopify App Development](https://shopify.dev/docs/apps)
- [Polaris Web Components](https://polaris.shopify.com/components)
- [Shopify Admin API](https://shopify.dev/docs/api/admin-graphql)
- [Shopify CLI](https://shopify.dev/docs/api/shopify-cli)

---

**Built for Claude Code** | [Report Issues](https://github.com/yourname/shopify-development-toolkit/issues)

## 📊 Plugin Summary

| Category | Plugins | Skills | Patterns |
|----------|---------|--------|----------|
| **Theme Development** | 5 | 6 | - |
| **App Development** | 6 | 3 | 1 |
| **Polaris UI** | 5 | 2 | - |
| **Total** | **16** | **11** | **1** |

All plugins work together seamlessly to provide comprehensive Shopify development support.
