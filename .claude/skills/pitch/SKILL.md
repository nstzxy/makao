---
name: pitch
description: Turn a product or design idea for Odrabiamy into a short, decision-ready idea brief for the CEO — problem, evidence, options, recommendation, conversion impact, cost, ask. Idea first, presentation second. Use for "pitch", "idea for the CEO", "how do I sell this idea", "uzasadnij pomysł", "pomysł dla prezesa", "one-pager", "deck", "should we build X".
---

# Pitch — a sharp idea, not a pretty deck

Goal: help the designer bring the CEO **one clear idea** with enough evidence to say yes, no or "test it". The CEO cares about the idea, not the slides. Polish the thinking, not the format.

## 0. Before writing
- Read `context/` (product, pricing, priorities). **The current company priority is conversion** (free → Premium), so every idea is judged by its conversion effect first.
- If the idea's target (parent vs student), surface (web, app, satellite) or goal is unclear, ask 1–3 short questions.
- Get evidence, don't invent it: GA4 (web `260847366`, apps `442870372`; read in the built-in browser), Figma screenshots, the live site, app-store reviews, competitor pages (use the `research` skill for bigger scans). Anything unverified gets ⚠. No made-up numbers, quotes or competitor claims.

## 1. First principles (internal, 3–5 lines)
- What user problem does it solve, for whom (Rodzic płaci, Uczeń używa)?
- Why would it move conversion (or retention/traffic → conversion)? Name the mechanism.
- What's the simplest version that proves it? Prefer no-dev or small-dev versions.

## 2. Output: the idea brief (default)
Reply in the user's language; UI copy quoted in Polish. Max ~1 screen.

1. **Pomysł w jednym zdaniu**: what we change, for whom, and the expected outcome.
2. **Problem**: what's broken today, with evidence (data / screenshot / quote, each with a source).
3. **Opcje** (2–3, including "zrób nic" or the cheapest version):

   | Opcja | Co | User win | Business win (conversion) | Koszt | Ryzyko |

   Mark each "bez developmentu" / "mały development" / "wymaga developmentu".
4. **Rekomendacja**: one option and why it beats the others.
5. **Jak sprawdzimy**: the metric (GA4 event or funnel step), the baseline if known, and the test (A/B, staged rollout, before/after). If the baseline is unknown, say so.
6. **⚖️ Devil's advocate**: the 2–3 strongest objections the CEO could raise (cost, cannibalising Premium, brand, UOKiK/dark-pattern risk, app-store rules) and the honest answer to each. Drop the idea if it doesn't survive.
7. **Prośba**: exactly what we need — a decision, a test slot, dev days, data access.

## 3. Format
- Default: **in chat**. Offer a shareable version in one line.
- If the user wants something to share: a Doc artifact (same structure). Build slides (Slides artifact, max ~8: problem → evidence → options → recommendation → impact/cost → ask) **only when asked**.
- Visuals: real Figma screenshots or a `prototype` link, never mock data presented as real.

## Rules
- Never: dark patterns, fake urgency, decoys, fake savings, parent "modes", web subscriptions (see `context/company.md`).
- Separate facts, estimates and guesses explicitly. An estimate shows its math.
- Don't flatter the idea. If the evidence is thin, say "worth a test, not a build".
