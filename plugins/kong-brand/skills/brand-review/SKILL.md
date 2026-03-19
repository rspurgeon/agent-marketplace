---
description: Apply Kong brand guidelines when generating or reviewing code, CSS, HTML, web pages, demos, presentations, or any visual content. Use when asked to make something "Kong branded" or conform to Kong brand standards.
---

# Kong Brand Review

You are applying the Kong Brand Guidelines 2026 v1.1. Read the full reference at `references/brand-guidelines.md` before proceeding.

## When generating or modifying code/content:

### Colors
- Use the official Kong color palette. Define CSS custom properties as shown in the reference.
- **Default to dark theme:** Dark Green (`#000F06`) backgrounds with Electric Lime (`#CCFF00`) accents. This is the priority theme.
- Use the gray scale for secondary UI elements (`#E7EDE5` through `#101110`).
- Bay (`#B7BDB5`) is the neutral color for muted/secondary text and borders.
- Text on dark backgrounds: `#F7F9FC` (near-white). Text on light backgrounds: `#35363A`.
- Never use off-brand colors for primary UI elements. If the existing code has non-brand colors, replace them with the nearest brand equivalent.

### Typography
- Use **Funnel Sans** for headings and body text, **Roboto Mono** for code blocks, and **Space Grotesk** for buttons/UI labels.
- Include the Google Fonts import shown in the reference.
- Follow the type hierarchy: Heading XL (72/78), Heading L (32/38), Body L (20/28).

### Dark Theme First
- Kong's brand is dark-dominant. Default to dark backgrounds unless the user specifically requests a light theme.
- If a light theme is requested, use Bay (`#B7BDB5`) or White (`#FFFFFF`) backgrounds with dark text (`#35363A`).

### Product Names
- Always use the exact product names from the reference (e.g., "Kong Konnect" not "Kong Connect").
- Always include "Kong" as a prefix — never write just "Gateway" or "Mesh" alone in external-facing content.

### Logo Usage
- On dark backgrounds: Electric Lime logomark + near-white text.
- On light backgrounds: black logomark + `#35363A` text.
- Maintain 1X clear space around logos.
- Never modify, distort, recolor (outside approved themes), or add effects to the logo.
- For co-branding: use a vertical divider with 1X spacing on each side.

### Graphic Style
- Use blueprint-style grid lines, cross markers, and tee intersections as decorative elements where appropriate.
- Favor clean, architectural layouts with structured grids.
- For hero sections or visual emphasis, consider connectivity layer patterns (flowing 3D ribbon forms).

## When reviewing existing content:

Check for and flag:
1. Colors not in the brand palette
2. Wrong product names (e.g., "Kong Connect" instead of "Kong Konnect")
3. Logo misuse (wrong colors for background, missing clear space, modifications)
4. Non-brand fonts where brand fonts should be used
5. Light themes used where dark theme would be more brand-appropriate

Suggest specific fixes with exact hex values, font names, and product name corrections.
