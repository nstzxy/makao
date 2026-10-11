---
name: copy-pl
description: Write, shorten or review Polish UI and marketing copy for any Odrabiamy product — short, engaging, consistent across the whole product, with correct Polish typography. Always says whether each line targets parents or students and argues for the choice. Use for "write copy", "shorten text", "rewrite", "headline", "CTA", "skróć tekst", "napisz", "popraw copy", microcopy, error/empty states.
---

# Copy PL — krótko, ciepło, spójnie

Goal: copy that a parent or a student understands in one glance and wants to act on — consistent in voice across odrabiamy.pl, the apps and all satellite products.

## 1. Pick the audience first (and say so)
For every piece of copy, state the target and **argue it in one line** so the designer can decide:

| | **Rodzic** (płaci) | **Uczeń** (używa) |
|---|---|---|
| Motywacja | spokój, wsparcie dziecka, oszczędność czasu i pieniędzy, uczciwość | szybciej odrobić, zrozumieć, lepsza ocena, mniej stresu |
| Ton | ciepły, rzeczowy, partnerski | luźny, energiczny, konkretny, bez infantylizmu |
| Forma | „Ty", bez oceniania | „Ty", krótkie zdania |
| Unikaj | obwiniania („nie dajesz rady"), straszenia, emocjonalnych awantur | moralizowania, „ściągania" jako obietnicy, slangu na siłę |

Default: landing/pricing/payment → **Rodzic**; in-product (solutions, Odrabiak Pro, fiszki, arkusze) → **Uczeń**. If a line could serve both, give both versions side by side.

## 2. Voice rules (both audiences)
- **Krótko.** One idea per sentence. Headline ≤ 6–8 words, subline ≤ 15–20 words, CTA 1–3 words (czasownik: „Wybierz plan", „Sprawdź rozwiązanie").
- **Konkret zamiast obietnic** — numbers, real features, real outcomes. No invented stats or testimonials.
- **Ciepło, bez winy.** Never imply a parent is failing or a student is lazy. Positive framing over pain.
- **Uczciwie.** No fake urgency or misleading discounts; savings say what they compare to („o 339 zł taniej niż 12 × 49 zł").
- **Nie jak AI.** No "Odkryj…", "Rewolucyjny…", "W dzisiejszym świecie…", triplets of adjectives, em-dash chains, emojis everywhere.
- **Spójnie.** Use the glossary below; same thing = same word everywhere.

## 3. Glossary (keep consistent)
- Odrabiamy (brand) · Premium · Odrabiak Pro · Kursy wideo · rozwiązania krok po kroku
- Plan names: Miesiąc · 3 miesiące · Rok
- Prices: „49 zł", „249 zł / rok", „ok. 21 zł / mies." (non-breaking space before „zł")
- Prefer „uczeń" / „dziecko" consistently within a screen; don't mix.
(Extend this list as decisions are made — ask the designer before introducing a new term.)

## 4. Polish typography
- Quotes „…" (and ‚…' nested), not "…".
- Spaced en dash „ – " in sentences; unspaced en dash in ranges: „1–8", „7–19 lat".
- Non-breaking space after single-letter words (a, i, o, u, w, z) and between number and unit („249 zł", „14 dni").
- Sentence case for headings and buttons. No trailing period in headlines/CTAs.
- Numbers: „1 000" (thin space) from 5 digits on; decimals with comma „20,75 zł".
- Check diacritics and common typos (ą ę ś ć ż ź ń ó ł).

## 5. Output format
For each text element:

| Element (node id / heading) | Było | Propozycja | Grupa (Rodzic/Uczeń) | Dlaczego (1 line) |

Then: 2–3 alternative versions for the key line (headline or CTA) in different angles (np. rzeczowy · ciepły · odważny). Mark the one you recommend.

When working in Figma: duplicate to the right (see `figma-variants`), swap text in place to keep text styles/bindings, and add a Dev Mode annotation „Było: …" on every changed text node.
