# Design / implementation spec

Source reference: `screenshots/Screenshot_20260929_005728_Chrome.jpg`
Content width: approximately 600px — Proposed starting point
Mobile reference: Provided as a tall mobile screenshot; desktop reference missing
Body background: white — Observed
Brand palette: deep navy/royal blue with white and a small red accent in the footer navigation — Observed
Font stack: serif display logo plus bold sans-serif headings — Observed; exact fonts need confirmation

## Sections

| ID | Reference location | Live content | Decorative content | Layout/stacking | Outlook risk | Status |
|---|---|---|---|---|---|---|
| 01 | Header + hero | Logo text, hero heading | Jordan footwear image | Single column | Image URL and crop | In progress |
| 02 | Intro CTA | Release paragraph, `LEARN MORE` | None | Single column | Button rendering | Planned |
| 03 | Upcoming Jordan drops | Heading, date, product names, CTA | Product images | Two-column product grid, then single item | Image blocking and stacking | Planned |
| 04 | Shop Nike footwear | Heading, availability, product names, CTA | Feature/product images | Feature image, three-product row | Mobile stacking | Planned |
| 05 | Contact, loyalty and footer | Contact, navigation, address, unsubscribe | Rewards artwork/icons | Single column | ESP/legal fields | Planned |

## Mobile and fallback contract

- Mobile reading order: top to bottom in screenshot order.
- 320px minimum: no horizontal scrolling; live text and CTAs remain readable without images.
- Image blocking state: all product visuals need meaningful alt text or decorative empty alt values; production assets are currently missing.
- Dark mode: not assessed; needs target-client testing.
- Composite exports: not approved; preserve live headings, product names, CTA text and legal copy.
- Client fallback: use MJML-generated presentation tables and web-safe font fallbacks.
