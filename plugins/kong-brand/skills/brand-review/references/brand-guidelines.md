# Kong Brand Guidelines 2026 v1.1

## Company Identity

- **Company name:** Kong
- **Tagline:** The AI Connectivity Company
- **Website:** konghq.com
- **Brand contact:** design@konghq.com

## Design Principles

### Speed
Innovation is about how quickly a product improves once it touches the real world. Speed compresses steps into a continuous, fluid motion.

### Electric
As fast as electricity, Kong dissolves the barriers between data and decision, creating a connectivity layer so fast, so fluid, and so reliable that it becomes an invisible extension of the human will.

### Architect
Structure, intent, and system thinking. The discipline of designing before building — where complexity is resolved through clarity, and ambition is grounded in sound frameworks.

---

## Logo

### Emblem (Logomark)
The brand's most essential asset: a singular, bold mark called "The Walker" — a symbol of perpetual motion and forward intent. It embodies the explorer mindset. Composed of distinct elements working in harmony, the mark reflects the belief that independent parts, when intelligently connected, can move as one.

### Logotype (Wordmark)
The Kong logotype is bold and highly legible, designed for clarity and impact across digital and printed environments. Its geometric structure conveys strength and precision, while subtle curves add balance and approachability.

### Logo Forms
- **Logomark:** The emblem only (The Walker symbol)
- **Logotype:** The emblem + "Kong" wordmark together

### Logo Themes

| Theme | Background | Logomark Color | Text Color | Usage |
|-------|-----------|---------------|------------|-------|
| Dark | Dark Green `#000F06` | Electric Lime `#CCFF00` | Near-white `#F7F9FC` | **Priority usage** |
| Electric | Electric Lime `#CCFF00` | Black `#000000` | Black `#000000` | **Priority usage** |
| Bay | Bay `#B7BDB5` | Gray | Gray | Secondary |
| White | White `#FFFFFF` | Gray `#35363A` | Gray `#35363A` | Secondary |

### Logo on Light Backgrounds
- Logomark: black (no explicit fill — defaults to black)
- Logotype text: `#35363A` (dark gray)

### Logo on Dark Backgrounds
- Logomark: Electric Lime `#CCFF00`
- Logotype text: `#F7F9FC` (near-white)

### Clear Space
Maintain 1X clear space on all sides of the logo, where X is derived from the logo's proportions.

### Logo Rules
- Do NOT modify the trademarks or use them in an altered way
- Do NOT suggest sponsorship or endorsement by Kong
- Do NOT confuse Kong with another brand
- Do NOT change logo colors outside the approved themes
- Do NOT distort, rotate, or add effects to the logo

### Co-branding
- Use a vertical divider between the Kong logo and partner logo
- Maintain 1X spacing: 1X from Kong logo to divider, 1X from divider to partner logo

---

## Colors

### Primary Palette

| Name | Hex | RGB | HSL | CMYK | Pantone | Usage |
|------|-----|-----|-----|------|---------|-------|
| Dark Green | `#000F06` | R:0 G:15 B:6 | H:144 S:100 B:6 | C:75 M:60 Y:70 K:85 | Black 3 U | Primary background |
| Electric Lime | `#CCFF00` | R:204 G:255 B:0 | H:72 S:100 B:100 | C:25 M:0 Y:100 K:0 | 2297 U | Primary accent |
| Bay | `#B7BDB5` | R:183 G:189 B:181 | H:105 S:4 B:74 | C:30 M:20 Y:27 K:0 | 7527 U | Neutral / secondary |
| White | `#FFFFFF` | R:255 G:255 B:255 | H:0 S:0 B:100 | C:0 M:0 Y:0 K:0 | White U | Backgrounds, text |

### Gray Scale

| Step | Hex | Usage Notes |
|------|-----|-------------|
| 50 | `#E7EDE5` | Lightest gray |
| 100 | `#D7DED4` | |
| 200 | `#CDD4CB` | |
| 300 | `#B7BDB5` | = Bay (primary neutral) |
| 400 | `#A1A69F` | |
| 500 | `#858983` | |
| 600 | `#676B66` | |
| 700 | `#4A4D49` | |
| 800 | `#2D2E2C` | |
| 900 | `#101110` | Darkest gray |

### CSS Custom Properties (recommended)

