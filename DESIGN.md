---
name: Velvet & Rose
colors:
  surface: '#f7f9ff'
  surface-dim: '#d7dadf'
  surface-bright: '#f7f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f4f9'
  surface-container: '#ebeef3'
  surface-container-high: '#e5e8ee'
  surface-container-highest: '#e0e3e8'
  on-surface: '#181c20'
  on-surface-variant: '#584048'
  inverse-surface: '#2d3135'
  inverse-on-surface: '#eef1f6'
  outline: '#8b7078'
  outline-variant: '#dfbec8'
  surface-tint: '#b5106b'
  primary: '#b5106a'
  on-primary: '#ffffff'
  primary-container: '#d63384'
  on-primary-container: '#ffffff'
  inverse-primary: '#ffb0cc'
  secondary: '#635c61'
  on-secondary: '#ffffff'
  secondary-container: '#e7dde2'
  on-secondary-container: '#686165'
  tertiary: '#9a3d67'
  on-tertiary: '#ffffff'
  tertiary-container: '#b95580'
  on-tertiary-container: '#130007'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffd9e4'
  primary-fixed-dim: '#ffb0cc'
  on-primary-fixed: '#3e0020'
  on-primary-fixed-variant: '#8d0051'
  secondary-fixed: '#eae0e5'
  secondary-fixed-dim: '#cec4c9'
  on-secondary-fixed: '#1f1a1e'
  on-secondary-fixed-variant: '#4b4549'
  tertiary-fixed: '#ffd9e4'
  tertiary-fixed-dim: '#ffb0cd'
  on-tertiary-fixed: '#3e0021'
  on-tertiary-fixed-variant: '#7d254f'
  background: '#f7f9ff'
  on-background: '#181c20'
  surface-variant: '#e0e3e8'
typography:
  display:
    fontFamily: Bodoni Moda
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Bodoni Moda
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Bodoni Moda
    fontSize: 28px
    fontWeight: '500'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Bodoni Moda
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  link-label:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  caption:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.4'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 480px
  gutter: 1rem
  margin-x: 1.5rem
  stack-sm: 0.75rem
  stack-md: 1.5rem
  stack-lg: 3rem
---

## Brand & Style

This design system is curated for a high-end women's fashion audience, embodying a "Chic Editorial" aesthetic. It balances the vibrant energy of high-fashion pinks with the grounded luxury of deep plum and charcoal. The visual narrative is sophisticated, feminine, and authoritative, positioning the brand as a tastemaker in the fashion space.

The style leverages **Minimalism** through generous whitespace and intentional content hierarchy, blended with **Tonal Layers** to create a sense of depth without clutter. It evokes the feeling of browsing a premium digital lookbook—clean, airy, and effortlessly stylish.

## Colors

The palette is anchored by the interplay between **Secondary (#FDF2F7)**, used as the primary canvas color to provide a soft, luminous background, and **Neutral (#212529)** for high-contrast, legible typography. 

- **Primary (#D63384):** Reserved for high-impact calls to action, active states, and decorative accents. It represents the "vibrant" core of the fashion house.
- **Tertiary (#701A45):** Used for secondary headings, borders, and subtle interactive elements to add a layer of "Deep Plum" sophistication.
- **Surface Strategy:** Use white or #FDF2F7 for page backgrounds. Use Tertiary and Primary in small doses to maintain a high-end, exclusive feel.

## Typography

The typography system employs a "Modern Editorial" pairing. **Bodoni Moda** provides a high-contrast serif foundation that screams luxury and fashion heritage. It should be used for brand names, section titles, and featured product names.

**Hanken Grotesk** serves as the functional counterpart. Its clean, contemporary geometry ensures that links and body copy remain highly readable on mobile devices. Use uppercase styling for labels and buttons to create a structured, "designer label" look.

## Layout & Spacing

Designed specifically for a "Link in Bio" context, the layout follows a **fixed-width container model** centered on the screen, optimized for mobile viewing (max-width 480px). 

The spacing rhythm is airy. Content blocks should be separated by `stack-md` or `stack-lg` to prevent the UI from feeling cramped. Elements within a card or link group should use `stack-sm`. Use a 12-column grid within the container for internal alignment of thumbnails and text.

## Elevation & Depth

To maintain a sophisticated feel, this design system avoids heavy, dark shadows. Instead, it utilizes **Ambient Shadows** and **Tonal Layers**:

- **Soft Depth:** Elements like primary buttons and featured cards use a very diffused shadow: `0px 4px 20px rgba(112, 26, 69, 0.08)`. This uses a tint of the Tertiary color to keep the shadow "warm" rather than grey.
- **Glassmorphism (Subtle):** For floating navigation or header bars, use a backdrop blur (12px) with a 90% opaque #FDF2F7 background to maintain a sense of lightness.

## Shapes

The shape language is defined as **Rounded**, providing a soft, approachable femininity without becoming "bubbly." 

- Base components (buttons, input fields) use a 0.5rem (8px) radius.
- Large containers (cards, image frames) use a 1rem (16px) radius.
- Interactive icons and avatars should be perfectly circular to contrast against the structured rectangular links.

## Components

### Buttons
- **Primary:** Background #D63384, Text #FFFFFF. 0.5rem roundedness. Subtle shadow on hover.
- **Secondary (Outline):** Border 1px #701A45, Text #701A45. No fill. Use for less critical actions like "View Gallery."

### Link Cards
- These are the hero components. Use a full-width #FFFFFF background with a 1px #FDF2F7 border. 
- Left-align text using `link-label` typography.
- Include a small circular thumbnail (32x32px) on the left for product-specific links.

### Input Fields
- For newsletter signups, use a minimal bottom-border style or a very soft filled field (#FDF2F7).
- Placeholder text should be in Neutral (#212529) at 50% opacity.

### Featured Chips
- Use for "New Arrival" or "Sale" tags. Small, uppercase text on a Primary (#D63384) background with 100px pill-rounding.

### Image Grids
- Use a 2-column masonry or square grid for "Shop the Look" sections. Images should have a 0.5rem corner radius to match the button style.