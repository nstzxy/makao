# Handoff — makao setup (from cloud session, 2026-10-11)

You're continuing setup of `~/repos/makao` (GitHub `nstzxy/makao`), a **workspace for Odrabiamy's holistic product designer**. It covers UX, UI, product decisions, product research, prototypes and C-level presentations across the whole company. The repo holds context and Claude tooling, not production code.

Start with `git fetch && git checkout claude/busy-johnson-8ebnzl`, then read `CLAUDE.md`, `context/company.md`, `context/design-system.md` and the 3 skills in `.claude/skills/`.

## 1. Where things stand
Branch `claude/busy-johnson-8ebnzl` (pushed, **not merged to main**):

| File | What |
|---|---|
| `CLAUDE.md` | Who the user is, working rules, where outputs go, skills, tool notes |
| `context/company.md` | Company, products, satellites, audience, pricing, competitors, regulation, gaps. ⚠ = from web research, unverified |
| `context/design-system.md` | Figma file keys, DS WEB 2.0 tokens, components, breakpoints |
| `.claude/skills/audit/` | First-principles, Apple-grade audit: good/bad practices, impact/effort, devil's advocate, Quick Wins / Bigger Bets |
| `.claude/skills/figma-variants/` | Variants as new frames **to the right** of the original; DS components and tokens; **new components allowed**, prefixed `🆕` + comment "NOWY komponent — nie istnieje w DS" |
| `.claude/skills/copy-pl/` | Short, warm, consistent Polish copy + typography; each line labelled Rodzic vs Uczeń with an argument so the designer decides |

## 2. To do (in order)
1. **Create `.claude/settings.json`.** It was blocked in the cloud session; the user approved it:
   ```json
   { "permissions": { "allow": ["mcp__Figma", "mcp__plugin_figma_figma"] } }
   ```
   Check the real Figma MCP server name locally (`/mcp`) and adjust the prefix (desktop Figma MCP may be named differently). Reason: every `use_figma` call needed manual approval, which caused stalls of hours and one abandoned session.
2. **Adapt "Tool notes" in `CLAUDE.md` for local use.** The cloud notes (proxy blocks figma.com assets and odrabiamy.pl; `/opt/pw-browsers`) may not apply locally. Keep the Figma API gotchas: plain `123:456` ids, `use_figma` returns < 20 KB, `get_metadata` per section, one query per `search_design_system`, preload Noto Sans.
3. **Verify the ⚠ facts in `context/company.md`.** Locally you can probably reach odrabiamy.pl, the satellites and the app stores. Check: free-tier limits, current prices, satellite URLs (fiszki, kartypracy), store ratings, whether web Premium is truly one-time. Remove ⚠ when confirmed. **Designer-confirmed facts win over web sources.**
4. **Ask the user the open questions** (they asked to be asked about missing context), then update `context/`:
   1. Current company priorities / OKRs and key numbers (paying users, conversion, web vs app split)?
   2. Who do they present to (CEO, COO, POs), and what format lands?
   3. Brand / tone-of-voice guide? Odrabiak mascot visuals?
   4. Do the apps share DS WEB 2.0, or is there a separate app Figma file?
   5. Research sources available (NPS, support ticket themes, analytics tool, past research)?
5. **Proposed next skills/agent** (user hasn't confirmed yet, so ask first):
   - `pitch`: idea → C-level deck (problem → evidence → options → recommendation → impact/cost → ask), max ~8 slides
   - `prototype`: Figma frame → shareable clickable HTML; real content only, DS tokens
   - `research`: competitor scans, app-store review mining, synthesis with sources
   - `devils-advocate` agent (`.claude/agents/`): read-only independent critic from UX / product / business angles
6. After the user reviews: **merge the branch to `main`** (ask first), then delete `HANDOFF.md`.

## 3. User preferences (from 22 past sessions)
- Ask clarifying questions before answering; keep it brief; TL;DR first.
- Writes English (casual, typos) or Polish. Reply in their language; **all UI copy in Polish**.
- Recurring asks:
  - "first principles", "Apple-grade experience", "don't be biased"
  - devil's advocate, pros/cons
  - UX + product + business perspectives
  - 3–5 variants
- Deliverables go to **Figma / Artifacts**, never repo files. They explicitly rejected a committed .md report and an unused app scaffold.
- Corrections they had to make (don't repeat):
  - No parent account / parent "mode". The Rodzic/Uczeń switch only changes messaging.
  - No subscriptions on web.
  - Concepts must not need new landing functionality unless asked.
  - Copy too long; copy that blamed parents ("nie dajesz rady").
  - "AI-sounding" copy.
  - Off-brand fonts in prototypes. Use Noto Sans, `#4f4fee`, `#313859`.
- Figma workflow:
  - Clone to the right, never edit the original.
  - Hide, don't delete.
  - Notes card next to each variant.
  - Dev Mode annotation "Było: …" on changed text.
  - The user edits the file live, so re-read nodes each turn.
- Figma connector must use the work account anastasiaplytka@odrabiamy.pl (org MAKALU MEDIA), not the personal Gmail.

## 4. Past-session evidence (for reference)
22 cloud sessions, 2026-09-10 → 10-08, all in `nstzxy/fantasticorterrible` (now retired, effectively empty). Most were Figma work on "RAW | Oferta 2026" (`9BxxFK7x8eAGfGEokS4VEH`):
- payment variants
- parent-section concepts
- CRO audits
- copy shortening
- responsive 1366→320
- above-fold variants
- illustrative tiles
- live HTML prototype
- satellite-products ecosystem audit
- component spec review in DS WEB 2.0 (`TYJ2jXpMeucSOqeGNmhjMX`)

Notable outputs:
- Live prototype "Oferta Rodzice 2026": https://claude.ai/artifact/K66X9qb9BGw4EAJrFL4iCa
- Ecosystem audit doc: https://claude.ai/artifact/NZxSicdQxxEA1WKrVekzdE
- Wireframes: https://claude.ai/artifact/7XeaYzUfuKq16wzXjNABvb

Tool usage was dominated by Figma `get_screenshot` (~270) and `use_figma` (~250). No `design:*` skills were used, though `design:accessibility-review`, `user-research`, `research-synthesis` and `design-handoff` fit the work.

## Git
Author: `nstzxy <anastasiaplytka@odrabiamy.pl>`. Commit only repo-tooling changes (CLAUDE.md, context/, .claude/).
