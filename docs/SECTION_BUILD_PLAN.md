# Section-by-section implementation plan

Reference: `screenshots/Screenshot_20260929_005728_Chrome.jpg`
Chosen stack: MJML
Target desktop wrapper: approximately 600px — proposed
Target mobile widths: 320px and 390px
Target inboxes: Needs confirmation

| Order | Section | Approved source/copy | Asset decision | HTML structure | Mobile behavior | Outlook/fallback risk | Progress |
|---|---|---|---|---|---|---|---|
| 01 | Header + hero | Screenshot-observed logo and heading; local source assets supplied | Separate logo and hero photo | `src/sections/hero.mjml` | Single column | Local image paths; hosted URLs required | Built — visual QA pending |
| 02 | Intro CTA | Screenshot-observed paragraph and `LEARN MORE`; URL missing | Live HTML | Text + MJML button | Single column | Placeholder URL; button click area | Built — visual QA pending |
| 03 | Upcoming Jordan drops | Product names observed; links and image assets missing | Separate product images | Reusable product cells | Two columns stack on mobile | Image blocking | Built — product images and URL pending |
| 04 | Shop Nike footwear | Headings and product names observed; links and assets missing | Feature photo + product images | Feature image + product row | Product row stacks | Width/crop differences | Not started |
| 05 | Contact, rewards and footer | Footer copy observed; ESP fields need approval | Rewards artwork/icons missing | Live footer/legal modules | Single column | ESP merge syntax | Not started |

## Stop rule

Implement one named section at a time. After each section, run `npm run build`, validate the compiled HTML, inspect 320/390/600px views where tooling is available, record deviations, and avoid changing completed sections.
