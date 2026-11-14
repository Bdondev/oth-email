# Email development rules

These rules apply to the marketing email in this repository.

## Project shape

- The source of truth is `src/email.mjml`.
- Reusable sections live under `src/sections/`.
- Shared MJML tokens and styles live in `src/styles/design-system.mjml`.
- Supplied assets live under `assets/source/`; processed assets belong under `assets/optimized/`.
- Campaign evidence, design decisions and QA reports live under `docs/`.
- `dist/` is generated preview output and is ignored by Git.

## Email rules

- Keep important copy, offers, legal text, unsubscribe content and CTA destinations as live HTML; never invent missing values.
- Use MJML and presentation-table HTML with inline critical styles and selective media queries.
- Avoid CSS Grid, Flexbox, absolute positioning and runtime JavaScript for email layout.
- Preserve logical reading order and use presentational table semantics in compiled output where supported.
- Give informative images meaningful alt text; use empty alt text for decorative images.
- Local asset paths are valid for repository previews only. Production and ESP handoff require absolute HTTPS or ESP-hosted image URLs.
- Keep the shared design tokens centralized in `src/styles/design-system.mjml`.

## Workflow

- Build one named section at a time after reviewing the relevant design and asset documentation.
- Preserve supplied source assets and existing project conventions.
- Run `npm run validate` and `npm run build` before visual QA.
- Run `npm run visual-qa` at 320px, 390px, 600px and 1440px.
- Browser screenshots do not prove Gmail, Apple Mail, Outlook, dark-mode or ESP compatibility.
- Before release, check images-off behavior, dark mode, Gmail clipping risk, Outlook fallbacks, CTA links and legal fields.
- Do not send, deploy, upload or commit without explicit approval.

## Required references

Before implementing a section, review:

- `docs/CAMPAIGN_BRIEF.md`
- `docs/DESIGN_SPEC.md`
- `docs/DESIGN_SYSTEM.md`
- `docs/ASSET_MANIFEST.csv`
- `docs/SECTION_BUILD_PLAN.md`
- `docs/ACCEPTANCE_CRITERIA.md`

When a production input is missing, document the blocker and keep a clear placeholder. Do not fabricate copy, URLs, assets, legal text, ESP syntax or client-test results.
