# Design system & Figma

## Files
| What | Figma file | Key |
|---|---|---|
| Design System WEB 2.0 (library) | Design-System-WEB-2.0 | `TYJ2jXpMeucSOqeGNmhjMX` |
| Oferta 2026 (offer / pricing for parents) | RAW \| Oferta 2026 | `9BxxFK7x8eAGfGEokS4VEH` |

Oferta 2026 landmarks (may move — re-read before editing): page "👨‍👩‍👦 Parent Offer" (`2361:26690`), section "parent offer", master frame `2464:51900` "1366 Offer Parents – final 01"; responsive frames to its right. Page "🎓 Student Offer" (`2561:40005`), section "student offer": `2561:40006` "1366 | Offer Students — v1 (review)" (one page for SP + szkoła średnia, no Rodzic/Uczeń switch; "Kup albo poproś rodzica"), local 🆕 `Ask Parent Card / Share link` `2561:42692`. Earlier pages "Oferta Rodzic", sections "finals" / "semi-final".
Page "👨‍👩‍👦 Parent Offer final", section "parent offer" (`2626:40197`): local component set `🆕 Paywall` (`2646:47530`, 2026-10-19) with `Size=800+` (1366/1024/800, two columns) · `600+` (stacked, plans in a row) · `320+` (360/320, stacked, plans as a list, padding 16). Built from the frame "Paywall - main component/600+" (`2643:49978`); the page frames still use detached copies, not instances. Local components for this page also sit in section "🧩 Responsive components" (`2626:44843`): Feature Tile, Sticky CTA, Step Toggle, Segmented Control.

DS WEB 2.0 conventions for new components (designer, 2026-10-19; see page "Modular Components - Landing" `16056:20149`): each component gets a "DS Card - <Name>" frame (Inside Title bar card with Specification / Menu / Overview links; sections "Component variants - for use", "Semi components - don't use", "Opis"), **its own spec page named after the component** (e.g. page "Segmented Control" `16064:25572`, page "Feature Tiles" `16077:174465`, each holding "DS Card - spec"), a box in "Overview - Modular Components - Landings" (`16057:20398`, Specification + Component links) and a link in the "Inside - DS Card - Menu" main component (`2264:34732`, section "MC - Landing"). **Every gap, padding and radius must be bound to a token** (e.g. Spacing/static/space-4…16, Spacing (Layout)/*, Radius/static/*); no raw values. Use as few Size variants as possible and let width be Fill: one variant per layout change, named by its lowest breakpoint (1024+ covers 1024 and 1366, 600+ covers 600 and 800, 320+ covers 360 and 320).
Landing components in the DS (2026-10-19): Segmented Control; **Feature Tiles** (`16069:173881`, Size=1024+ 4 in a row · 600+ 2×2 · 320+ full-bleed carousel with Stepper (gap space-12); tiles Fill with equal row height; every size and row hugs its height, never a fixed height on containers that clip) built on semi component **Feature Tile** (`16069:11157`, Feature=Success/Tertiary/Warning/Primary (colour names) × State=Default/Hover; copy uses hard spaces after one-letter words and in "krok po kroku"). Card `16069:173882`, spec `16072:173850`. Not yet published to the library; the Oferta page frames still use detached tiles (800 there is still 4 in a row, the DS now says 2×2).

Which DS applies where (designer, 2026-10-11):
- **odrabiamy.pl** → mostly DS WEB 2.0.
- **iOS / Android apps** → a **separate app design system** Figma file (key unknown, ask for the link). Don't apply WEB 2.0 components to app screens.
- **Satellites** → DS WEB 2.0 is attached but not used consistently. Expect drift; flag it, don't assume components match.
- **Odrabiak illustrations** → in Figma (link pending), 3D style.

Figma org: MAKALU MEDIA. The Figma connector must be signed in as the **work** account (anastasiaplytka@odrabiamy.pl), not a personal Gmail — check with `whoami` if you get "no edit access".

## Foundations (Design System WEB 2.0)
- Font: **Noto Sans** (+ Noto Sans Mono). Load all weights before editing text.
- Text styles: `Hedline/H1–H6` (the DS spelling is "Hedline"), `Subtitle-1/2`, `Body/Large|Medium`, `Label/*`, `Caption/Small`. Hero steps H1 48 → H2 40 → H3 34 → H4 28 across breakpoints.
- Colour variables (selection):
  - Primary `#4f4fee`, primary-text `#423dd1`
  - Text/text-primary `#313859`, secondary `#4c547b`, tertiary `#5d658e`
  - Outlines `#d6d9e5` / `#ecedf3`
  - Surface/surface-1 `#fcfcfd`
  - Tertiary `#9945a1`, green ≈ `#37B992`
  - Known issue: success icon `#70d2b4` fails contrast (proposed `#12866a`).
- Collections: Colors, **Units** (modes Desktop / Tablet / Mobile; e.g. `Spacing (Layout)/horizontal/main-margin`), Spacing/*, Radius/* (4–24), shadow `shadow/01px`.

## Components (known)
Main Button (40px tall — below 44px touch target, flag it; max width 448px, not overridable in instances; width rule (designer, 2026-10-13): **Fill only on mobile (360/320), Hug on tablet (800/600)**), Bullet Point, Tag, Chip, Price Tag (RAW), Summary line – semi, Accordion, Segmented Control, Carousel, Opinion, Top Bar Menu (sizes 1366+/1024+/800+/600+/320+), Footer (800+/600+/320+), Icons/18/*.
The Rodzic/Uczeń switch on Oferta is currently hand-built, not a DS component.

## Breakpoints
1366 (desktop master) → 1024 → 800 → 600 → 360 → 320. Side padding ≈ 40 / 40 / 32 / 24 / 16 / 16. Fold checks: 1366×768, 360×800.

## Topic colours used on Oferta tiles
green = rozwiązania krok po kroku · purple = Odrabiak Pro · orange = kursy wideo · blue = wyniki.
