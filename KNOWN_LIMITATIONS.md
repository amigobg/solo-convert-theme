# Known Limitations - Solo Convert Theme v1.0

This document outlines known limitations and potential future enhancements for the Solo Convert theme.

## Current Limitations

### 1. Variant Price Updates
**Issue:** When selecting different product variants, the displayed price doesn't update dynamically.

**Impact:** Minor - Shopify's native behavior still works correctly, and the correct price shows at checkout.

**Reason:** Maintaining minimal JavaScript philosophy. Adding dynamic price updates would require ~50-100 lines of JS.

**Workaround:** 
- Product prices are shown correctly on initial load
- Cart and checkout show accurate pricing
- For products with significant price variations, consider creating separate products

**Future Enhancement:** Could add optional JavaScript module for dynamic price updates in v2.0.

---

### 2. Sticky Cart Variant Sync
**Issue:** The sticky add-to-cart doesn't reflect variant changes made in the hero form.

**Impact:** Low - The sticky button triggers the hero form submission, so the selected variant is added correctly.

**Reason:** Minimal JavaScript approach. Syncing would require event listeners and state management.

**Workaround:** The sticky button correctly adds whatever variant is currently selected in the hero form.

**Future Enhancement:** Could add variant sync in v2.0 with optional JavaScript module.

---

### 3. Comparison Table Flexibility
**Issue:** Comparison table is limited to exactly 2 competitors maximum.

**Impact:** Low - Most effective comparisons show 1-2 alternatives anyway.

**Reason:** Simplified schema and code for easier merchant configuration.

**Workaround:** 
- Use 1 or 2 competitors (both work fine)
- For more complex comparisons, use Image with Text sections

**Future Enhancement:** Could make fully dynamic in v2.0.

---

### 4. Star Rating Display
**Issue:** Star rating uses inline CSS custom properties instead of CSS classes.

**Impact:** Negligible - Minimal HTML/CSS impact, still very performant.

**Reason:** Simpler implementation for dynamic percentage-based fills.

**Workaround:** None needed - performance impact is minimal.

**Future Enhancement:** Could refactor to use CSS classes with discrete ratings (0.5, 1, 1.5, etc.).

---

## Design Decisions (Not Bugs)

### Single Product Focus
**Decision:** Theme is designed for ONE hero product only.

**Why:** Removes distractions, increases conversion rates for single-product brands.

**Alternative:** For multiple products, use Shopify's standard themes or create separate stores.

---

### Minimal JavaScript
**Decision:** Only ~100 lines of JS total (sticky cart only).

**Why:** Performance, simplicity, reliability. CSS-first approach.

**Trade-off:** Some dynamic features require page refresh or manual merchant configuration.

---

### Simplified Settings
**Decision:** Yes/No options instead of complex custom inputs.

**Why:** Easier for merchants, fewer errors, clearer choices.

**Trade-off:** Less flexibility in some areas (e.g., comparison table).

---

## Not Planned

These features are intentionally excluded to maintain focus:

- Multi-product support
- Complex variant selection UI
- Product recommendations
- Upsell/cross-sell modules
- Collection browsing
- Advanced search
- Blog integration (beyond basic templates)
- Complex animations
- JavaScript frameworks
- CSS frameworks

---

## Future Roadmap (Potential v2.0)

If there's demand, future versions could include:

1. **Optional JavaScript Module**
   - Dynamic price updates
   - Variant image switching
   - Sticky cart sync
   - Can be toggled on/off for performance

2. **Extended Comparison Features**
   - Dynamic competitor columns
   - Custom text values
   - Image comparisons

3. **Advanced Testimonials**
   - Video testimonials
   - Carousel/slider
   - Instagram integration

4. **Scarcity Features**
   - Inventory counter
   - Timer countdown
   - Limited edition badge

5. **Analytics Integration**
   - Conversion tracking helpers
   - A/B testing support
   - Heat map compatibility

---

## Contributing

If you'd like to address any of these limitations or add features, please:

1. Read CONTRIBUTING.md
2. Keep changes minimal and focused
3. Maintain the single-product, conversion-first philosophy
4. Ensure mobile-first responsive design
5. Avoid adding dependencies

---

## Version Philosophy

**v1.0 Goal:** Simple, fast, conversion-focused, works out of the box.

**Future Goals:** Optional enhancements that maintain core simplicity.

---

## Support

For questions about limitations or feature requests:
- GitHub Issues: [Report here](https://github.com/amigobg/solo-convert-theme/issues)
- Documentation: [README.md](README.md)
- Merchant Guide: [MERCHANT_GUIDE.md](MERCHANT_GUIDE.md)

---

**Remember:** These limitations are intentional trade-offs for simplicity, performance, and focus. For most single-product DTC brands, the current feature set is more than sufficient.
