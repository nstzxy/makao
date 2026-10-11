# Design system & Figma

## Files
| What | Figma file | Key |
|---|---|---|
| Design System WEB 2.0 (library) | Design-System-WEB-2.0 | `TYJ2jXpMeucSOqeGNmhjMX` |
| Oferta 2026 (offer / pricing for parents) | RAW \| Oferta 2026 | `9BxxFK7x8eAGfGEokS4VEH` |

Oferta 2026 landmarks (may move — re-read before editing): page "1366", master frame `2464:51900` "1366 Offer Parents – final 01"; responsive frames to its right; earlier pages "Oferta Rodzic", sections "finals" / "semi-final".

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
Main Button (40px tall — below 44px touch target, flag it), Bullet Point, Tag, Chip, Price Tag (RAW), Summary line – semi, Accordion, Segmented Control, Carousel, Opinion, Top Bar Menu (sizes 1366+/1024+/800+/600+/320+), Footer (800+/600+/320+), Icons/18/*.
The Rodzic/Uczeń switch on Oferta is currently hand-built, not a DS component.

## Breakpoints
1366 (desktop master) → 1024 → 800 → 600 → 360 → 320. Side padding ≈ 40 / 40 / 32 / 24 / 16 / 16. Fold checks: 1366×768, 360×800.

## Topic colours used on Oferta tiles
green = rozwiązania krok po kroku · purple = Odrabiak Pro · orange = kursy wideo · blue = wyniki.
