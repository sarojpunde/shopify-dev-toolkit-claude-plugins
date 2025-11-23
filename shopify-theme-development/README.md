# Shopify Theme Development - Claude Code Plugins

**Pure, unopinionated Shopify theme development tools**

This marketplace provides Claude Code plugins for building Shopify themes using vanilla Liquid, CSS, and JavaScript - no frameworks, no build tools, no custom conventions.

## Philosophy

- ✅ **Framework-agnostic**: Pure Shopify standards only
- ✅ **No build tools**: Direct deployment, instant changes
- ✅ **Unopinionated**: No enforced naming conventions or patterns
- ✅ **Beginner-friendly**: Lower barrier to entry
- ✅ **Shopify-first**: Follows official Shopify best practices

## Plugins

### 1. Shopify Liquid Specialist
Expert in Shopify Liquid templating for sections, snippets, and templates.

**Features**:
- Pure Liquid code generation
- Schema validation
- Inline CSS/JS with `{% stylesheet %}` and `{% javascript %}` tags
- Translation key management
- No framework dependencies

**Use for**: Creating sections, snippets, handling Liquid logic

### 2. Shopify Section Builder
Specialized in building Shopify 2.0 sections with complete schema.

**Features**:
- Complete section structure
- Merchant-configurable settings
- Block integration
- Mobile-responsive CSS Grid
- Vanilla JavaScript interactivity

**Use for**: Building customizable theme sections

### 3. Shopify Global Settings
Manages `config/settings_schema.json` for theme-wide settings.

**Features**:
- Color scheme configuration
- Typography settings
- Layout settings
- Social media links
- Cart behavior settings

**Use for**: Setting up global theme configuration

### 4. Shopify Snippet Library
Creates reusable Liquid snippets with documentation.

**Features**:
- Product cards
- Form elements
- Icons and UI components
- Proper parameter documentation
- Reusable code fragments

**Use for**: Building reusable theme components

### 5. Shopify Translation Manager
Handles multi-language support and locale files.

**Features**:
- Locale file management
- Schema translation keys
- i18n patterns
- Translation validation

**Use for**: Multi-language theme support

## Installation

```bash
# Add this marketplace to Claude Code
/plugin marketplace add shopify-theme-development

# Install specific plugins
/plugin install shopify-liquid-specialist
/plugin install shopify-section-builder
```

## Usage Example

```
> Use shopify-liquid-specialist to create a featured products section
> Use shopify-global-settings to add color scheme settings
> Use shopify-snippet-library to create a product card snippet
```

## Project Structure

```
your-theme/
├── sections/
│   └── featured-products.liquid    # All code in one file
├── snippets/
│   └── product-card.liquid
├── locales/
│   ├── en.default.json
│   └── en.default.schema.json
├── config/
│   ├── settings_schema.json        # Global theme settings
│   └── settings_data.json
├── layout/
│   └── theme.liquid
├── templates/
│   └── index.json
└── assets/
    └── images/                      # Static files only
```

## Key Differences from Framework Approaches

| Aspect | This Marketplace | Framework-Based |
|--------|-----------------|-----------------|
| CSS | Inline `{% stylesheet %}` | External files + build tools |
| JavaScript | Inline `{% javascript %}` | Webpack/bundlers |
| Styling | Vanilla CSS | Tailwind/Sass |
| Interactivity | Vanilla JS | Alpine.js/React |
| Deploy | Direct push to Shopify | Build step required |
| Learning Curve | Lower | Higher |

## When to Use This Marketplace

✅ **Use when**:
- Building simple to medium complexity themes
- Team unfamiliar with modern build tools
- Want fastest development iteration
- Prefer minimal dependencies
- Need lower barrier to entry

❌ **Consider framework-based when**:
- Building complex, enterprise themes
- Need utility-first CSS
- Want reactive components
- Team comfortable with tooling
- Performance optimization critical

## License

MIT

## Contributing

Issues and pull requests welcome at: [your-repo-url]

## Support

- Documentation: [your-docs-url]
- Issues: [your-issues-url]
- Discussions: [your-discussions-url]
