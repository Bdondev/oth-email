# Section QA: Upcoming Jordan Drops

Status: **NEEDS ASSETS / URL APPROVAL**

## Implemented

- Live `UPCOMING JORDAN DROPS` heading and release timing copy.
- Five live product names in a two-column / single-item / two-column layout.
- Responsive MJML structure that stacks columns on narrow screens.
- Live `SEE UPCOMING RELEASES` CTA with a temporary `#` href.
- The first product card now uses the supplied Jordan product image.
- The second product card now uses the supplied Air Jordan 9 image and live `Air Jordan 9` copy.
- The third product card now uses the supplied Air Jordan 12 Retro “Idols Become Rivals” image and live copy.
- The fourth product card now uses the supplied Air Jordan 5 Retro “Halloween” image and live copy.
- The fifth product card now uses the supplied Air Jordan 8 Retro “Chrome” image and live copy.

## Evidence

- `npm run validate` — passed.
- `npm run build` — passed.
- `npm run visual-qa` — passed at 320px, 390px, 600px and 1440px.
- Browser QA found no horizontal overflow, unloaded images or missing alt text.
- Compiled HTML: 24,445 bytes.

## Remaining blockers

- The Air Jordan 9 colorway/product copy needs approval if a more specific label is required.
- The release-calendar CTA destination is not approved; `#` is a placeholder.
- Browser screenshots do not validate Gmail, Apple Mail, Outlook, dark mode or ESP processing.

