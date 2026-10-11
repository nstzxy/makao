---
name: figma-variants
description: Explore and design the best solution to a problem directly in Figma — build one or more variants as new frames to the RIGHT of the existing frame, using Design System WEB 2.0 components and tokens, and proposing brand-new components when the DS lacks one (marked as "NEW"). Use for "make variants", "propose a better version", "redesign this section", "zrób warianty", "zaproponuj", "v2/v3 next to it", "how could this be better".
---

# Figma variants — find the best solution

Goal: give the designer **real, comparable options** in Figma that solve the problem better for **both the user and the business**. Not cosmetic reshuffles.

## Hard rules
1. **Never touch the original.** Duplicate or build new frames placed to the **right** of the source frame (same page/section, aligned top, 200px gap; further variants continue right). If the user edits the file between turns, re-read the current node first.
2. **Design system first.** Load `figma:figma-use` before any `use_figma`. Use `search_design_system` (one query per call) and existing **instances** of Design System WEB 2.0 components; bind colours/spacing/radius to variables and text to DS text styles (note: styles are spelled "Hedline/…"). Don't detach instances. Preload all Noto Sans weights before editing text.
3. **New components are allowed — and welcome when they solve the problem better.** Build them locally in the working file (not in the DS library), still built from DS tokens, and mark each one:
   - name prefix `🆕 ` (e.g. `🆕 Plan Picker / Compact`)
   - a Figma comment / Dev Mode annotation: "NOWY komponent — nie istnieje w DS. Po co: … Warianty/stany: …"
4. **Hide, don't delete** anything you remove from a duplicated layout, so the designer can compare.
5. **Only real content.** Use existing copy unless the task is copy; new copy follows the `copy-pl` skill. Never invent testimonials, numbers or features — use clearly labelled placeholders.
6. **Respect product reality** (see `context/`): no features the product doesn't have unless the variant is explicitly a "Bigger Bet" — and then label it "wymaga developmentu".

## Process
1. **Frame the problem** (2–4 lines): user problem, business goal, constraint. If ambiguous, ask one question before building.
2. **Diverge**: decide variants from genuinely different angles, e.g.
   - A — *Refine*: same structure, Apple-grade polish (hierarchy, spacing, copy, one CTA).
   - B — *Rethink*: different structure/interaction from first principles.
   - C — *Bold*: new component or pattern, best possible experience even if it needs dev.
   Default 3 variants; follow the number the user asks for.
3. **Build** each variant to the right, named `<width> | <Screen> — Wariant A (refine)` etc.
4. **Annotate** next to each variant a notes card (DS surface, Body/Medium):
   - Co się zmieniło (changes; use "Było: …" for text swaps)
   - Dlaczego — user benefit · business benefit
   - Ryzyka / trade-offs
   - 🆕 new components used
   - Dev cost: brak / mały / duży
5. **Verify**: `get_screenshot` each variant; check alignment, overflow, contrast, touch targets ≥ 44px.
6. **Recommend** in chat: TL;DR, a comparison table (Variant · Best for · User win · Business win · Risk · Dev cost), and which one you'd ship and why. Link node ids.

## Responsive (when asked)
Base 1366 → 1024 → 800 → 600 → 360 → 320. Use the DS "Units" variable modes (Desktop/Tablet/Mobile) and DS size variants of Top Bar Menu / Footer. Place breakpoints left-to-right next to the source.

## Tooling gotchas
- Screenshots: `get_screenshot` with `enableBase64Response: true`; never curl figma.com assets (blocked).
- Pass plain `123:456` ids to `get_screenshot` (instance ids `I…;…` fail).
- Keep `use_figma` return values small (< 20 KB); build large layouts in several calls.
- If Figma MCP disconnects, reload its tools via ToolSearch and continue from the last built node.
