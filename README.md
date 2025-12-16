<h1 align="center" style="position: relative;">
  <br>
    <img src="./assets/shoppy-x-ray.svg" alt="logo" width="200">
  <br>
  Solo Convert - Single Product Shopify Theme
</h1>

A **high-converting Shopify theme** purpose-built for **one product only**. Designed for DTC brands selling a hero product with paid traffic (Meta, Google, TikTok). Optimized for **maximum conversion rate, speed, and clarity**.

<p align="center">
  <a href="./LICENSE.md"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License"></a>
</p>

---

## 🎯 Purpose

This theme transforms your product page into a **landing-page style storefront** focused on:

* **High Conversion** – Trust, clarity, urgency built-in
* **Mobile-First UX** – Designed for mobile before desktop
* **Fast Load Time** – Core Web Vitals optimized, minimal JS
* **Simple Customization** – Theme Editor ready for non-technical merchants

**This theme outperforms generic multi-product themes** for single-product businesses.

---

## ✨ Key Features

### Conversion-Optimized Sections

All sections are designed following CRO (Conversion Rate Optimization) best practices:

1. **Hero Product** - Above-the-fold product display with:
   - Product title & core benefit (not just description)
   - Price with compare-at pricing
   - Star rating (static or metafield-driven)
   - Primary CTA (Add to Cart / Buy Now)
   - Payment badges (Shop Pay, Apple Pay, etc.)
   - Trust signals

2. **Product Benefits** - Icon + copy benefits section
   - Highlight 3-6 core benefits
   - Visual icons or emojis
   - Clear, benefit-driven copy

3. **Social Proof** - Testimonials & reviews
   - Customer testimonials with ratings
   - Customer photos
   - Social proof statistics

4. **Image with Text** - Problem → Solution narrative
   - Flexible layout (image left/right)
   - Storytelling format
   - Key points with icons

5. **Comparison Table** - vs. Alternatives
   - Compare your product with competitors
   - Highlight your advantages
   - Mobile-optimized table

6. **Guarantee** - Risk reversal
   - Money-back guarantee messaging
   - Trust-building content
   - Reduce purchase anxiety

7. **FAQ** - Accordion style
   - Answer common objections
   - Clean, collapsible design
   - Overcome purchase barriers

8. **Sticky Add to Cart** - Mobile CTA
   - Appears on scroll (mobile only)
   - Always accessible CTA
   - Boosts mobile conversion

---

## 🚀 Getting Started

### Prerequisites

Before starting, ensure you have the latest Shopify CLI installed:

