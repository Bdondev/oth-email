# Off The Hook email design system

This system records the reusable visual rules for the email campaign. Values marked **Observed** come from the supplied screenshot. Values marked **Proposed** are implementation defaults and need confirmation against final brand guidelines or an approved desktop design.

## Color tokens

| Token | Value | Status | Use |
|---|---|---|---|
| `color.brand` | `#003b7a` | Observed | Headings, body copy, logo treatment and primary CTAs |
| `color.accent` | `#1175b9` | Observed | Thin top border and blue accent details |
| `color.accent-red` | `#b12c1e` | Observed | Sale/navigation emphasis where present |
| `color.surface` | `#ffffff` | Observed | Email canvas and content sections |
| `color.outer-background` | `#f5f5f0` | Proposed | Desktop side gutters outside the centered email |
| `color.text-on-brand` | `#ffffff` | Proposed | Text on blue buttons or banners |

## Typography

| Role | Rule | Status |
|---|---|---|
| Brand mark | Supplied transparent logo image; display at approximately 360px wide | Observed / Proposed display size |
| Display heading | Arial/Helvetica fallback, bold, approximately 56px, 1.08 line-height | Observed / Proposed fallback |
| Body copy | Arial/Helvetica, 16px, 1.35 line-height | Proposed |
| CTA label | Arial/Helvetica, bold, 20px | Proposed |

No web font is required. Web-safe fallbacks are intentional for email-client compatibility.

## Layout and spacing

| Token | Value | Status | Use |
|---|---:|---|---|
| `layout.wrapper` | `600px` | Proposed | Desktop email container |
| `space.section-top` | `72px` | Observed / Proposed | Hero top spacing |
| `space.logo-bottom` | `88px` | Observed / Proposed | Logo to hero heading |
| `space.heading-bottom` | `64px` | Observed / Proposed | Hero heading to banner |
| `space.mobile-gutter` | `24px` | Proposed | Small-screen horizontal padding |
| `image.hero-display` | `504px` | Proposed | Hero banner display width |

## Email implementation rules

- Keep headings, body copy, CTA labels and legal text as live HTML.
- Use separate image assets for the logo and product photography.
- Use MJML-generated presentation tables; avoid grid, flexbox and essential absolute positioning.
- Use local asset paths only for preview. Final sends require HTTPS or ESP-hosted image URLs.
- Keep all new sections aligned to these tokens and update this document when a token changes.
- Test at 320px, 390px, 600px and 1440px before client QA.

## Source of truth

- Reference screenshot: `screenshots/Screenshot_20260929_005728_Chrome.jpg`
- MJML tokens: `src/styles/design-system.mjml`
- Section source: `src/sections/`
