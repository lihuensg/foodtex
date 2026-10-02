# Nosotros mobile correction

Observed defect: `.story-chapter` retained its desktop flex-row while mobile photos were inserted ahead of the text. Photos took full available width and the chapter copy escaped the clipped page. The prior document overflow check missed content clipped by a parent.

Correction is confined to `@media(max-width:760px)` in about-mobile.css: restore the existing changing-photo stage and four chapter buttons in a compact sticky stack; hide the duplicate chapter photos, force chapters into block flow, give text its full available width, and set scroll offsets for the compact stage. Short landscape screens use normal flow. Desktop styles, app.js, data.js, chapter content and existing motion logic are unchanged.

Checks: four chapter content bounds remain inside the viewport at 320, 360, 375, 390, 430, 768 and 1366 px; no heading/paragraph horizontal clipping or document overflow detected. Visual mobile previews inspected all five requested widths. Chapter buttons 01, 02 and 03 correctly synchronize photograph, caption, number and active state. Native PageDown moves the active index from 01 to 02. No scroll interception was added.

Screenshot: about-mobile-repaired.jpg.
