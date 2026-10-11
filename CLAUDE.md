# makao — Odrabiamy product design workspace

I'm a holistic product designer for the whole of Odrabiamy (odrabiamy.pl, apps, satellite sites). My work covers UX, UI, product decisions, product research, prototypes and bringing ideas to the CEO. **The company priority now is conversion** (free → Premium). This repo holds **context and tools**, not production code.

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
| Live prototype to share | Artifact (skill `prototype`): single HTML, DS tokens (Noto Sans, `#4f4fee`, `#313859`), only real content |
| Idea for the CEO | Idea brief in chat (skill `pitch`); Doc artifact to share; slides only if I ask |
| Research / competitor scan / data | Skill `research`; Doc artifact with sources |

**Don't create files in this repo** for deliverables (no .md reports, no app scaffolds) unless I ask. Scratch work goes in the scratchpad. The repo only changes when we improve `CLAUDE.md`, `context/` or skills.

## Skills
- `audit`: good and bad practices, first principles, Apple-grade, impact/effort, devil's advocate.
- `figma-variants`: best-solution variants next to the original; DS components and tokens; new components allowed, marked 🆕.
- `copy-pl`: short, warm, consistent Polish copy and typography; states parent vs student tone with arguments.
- `pitch`: idea → decision-ready brief for the CEO (problem, evidence, options, recommendation, conversion impact, cost, ask).
- `prototype`: Figma frame → shareable clickable HTML artifact; real content, DS tokens.
- `research`: competitor scans, app-store reviews, live-site checks, GA4 data; synthesis with sources.
- Also useful: `design:accessibility-review`, `design:user-research`, `design:research-synthesis`, `design:design-handoff`, `figma:figma-use` (required before `use_figma`).

## Tool notes
- Figma connector must be the **work** account (anastasiaplytka@odrabiamy.pl, org MAKALU MEDIA). On "no edit access", run `whoami` and tell me to reconnect.
- Figma: plain `123:456` node ids for screenshots; `use_figma` returns < 20 KB; `get_metadata` on sections, not whole pages; one query per `search_design_system`; preload Noto Sans weights. Re-read nodes each turn, because I edit the file live.
- GA4: **web** property `260847366` (`#/a66621836p260847366/…`), **mobile apps** property `442870372` (`#/a66621836p442870372/…`). Read them in the **built-in browser** (I'm signed in there with read-only access). `get_page_text` gives numbers but loses ↑/↓, so take a screenshot for trend direction. Always state the date range and comparison period. Never invent numbers.
- Live pages: **always use the built-in browser** for odrabiamy.pl, the satellites and GA4. Don't use curl/WebFetch: odrabiamy.pl returns 403 (bot protection), and they can't see logged-in states. Logins: I sign in myself in the built-in browser (free or Premium account) and tell you which one is active. Never type passwords and never sign out; ask me to switch accounts.
- Cloud sessions only: the proxy blocks figma.com asset URLs and odrabiamy.pl (+ subdomains), so use `get_screenshot` with `enableBase64Response: true`; Chromium is under `/opt/pw-browsers`.
- Git (only when changing this repo): author `nstzxy <anastasiaplytka@odrabiamy.pl>`, `claude/*` branches.
