# Akshay Portfolio Design System

Slug: akshay-editorial
Version: 1.0

## Direction

A polished, minimalist portfolio for a full-stack developer: editorial clarity with a quiet technical edge. The visual language should feel intentional, confident, and human—not like a generic developer template and not like a loud terminal simulator.

## Foundations

### Color tokens

- Canvas: #F5F3EE — warm paper background
- Surface: #FCFBF8 — elevated cards and navigation
- Ink: #171717 — primary text and headings
- Ink-muted: #6E6B66 — secondary text
- Line: #D9D5CC — dividers and borders
- Accent: #D94F35 — action color, active states, small highlights
- Accent-soft: #F1D6CF — subtle accent fills
- Dark panel: #202222 — code and capability panel
- Dark text: #F5F3EE — text on dark panel
- Success: #437A5B — availability/status indicator

Do not introduce additional colors without updating this list. Use accent sparingly: links, buttons, status, and a few project signals.

### Typography

- Display / headings: Space Grotesk, system fallback; weight 500–600; tight tracking (-0.04em)
- Body: Inter, system fallback; weight 400–500; comfortable line-height 1.6
- Technical labels: IBM Plex Mono, monospace fallback; 11–13px; uppercase or code-like syntax
- Type scale: 12, 14, 16, 20, 28, 40, 64px with responsive clamp for display sizes

### Layout

- Max content width: 1180px
- Reading measure: 660px
- Page gutters: 24px mobile, 40px tablet, 64px desktop
- Section spacing: 128px desktop, 88px tablet, 72px mobile
- Grid: 12 columns desktop, 6 tablet, single column mobile
- Dividers are 1px and full-bleed within the content rail

### Shape and depth

- Radius: 0px for structural sections, 2px for controls, 6px only for media or tags
- Shadows: none by default; use a soft 0 12px 30px rgba(23,23,23,.08) only for floating interactions
- Prefer borders, whitespace, and alignment over cards with heavy elevation

## Components

### Navigation

A compact top rail with monogram/name on the left and text links on the right. Sticky only on desktop if it does not obscure content. Active/hover states use accent underline or color, never filled pills.

### Hero

Eyebrow, one decisive two-line statement, supporting paragraph, and two actions. Include availability as a small status line. Use generous top padding and avoid a hero illustration competing with the name.

### Section header

Monospace index (01, 02, 03), serif-free section title, and a one-line description. Keep the header aligned to the main content grid.

### Project row

A horizontal editorial row with project number, title, one-sentence outcome, technology tags, and an external link. On hover, reveal accent line and a subtle image tint. On mobile, stack content while preserving the number/title hierarchy.

### Experience row

Use a clean timeline/list treatment: role and company at left, dates at right, concise contribution below. Do not use dense boxed cards.

### Capability panel

Dark panel with a short statement and grouped technical skills. Syntax-inspired labels may remain as a nod to the original identity, but the content must stay easy to scan.

### Buttons and links

Primary action: ink background with paper text; hover inverts to accent. Secondary action: transparent with ink border. Text links are underline-on-hover. Always provide visible keyboard focus.

## Motion

- Use 180–240ms ease-out transitions for color, transform, and opacity.
- Hover project rows translate no more than 4px.
- Respect prefers-reduced-motion and disable smooth scrolling/entrance effects there.
- No looping decorative animation.

## Accessibility

- Body text contrast must meet WCAG AA on the canvas.
- All interactive elements need visible :focus-visible treatment in accent.
- Images require meaningful alt text; decorative images use empty alt.
- Use semantic landmarks, one h1, logical heading order, and keyboard-accessible navigation.
- External links must indicate a new tab in accessible text or title.

## Content voice

Specific, concise, and outcome-led. Prefer “I build…” and measurable contribution over vague claims. Keep the personality warm and direct; avoid buzzword stacks.
