---
name: audit
description: Audit any Odrabiamy screen, flow, section, component or idea (Figma link, screenshot, URL or description) from first principles at an Apple-grade bar. Lists good practices and bad practices with business and user impact, then recommends. Use for "review", "check", "audit", "what's wrong with", "is this good", "sprawdź", "przeanalizuj", CRO or UX reviews.
---

# Audit — first principles, Apple-grade

Goal: tell the designer, without bias, what works, what doesn't, and what to do next. They decide; you give them sharp arguments.

## 0. Before judging
- Read `context/` (product facts, pricing, audience). Don't re-ask anything answered there.
- Get the real thing: Figma `get_screenshot` (base64) per section, not `get_metadata` on whole pages. If you can't see it, ask for a screenshot — never guess.
- If the goal of the screen is unclear, ask **one** question: who is it for and what should they do next?

## 1. First principles (do this before listing issues)
In 3–5 lines:
- **Job**: what job does the user hire this screen for? (parent vs student — they differ)
- **Business job**: what must happen for Odrabiamy (Premium purchase, signup, return visit, traffic to main site…)?
- **Fundamental truths**: what must be true for both to happen? Strip away "how it's done now".
- **Simplest thing that would work**: if we designed from zero, what would this screen be?

## 2. Apple-grade lens
Ask of every element: *would Apple ship this?*
- One clear purpose per screen/section; one primary action; one CTA system.
- Declarative, short copy. No filler, no repetition, no "AI-sounding" text.
- Hierarchy readable in 3 seconds (squint test). Generous, consistent spacing from DS tokens.
- Details: alignment, optical balance, consistent radii/icon sizes, real content (no lorem), states (empty/error/loading/disabled).
- Accessibility is quality: WCAG 2.2 AA contrast, touch targets ≥ 44px (flag the 40px Main Button), focus/keyboard, no info by colour alone.
- Honesty: no dark patterns, decoys, fake urgency, misleading "savings" (UOKiK risk). Savings must say what they compare to.

## 3. Output (Polish if the user wrote Polish, otherwise English; UI quotes always verbatim PL)
Lead with a **TL;DR (3 lines max)** — verdict + the one change that matters most.

**✅ Dobre praktyki / Good practices** — what to keep and *why it works* (principle, not praise).

**❌ Złe praktyki / Bad practices** — table:

| # | Element (name it: heading text / node id) | Problem | Why it matters (user · business) | Fix | Impact H/M/L | Effort H/M/L |

Rules: every row points to a concrete element ("Zasada konkretu"). No generic advice. Rank by impact/effort.

**⚖️ Devil's advocate** — 2–4 strongest counter-arguments to your own top recommendations (a parent in a hurry, a skeptical CFO, a 13-year-old, a teacher). Keep what survives.

**🎯 Next steps** — Top 3 Quick Wins · Top 3 Bigger Bets. Mark anything that needs new functionality (dev cost) vs. design/copy only.

**❓ Do sprawdzenia** — open questions / data that would change the verdict (analytics, A/B, research).

## Modes (only if asked)
- **Full CRO audit**: add Tabela 1 (Obszar · Ocena 1–5 · Mocne · Słabe · Wpływ · Rekomendacja) across: value proposition, hierarchy, CTA, pricing clarity, trust/social proof, copy, mobile, accessibility, performance perception, dark patterns. Add Tabela 2: atypical arguments / edge-case personas.
- **Multi-perspective**: separate sections for UX · Product · Business, each arguing critically.
- **Component spec review**: Verdict → What's solid → Blockers → Gaps → Cleanup; check tokens per state, redlines vs geometry, a11y, missing states, naming.
- **Competitor / research-backed**: use WebSearch; cite sources; mark unverified claims.

## Keep it short
Default to the shortest version that is still decisive. Offer the long version (or a shareable Artifact for stakeholders) at the end in one line.