- [Shopify CLI](https://shopify.dev/docs/api/shopify-cli) – helps you download, upload, preview themes, and streamline your workflows

If you use VS Code:

- [Shopify Liquid VS Code Extension](https://shopify.dev/docs/storefronts/themes/tools/shopify-liquid-vscode) – provides syntax highlighting, linting, inline documentation, and auto-completion

### Installation

Clone this repository:

```bash
git clone git@github.com:amigobg/solo-convert-theme.git
cd solo-convert-theme
```

### Preview

Preview this theme using Shopify CLI:

```bash
shopify theme dev
```

### Deploy

Push to your Shopify store:

```bash
shopify theme push
```

---

## 📋 Setup Guide

### 1. Set Your Product Page as Homepage

Since this is a single-product theme, set your main product page as the homepage:

1. Go to **Online Store > Navigation**
2. Edit the **Home** link
3. Point it to your main product page

Or use the default homepage with a CTA button to your product.

### 2. Customize Sections

All sections are fully customizable via the Theme Editor:

1. Go to **Online Store > Themes > Customize**
2. Navigate to your product page
3. Configure each section:
   - Upload images
   - Add copy
   - Customize colors
   - Enable/disable features

### 3. Configure Settings

#### Typography
- Choose your primary font
- System fonts recommended for performance

#### Layout
- Page width (Narrow/Wide)
- Page margins

#### Colors
- Background color
- Foreground (text) color
- Input corner radius

---

## 🎨 Theme Architecture

```bash
.
├── assets          # CSS, icons, images
├── blocks          # Reusable, nestable components
├── config          # Theme settings
├── layout          # Page wrappers (theme.liquid)
├── locales         # Translation files
├── sections        # Conversion-focused sections
│   ├── hero-product.liquid
│   ├── benefits.liquid
│   ├── social-proof.liquid
│   ├── image-with-text.liquid
│   ├── comparison-table.liquid
│   ├── guarantee.liquid
│   ├── faq.liquid
│   └── sticky-add-to-cart.liquid
├── snippets        # Reusable code fragments
└── templates       # Page templates (product.json)
```

---

## ⚡ Performance

This theme is optimized for speed:

- **No jQuery** - Pure vanilla JS only when needed
- **Minimal JavaScript** - CSS-first approach
- **Critical CSS** - Inlined for fast first paint
- **Font Optimization** - Preconnect & preload
- **Lazy Loading** - Images load on demand
- **Target: Lighthouse 90+ mobile**

---

## 🎯 Best Practices

### Merchant-Friendly Labels

Settings use marketing language, not developer jargon:

- ❌ "Heading Text"
- ✅ "Main Benefit Headline"

### Conversion-First Design

Every section follows proven CRO principles:

1. **One Product, One Goal** – Remove distractions
2. **Mobile First** – Design for mobile before desktop  
3. **Speed Over Everything** – Minimal bloat
4. **Above-the-Fold Conversion** – CTA visible immediately
5. **Trust Before Features** – Credibility early

### Section Order

The product template follows this proven conversion flow:

1. Hero Product (above the fold)
2. Benefits (why choose this)
3. Story/Problem-Solution
4. Social Proof (testimonials)
5. Comparison (vs alternatives)
6. Guarantee (risk reversal)
7. FAQ (overcome objections)
8. Sticky CTA (mobile)

---

## 🛠️ Customization

### Adding Custom Sections

All sections are modular. You can:

- Reorder sections in Theme Editor
- Duplicate sections
- Hide/show sections
- Customize all content

### Section Settings

Each section has merchant-friendly settings:

- **Hero Product**: Core benefit, CTA text, trust signals
- **Benefits**: Icons, titles, descriptions
- **Social Proof**: Testimonials, ratings, stats
- **Comparison**: Features, competitors
- **Guarantee**: Guarantee copy, features
- **FAQ**: Questions & answers

---

## 📱 Mobile Optimization

This theme is **mobile-first**:

- Large tap targets (min 44x44px)
- Sticky Add to Cart on mobile
- Optimized typography scaling
- Touch-friendly accordions
- Responsive grid layouts

---

## ♿ Accessibility

- Semantic HTML
- Proper heading hierarchy
- Alt text support on all images
- Keyboard navigation
- ARIA labels where needed

---

## 📊 SEO

- SEO-friendly product schema
- Meta tags support
- Proper heading structure
- Fast page load (ranking factor)

---

## 🤝 Contributing

We welcome contributions! This theme aims to remain lean and conversion-focused. Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

---

## 📄 License

Solo Convert Theme is open-sourced under the [MIT](./LICENSE.md) License.

---

## 💡 Tips for Success

1. **Use High-Quality Images** - Professional product photos increase trust
2. **Write Benefit-Driven Copy** - Focus on outcomes, not features
3. **Test Your Headlines** - A/B test different benefit statements
4. **Gather Real Testimonials** - Authentic reviews build credibility
5. **Keep It Simple** - Less is more for conversion

---

## 🎓 Learn More

- [Shopify Theme Development](https://shopify.dev/docs/storefronts/themes)
- [Liquid Template Language](https://shopify.dev/docs/api/liquid)
- [Theme Architecture](https://shopify.dev/docs/storefronts/themes/architecture)
- [Performance Optimization](https://shopify.dev/docs/storefronts/themes/best-practices/performance)

---

**Built for merchants who want to sell one product really, really well.**
