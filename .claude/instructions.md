# Claude Code Agent Instructions

This directory contains the Shopify Development Toolkit - a unified marketplace with 16 specialized agents for Shopify theme development, app development, and Polaris UI.

## Agent Invocation

When the user requests help with Shopify development tasks, analyze the request and delegate to the appropriate specialized agent:

### Theme Development Tasks
- Liquid templating → `shopify-liquid-specialist`
- Section creation → `shopify-section-builder`
- Theme settings → `shopify-global-settings`
- Snippets → `shopify-snippet-library`
- Translations → `shopify-translation-manager`

### App Development Tasks
- Full-stack features → `shopify-app-orchestrator`
- Database design → `shopify-database-specialist`
- Shopify API → `shopify-api-integration`
- App UI → `shopify-polaris-ui`
- Design compliance → `shopify-design-system`
- Code consistency → `shopify-pattern-enforcer`

### Polaris UI Tasks
- General components → `polaris-component-expert`
- Forms → `polaris-forms-specialist`
- Layouts → `polaris-layout-specialist`
- Page patterns → `polaris-patterns-expert`
- App Bridge → `polaris-app-bridge-specialist`

## Directory Structure

```
.
├── CLAUDE.md                      # Main agent documentation
├── .claude-plugin/
│   └── marketplace.json           # Unified marketplace (16 plugins)
├── shopify-theme-development/
│   ├── agents/                    # 5 theme agents
│   └── skills/                    # 6 theme skills
├── shopify-app-development/
│   ├── agents/                    # 6 app agents
│   ├── skills/                    # 3 app skills
│   └── patterns/                  # 1 safety pattern
└── shopify-polaris/
    ├── agents/                    # 5 Polaris agents
    └── skills/                    # 2 Polaris skills
```

## Skills

Skills are automatically invoked based on task context. No explicit invocation needed.

**Theme Skills:** shopify-liquid-fundamentals, shopify-section-patterns, shopify-schema-design, shopify-snippet-library, shopify-i18n-basics, shopify-workflow-tools

**App Skills:** shopify-api-patterns, polaris-ui-patterns, database-best-practices

**Polaris Skills:** polaris-fundamentals, polaris-compositions

## Best Practices

1. **Choose Specific Agents** - Use the most specialized agent for the task
2. **Use Orchestrators** - For complex multi-layer tasks
3. **Leverage Skills** - Skills provide automatic pattern support
4. **Follow Patterns** - Use established patterns from skills
5. **Check Documentation** - Refer to CLAUDE.md for guidance

## Tool Usage

- Use `Task` tool to invoke specialized agents
- Agents have access to their respective documentation paths
- Skills auto-activate based on task context
