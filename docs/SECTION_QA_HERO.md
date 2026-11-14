# Hero section QA

Section: Header + hero
Reference: `screenshots/Screenshot_20260929_005728_Chrome.jpg`
Source: `src/sections/hero.mjml`
Assets: `assets/source/off-the-hook-logo.png`, `assets/source/hero.png`

## Build evidence

- [x] Scope limited to the header + hero section.
- [x] MJML compiled with `npm run build`.
- [x] Asset audit completed in `docs/ASSET_AUDIT.md`.
- [x] Static email audit completed with 0 non-hosting errors.
- [ ] Browser screenshots inspected at 320px, 390px, 600px and 1440px.
- [ ] Final image hosting URLs supplied and verified.
- [ ] Real inbox rendering tested.

## Observed deviations and risks

- The screenshot is a mobile reference; desktop behavior is proposed, not measured.
- The logo and banner are currently local asset paths. They will not be deliverable in a sent email until replaced with HTTPS or ESP-hosted URLs.
- The static audit reports no links, preheader, unsubscribe link or postal address because those belong to later sections and ESP configuration.
- The hero uses live text for the headline and a separate image for the banner, preserving readable content when images are blocked.

## Status

Built; needs browser and real-client QA before release.
