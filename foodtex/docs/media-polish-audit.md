# Scoped visual correction — FOODTEX

Scope: uniform product listing on desktop/tablet; vertical journal on mobile; media fitting and integrated technical backgrounds. Preserve hero, home solutions explorer, desktop journal composition, motion, routes and data.

Causes: product-featured span 2 + 380/420 px imagery versus 310/350 px ordinary cards. Mobile journal sidebar still used a title/image two-column grid with 65–90 px thumbnails and contain letterboxing.

Changes: equal columns (2 tablet, 3 desktop, 4 wide desktop), intrinsic 4:3 media and equal flexible rows, CTA anchored below content, minimum two-line title space and up to three summary lines. Technical pictures remain contain on transparent integrated media. Editorial thumbnails cover; mobile journal image/category/title/action stack. Article photos use their intrinsic ratio without coloured letterbox. Logos and case video remain contained.

No JavaScript, route, product/news content, interaction or data changes.

Validation: 12 product cards measured at 1280, 1366, 1440, 1920 and 768 px: equal row/card heights and media ratio, CTA offset matching within subpixel rounding, no document overflow. Found and corrected the old first-card metadata margin (2 px discrepancy).

25 mobile route/width combinations (430, 390, 375, 360, 320; home, products, product detail, news, video article) passed overflow and heading/paragraph horizontal clipping checks. Journal secondary images span the full card and titles occur below imagery. Visual checks inspected secondary news cards at all five sizes and product listing/detail at notebook.

Existing isolated checks still pass for 35 routes, 184 asset references, filters/empty state, categories, quote encoding and form states. Source app.js and data.js are untouched.

Final published checks and screenshots follow in this report.

Final v23 measurements at all four desktop widths: 12 cards, width/height/title/description/CTA spread below 0.02 CSS px (subpixel rounding), media ratio 4:3, zero document overflow. Visual previews inspected all four widths. White studio backgrounds now blend at the card boundary, including existing hover compositing.

Article portrait photos keep the previous 650 px maximum scale to avoid a new giant image; transparent surrounding background removes visible letterboxing without cutting event/poster information. Case videos remain unchanged.
