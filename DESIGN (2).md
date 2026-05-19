---
name: Stark Poeticism
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#47464b'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#77767b'
  outline-variant: '#c8c5cb'
  surface-tint: '#5e5e63'
  primary: '#19191e'
  on-primary: '#ffffff'
  primary-container: '#2e2e33'
  on-primary-container: '#97959b'
  inverse-primary: '#c8c5cc'
  secondary: '#5e5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e3e2e2'
  on-secondary-container: '#646464'
  tertiary: '#1d1912'
  on-tertiary: '#ffffff'
  tertiary-container: '#322e26'
  on-tertiary-container: '#9c958a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e4e1e8'
  primary-fixed-dim: '#c8c5cc'
  on-primary-fixed: '#1b1b20'
  on-primary-fixed-variant: '#46464c'
  secondary-fixed: '#e3e2e2'
  secondary-fixed-dim: '#c7c6c6'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#464747'
  tertiary-fixed: '#eae1d5'
  tertiary-fixed-dim: '#cdc5ba'
  on-tertiary-fixed: '#1f1b14'
  on-tertiary-fixed-variant: '#4b463d'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
  canvas-white: '#FFFFFF'
  ink-black: '#000000'
  fossil-grey: '#808080'
typography:
  display-lg:
    fontFamily: EB Garamond
    fontSize: 72px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: EB Garamond
    fontSize: 48px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: EB Garamond
    fontSize: 40px
    fontWeight: '400'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: EB Garamond
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
  label-small:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1.4'
spacing:
  unit: 8px
  margin-page: 64px
  margin-mobile: 24px
  gutter: 32px
  section-gap: 128px
---

## Brand & Style

This design system is built on the philosophy of "essentialism as luxury." It balances a high-end, editorial aesthetic with a utilitarian logic, creating a digital environment that feels both poetic and employable. 

The visual direction follows a **High-End Minimalism** approach. It leverages extreme whitespace, a strictly monochromatic palette, and the tension between classic serif typography and modern grotesque faces. The goal is to evoke a sense of quiet authority, clarity, and timelessness. Interfaces should feel like a well-typeset printed folio—spacious, intentional, and devoid of unnecessary decoration.

## Colors

The palette is intentionally restrained to prioritize content and legibility. 

- **Canvas-White (#FFFFFF):** The primary background surface. It must be used generously to create the "poetic" breathing room required.
- **Ink-Black (#000000) & Deep Charcoal (#2E2E33):** Used for primary text and high-contrast actions. While #000000 is used for large headlines to create impact, #2E2E33 provides a slightly softer reading experience for long-form body text.
- **Neutral Accents (#F5F5F5 / #808080):** Used for subtle structural divisions, disabled states, and secondary metadata.

Avoid using gradients or saturated colors. Depth is achieved through contrast and scale rather than hue.

## Typography

The typographic hierarchy is the cornerstone of this design system. It uses **EB Garamond** for an intellectual, editorial feel in headlines and **Inter** for functional, modern clarity in body text and interface elements.

- **Headlines:** Use EB Garamond with tight letter-spacing for large sizes. The "poetic" nature comes from the serif's organic curves contrasted against the rigid layout.
- **Body:** Use Inter with generous line-height to ensure maximum readability and a "clean" feel.
- **Labels:** Small caps with tracking (letter-spacing) should be used for secondary navigation or categories to provide a technical, "employable" touch to the editorial style.

## Layout & Spacing

The layout is based on a **fixed-width, high-margin grid** for desktop and a fluid single-column for mobile. 

- **The Void:** Use "section-gap" (128px) to separate primary content blocks. This creates the "high-end" feeling by proving the product isn't afraid of empty space.
- **Alignment:** All text should generally be left-aligned to maintain a strong vertical "spine" for the user's eye, mimicking professional typesetting.
- **The Grid:** A 12-column grid is used for desktop (1140px max-width), but content is often pushed to the center 8 columns to maximize the surrounding white space.

## Elevation & Depth

This design system rejects shadows and blurs in favor of **Tonal Layers** and **Hairline Borders**.

- **Flat Depth:** Hierarchy is established by stacking surfaces of #FFFFFF (Canvas) on #F5F5F5 (Neutral).
- **Hairlines:** 1px solid lines in #2E2E33 (at 10-15% opacity) or #F5F5F5 should be the only method of defining boundaries.
- **Interaction:** Depth is conveyed through movement or state changes (e.g., a button filling with solid black on hover) rather than Z-axis shadows.

## Shapes

The shape language is strictly **Sharp (0px)**. 

Every UI element—from buttons and input fields to card containers—must feature 90-degree corners. This reinforces the architectural, structured, and professional nature of the system. Circular elements are only permitted for profile avatars or specific status indicators to provide a single point of organic contrast.

## Components

- **Buttons:** Primary buttons are solid Ink-Black with white Inter-Medium text. Secondary buttons are 1px black outlines. All buttons feature sharp corners and high horizontal padding.
- **Input Fields:** Minimalist under-lines or very light grey 1px boxes. Labels sit above the field in `label-caps`. Focus states are indicated by the line becoming solid Ink-Black.
- **Cards:** Cards should not have shadows. Use 1px #F5F5F5 borders or simply use whitespace to group content. 
- **Chips:** Small, sharp-edged rectangles with `label-small` text. Used for categorization without adding visual weight.
- **Lists:** High-density text separated by 1px hairlines that span the full width of the container. 
- **Navigation:** Simple text links in Inter. The active state is indicated by a simple underline or a weight change, never a background "pill."