```css
:root {
  /* Primary palette */
  --kong-dark-green: #000F06;
  --kong-electric-lime: #CCFF00;
  --kong-bay: #B7BDB5;
  --kong-white: #FFFFFF;

  /* Gray scale */
  --kong-gray-50: #E7EDE5;
  --kong-gray-100: #D7DED4;
  --kong-gray-200: #CDD4CB;
  --kong-gray-300: #B7BDB5;
  --kong-gray-400: #A1A69F;
  --kong-gray-500: #858983;
  --kong-gray-600: #676B66;
  --kong-gray-700: #4A4D49;
  --kong-gray-800: #2D2E2C;
  --kong-gray-900: #101110;

  /* Semantic aliases */
  --kong-bg-primary: var(--kong-dark-green);
  --kong-accent: var(--kong-electric-lime);
  --kong-text-primary: var(--kong-white);
  --kong-text-secondary: var(--kong-bay);
  --kong-text-on-light: #35363A;
  --kong-text-on-dark: #F7F9FC;
}
```

---

## Typography

### Typefaces

| Typeface | Role | Weights | Source |
|----------|------|---------|--------|
| **Funnel Sans** | Primary — headings and body text | Light, Italic, Extra Bold | Google Fonts |
| **Roboto Mono** | Code and technical content | Regular, Bold | Google Fonts |
| **Space Grotesk** | Buttons and UI labels | Regular | Google Fonts |

### Type Hierarchy

| Level | Font | Weight | Size/Leading |
|-------|------|--------|-------------|
| Heading XL | Funnel Sans | Bold | 72px / 78px |
| Heading L | Funnel Sans | Bold | 32px / 38px |
| Body L | Funnel Sans | Regular | 20px / 28px |
| Body L (emphasis) | Funnel Sans | Bold | 14px / 16px |
| Button | Space Grotesk | Regular | — |
| Code | Roboto Mono | Regular / Bold | — |

### CSS Font Stack (recommended)

```css
:root {
  --kong-font-primary: 'Funnel Sans', sans-serif;
  --kong-font-code: 'Roboto Mono', monospace;
  --kong-font-button: 'Space Grotesk', sans-serif;
}
```

### Google Fonts Import

```css
@import url('https://fonts.googleapis.com/css2?family=Funnel+Sans:ital,wght@0,300;0,800;1,300&family=Roboto+Mono:wght@400;700&family=Space+Grotesk&display=swap');
```

---

## Product Names

Always use the exact product name formatting below. "Kong" is always included as a prefix.

| Correct Name | Common Mistakes to Avoid |
|---|---|
| **Kong Konnect** | "Kong Connect", "Konnect" (without Kong) |
| **Kong AI Gateway** | "AI Gateway" (without Kong) |
| **Kong Gateway** | "Kong API Gateway" (old name), "Gateway" alone |
| **Kong Event Gateway** | "Event Gateway" alone |
| **Kong Mesh** | "Mesh" alone |
| **Kong Ingress Controller** | "KIC" in external content |
| **Kong Plugins** | "Plugins" alone |
| **Kong Manager** | "Manager" alone |
| **Kong Operator** | "Operator" alone |

### Product Logo Format
Product names are rendered as: **Kong** [Product Name] — where "Kong" uses the bold logotype weight and the product name uses a lighter weight.

---

## Graphic Style

### Blueprint Guides
The blueprint graphic guides — composed of lines, grids, and cross intersections — draw from architectural drafting systems. They represent construction, precision, and intentional design. Elements include:
- **Glow:** Subtle light emanation at intersections
- **Cross:** Full cross-hair intersections
- **Tee:** T-shaped intersections
- **Grid:** Underlying grid structure

### Connectivity Layers
3D ribbon/helix forms that visualize how individual elements operate together as a cohesive system. Composed of sequential forms arranged in fluid rhythm, they express harmony through structure.

### Design Approach
- Dark-dominant aesthetic (Dark Green `#000F06` backgrounds)
- Electric Lime `#CCFF00` as the primary accent and highlight color
- Blueprint grid lines and cross markers as decorative elements
- Connectivity layer imagery for hero sections and backgrounds
- Clean, architectural layout with structured grid systems

---

## Trademark

The Kong trademark includes the Kong name and logo, and any word, tagline, phrase, image, or other designation that identifies any Kong products. Rules:
- Do not modify trademarks or use them in an altered way
- Do not suggest sponsorship or endorsement by Kong
- Do not confuse Kong with another brand
- Contact the Marketing Design team for any intended use not covered by these guidelines
