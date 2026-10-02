# FOODTEX final visual / UX pass

Scope: current v18, preserving the established art direction and actual content. This is the final presentation frontend; admin and inquiry persistence are still explicitly local demos.

## Classification before edits

| Module | Grade | Decision |
|---|---|---|
| Hero, solutions explorer, Carnave preview, contact hero | A | Preserve; only responsive/performance fixes |
| Brand band, process desktop, footer, about desktop narrative | B | Calm brand strip, refine labels; use normal photo/text sequencing on mobile |
| Home institutional and news cards | C | Editorial global/local scene and brand journal |
| Product listing | B | Keep neutral contrast; horizontal filters and restrained editorial size variation |
| Product detail | C/D | Repeated H1/title and delayed CTA; single-title product composition, technical content below |
| News listing and article | C | Journal layout, category filtering, reading width, preserve portrait/video ratios |
| Quote request | C | B2B request, quantities/notes, retain WhatsApp and local demo |
| Contact form states, mobile menu, 404 | C | Intent, visible errors/success, accessible menu, authored empty/error states |
| Admin dashboard, editors and preview | B | Preserve editing; polish tokens/table containment only |

Audit evidence: source read for every public route and admin workflow; browser reviewed product detail, news listing, article, quote, about and admin before changes. Existing audit from explorer iteration includes home, catalogue, contact, tablet and mobile. Reference Allia was inspected in prior art-direction pass; its identity is not copied.

## Constraints

No fabricated dates, metrics, projects or product data. No new backend or authentication claim. Preserve official logo, real catalogues, current hero and Carnave source. No ornamental sliders or hijacked page scrolling. Product surfaces remain neutral as requested previously.

## Validation of v19 and final corrections

- Isolated render and interaction checks passed for 35 routes and 184 image references: one H1, catalogue empty state, category filtering, quantities and notes encoded in WhatsApp, invalid email and local success states.
- Browser DOM checks on nine public routes at 320, 360, 375, 390, 430, 768, 1024, 1280, 1440, 1600 and 1920 px passed after waiting for actual render: no document horizontal overflow, no measured heading/paragraph horizontal clipping, one main H1. This is geometry validation, not a device-lab certification.
- Visual inspection covered desktop hero, explorer, Carnave, institutional scene, journal, product technical details, quotation and case article; mobile preview covered hero, explorer, menu, catalogue, journal, about introduction and 320 px contact.
- Browser interactions verified direct solution selection, menu Escape with aria-expanded reset, invalid contact submission, product-to-quotation navigation, quantity/note WhatsApp encoding and news category controls. No WhatsApp message was sent. No application-origin console errors were observed.
- Two final CSS corrections: preserve dark active-filter contrast over older mobile rules and hide the duplicate mobile PDF link on desktop.
- Reduced-motion styles and motion guards are retained. Images have known dimensions and responsive WebP variants; decorative case video loads only on eligible desktop interaction. No Lighthouse or field Core Web Vitals benchmark was run, and real-device touch/performance checks remain useful before production.
- The Carnave original is a 540 × 960 portrait film. Its composition is retained within a panoramic case-study frame rather than being stretched or heavily cropped into a hero background. The current hero art direction is preserved.
- Admin and form persistence remain local demonstrations, explicitly labelled. Production backend, authenticated admin and actual form delivery are outside this presentation iteration.
