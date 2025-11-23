# Shopify Polaris - Claude Code Plugin

A comprehensive Claude Code plugin providing complete Polaris Web Components reference, patterns, and expert guidance for building Shopify apps.

## 🎯 Overview

This plugin provides specialized agents and skills for working with Shopify's Polaris Web Components design system, including:

- **Complete Component Library** - All Polaris Web Components (actions, forms, feedback, media, structure, text)
- **Composition Patterns** - Templates for common page layouts and UI patterns
- **App Bridge Integration** - Native Shopify app integration components
- **Design System Guidelines** - Best practices for Polaris design tokens and patterns

## 📦 Included Plugins

### 1. **polaris-component-expert**
General Polaris Web Components expert with access to the full component library.

**Use for:**
- Choosing the right component for your use case
- Understanding component properties and usage
- Learning Polaris Web Components fundamentals

**Example:**
```
Use polaris-component-expert to help me build a product selection interface
```

### 2. **polaris-forms-specialist**
Expert in Polaris form components and validation.

**Use for:**
- Building forms with text fields, checkboxes, selects
- Implementing form validation
- Creating file upload interfaces

**Example:**
```
Use polaris-forms-specialist to create a product edit form
```

### 3. **polaris-layout-specialist**
Expert in Polaris layout and structure components.

**Use for:**
- Creating page layouts with s-page, s-card, s-section
- Building responsive grids and stacks
- Organizing content with proper spacing

**Example:**
```
Use polaris-layout-specialist to design a dashboard layout
```

### 4. **polaris-patterns-expert**
Expert in Polaris composition patterns and templates.

**Use for:**
- Implementing index tables with actions
- Creating settings pages
- Building homepage layouts
- Using established UI patterns

**Example:**
```
Use polaris-patterns-expert to create an index page with filters
```

### 5. **polaris-app-bridge-specialist**
Expert in Shopify App Bridge components.

**Use for:**
- Implementing app navigation
- Creating title bars with actions
- Integrating native Shopify features
- Building embedded app experiences

**Example:**
```
Use polaris-app-bridge-specialist to setup app navigation
```

## 📚 Component Categories

### Actions
- Button
- Button Group
- Link
- Icon Button

### Forms
- Text Field
- Checkbox
- Select
- Color Picker
- Drop Zone
- Password Field
- Search Field
- Number Field
- URL Field

### Feedback
- Banner
- Toast
- Progress Bar
- Spinner
- Skeleton

### Media
- Avatar
- Icon
- Thumbnail
- Video Thumbnail

### Structure
- Page
- Card
- Section
- Box
- Grid
- Stack
- Divider
- List
- Table

### Titles and Text
- Heading
- Text
- Paragraph
- Badge
- Chip

## 🛠️ Installation

1. Clone or download this repository
2. Place in your project's `claude-plugins/` directory
3. Invoke agents by name in your Claude Code session

## 🚀 Quick Start

### For General Component Help
```
Use polaris-component-expert to explain how to use badges
```

### For Form Building
```
Use polaris-forms-specialist to create a customer registration form
```

### For Layout Design
```
Use polaris-layout-specialist to build a three-column dashboard
```

### For Common Patterns
```
Use polaris-patterns-expert to implement a resource index page
```

### For App Integration
```
Use polaris-app-bridge-specialist to setup title bar with breadcrumbs
```

## 📖 Skills

This plugin includes skills that provide:
- Component usage patterns and examples
- Composition templates for common layouts
- App Bridge integration patterns
- Design system best practices

Skills are automatically invoked when working with relevant components.

## 🎓 Learning Resources

- [Polaris Web Components Documentation](https://polaris.shopify.com/components)
- [Shopify App Bridge](https://shopify.dev/docs/api/app-bridge)
- [Polaris Design Tokens](https://polaris.shopify.com/tokens)

## 📁 Directory Structure

```
polaris-web-components/
├── components/           # Full component library
│   ├── actions/
│   ├── feedback/
│   ├── forms/
│   ├── media/
│   ├── structure/
│   └── titles-and-text/
├── app-bridge-components/  # App Bridge integration
│   ├── app-nav.md
│   ├── app-window.md
│   ├── forms.md
│   └── title-bar.md
└── patterns/             # Composition patterns
    ├── compositions/
    └── templates/
```

## 🤝 Contributing

Contributions welcome! Please ensure agents follow Polaris design principles and include proper documentation.

## 📄 License

MIT License - See LICENSE file for details

---

**Built for Claude Code** | [Report Issues](https://github.com/yourname/shopify-polaris/issues)
