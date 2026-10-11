---
name: prototype
description: Turn a Figma frame, flow or idea for Odrabiamy into a shareable, clickable HTML prototype published as an Artifact — real content only, DS WEB 2.0 tokens, responsive. Use for "prototype", "make it clickable", "live version", "share a link", "zrób prototyp", "klikalny prototyp", "pokaż to na żywo".
---

# Prototype — a live page people can click

Goal: a single-page HTML prototype that looks and behaves like the real product closely enough for a CEO, PO or a test user to react to the idea, not to the fidelity gaps.

## 0. Before building
- Read `context/`. Ask 1–3 questions if unclear: which frame(s), which breakpoints, what must be clickable, who will see it (internal vs test users).
- Source of truth is Figma: `get_screenshot` per section (plain `123:456` ids) and `get_design_context` / `get_variable_defs` for exact tokens and copy. Re-read nodes each time; the designer edits live.
- Pick the right DS: **odrabiamy.pl and satellites → DS WEB 2.0**; **app screens → the separate app DS** (ask for the file if it isn't in `context/design-system.md`).
- Load `artifact-design` before writing the page.

## 1. Build rules
- **One HTML file**, published with the Artifact tool (scratchpad, never this repo). Update the same file for new versions so the link stays.
- **Tokens:** Noto Sans (Google Fonts, all used weights), primary `#4f4fee`, text `#313859`, plus the rest from `context/design-system.md` as CSS variables. No off-brand fonts or colours.
- **Real content only:** copy, prices (49 / 99 / 249 zł), features and images from Figma or the live site. No lorem, no invented testimonials, numbers or features. A missing asset gets a neutral labelled placeholder.
- **Responsive:** 1366 and 360 at least (DS breakpoints 1366 → 1024 → 800 → 600 → 360 → 320; side padding 40 → 16). No horizontal scroll.
- **Interactions:** only what the idea needs (switch Rodzic/Uczeń, select a plan, open an accordion, go to the next step). Dead ends show a short "W prototypie niedostępne" note, never a broken link. Payments and logins are faked, with no real form submission.
- **Accessibility:** WCAG 2.2 AA contrast, focus states, touch targets ≥ 44px, semantic HTML.
- **Honesty:** anything the product doesn't do today gets a small "wymaga developmentu" tag (hidden with `?clean=1` for clean demos).

## 2. Verify
Open the artifact, check 1366 and 360, click every interactive element, and compare against the Figma screenshot. Fix differences before sharing.

## 3. Reply
TL;DR + link, what's clickable, what's faked or simplified, differences from Figma and why. Offer variants (A/B toggle via `?v=b`) in one line if useful.
