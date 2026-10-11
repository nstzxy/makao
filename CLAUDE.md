# makao — Odrabiamy product design workspace

I'm a holistic product designer for the whole of Odrabiamy (odrabiamy.pl, apps, satellite sites). My work covers UX, UI, product decisions, product research, prototypes and presenting ideas to C-level. This repo holds **context and tools**, not production code.

Read before working: `context/company.md` (product, audience, pricing, market) and `context/design-system.md` (Figma files, tokens, components, breakpoints). Treat them as known facts; don't make me re-explain them. If something is missing or contradicted, ask me, then update the file.

## How I want you to work
- **Ask before assuming.** If the goal, audience (parent vs student) or constraint is unclear, ask 1–3 short questions first. Wrong product assumptions (e.g. parent "modes", subscriptions on web) have cost whole rounds.
- **Short first.** Lead with a TL;DR. Offer the long version or a shareable page in one line.
- **First principles, Apple-grade, unbiased.** Argue pros *and* cons, include a devil's advocate, and don't flatter my designs.
- **Business + user.** Every recommendation states the user win and the business win. Prefer solutions that need no new development unless I ask for "bigger bets", and label anything that does: "wymaga developmentu".
- **No invented facts.** No made-up stats, testimonials, competitor claims or features. Cite sources for research and mark anything unverified.
- **Language:** reply in the language I write in. All UI and product copy is **Polish** (see the `copy-pl` skill). Explain jargon in one line.

## Where work goes
| Need | Output |
|---|---|
| Design, variants, responsive | **Figma** (skill `figma-variants`): new frames to the right of the original, never edit the original |
| Review / audit | Chat (skill `audit`); Artifact page if it's for others |
| Live prototype to share | Artifact (single HTML, DS tokens: Noto Sans, `#4f4fee`, `#313859`), using only real content |
| C-level pitch | Slides artifact: problem → evidence → options → recommendation → impact/cost → ask. Max ~8 slides |
| Research / competitor scan | Doc artifact with sources |

**Don't create files in this repo** for deliverables (no .md reports, no app scaffolds) unless I ask. Scratch work goes in the scratchpad. The repo only changes when we improve `CLAUDE.md`, `context/` or skills.

## Skills
- `audit`: good and bad practices, first principles, Apple-grade, impact/effort, devil's advocate.
- `figma-variants`: best-solution variants next to the original; DS components and tokens; new components allowed, marked 🆕.
- `copy-pl`: short, warm, consistent Polish copy and typography; states parent vs student tone with arguments.
- Also useful: `design:accessibility-review`, `design:user-research`, `design:research-synthesis`, `design:design-handoff`, `figma:figma-use` (required before `use_figma`).

## Tool notes (cloud sessions)
- Figma connector must be the **work** account (anastasiaplytka@odrabiamy.pl, org MAKALU MEDIA). On "no edit access", run `whoami` and tell me to reconnect.
- The proxy blocks figma.com asset URLs and odrabiamy.pl (+ subdomains). Use `get_screenshot` with `enableBase64Response: true`, never curl. Ask me for screenshots of live pages, or try the browser tool.
- Figma: plain `123:456` node ids for screenshots; `use_figma` returns < 20 KB; `get_metadata` on sections, not whole pages; one query per `search_design_system`; preload Noto Sans weights. Re-read nodes each turn, because I edit the file live.
- Playwright: Chromium is under `/opt/pw-browsers`.
- Git (only when changing this repo): author `nstzxy <anastasiaplytka@odrabiamy.pl>`, `claude/*` branches.
