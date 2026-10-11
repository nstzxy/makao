---
name: research
description: Product research for Odrabiamy with sources — competitor scans, app-store review mining, live-site checks, GA4 data pulls and synthesis into insights and opportunities. Use for "research", "competitor scan", "what do users say", "app store reviews", "how do others do X", "check the data", "zbadaj", "porównaj konkurencję", "co mówią użytkownicy", "sprawdź w GA".
---

# Research — evidence, not opinions

Goal: give the designer evidence they can defend in front of the CEO. Every claim has a source; anything unverified is marked ⚠.

## 0. Frame the question
- Read `context/` first. Ask 1–3 short questions if unclear: the decision this research feeds, audience (Rodzic vs Uczeń), surface (web / app / satellite), depth (quick scan vs deep dive).
- Write the research question in one line and what result would change the decision.

## 1. Sources (use what fits)
- **GA4**: web property `260847366` (`https://analytics.google.com/analytics/web/#/a66621836p260847366/...`) and mobile apps property `442870372` (`.../#/a66621836p442870372/...`). Open them in the built-in browser; the designer is signed in there. Use reports and explorations for funnels, conversion by device, landing page, source and season. Read numbers with `get_page_text` and trend arrows (↑/↓) from a screenshot. Always state the date range and compare to the same period last year (seasonality: September, winter breaks, April–May exams). If the sign-in has expired, ask the designer to sign in again; never enter credentials.
- **Live product** (odrabiamy.pl + satellites): built-in browser only (curl/WebFetch get 403 and miss logged-in states). The designer signs in to the free or Premium account; never type passwords, sign out or buy.
- **App stores**: "Odrabiamy – pomoc w nauce" on App Store and Google Play. Sample recent reviews; tag theme, sentiment and audience (parent vs student); quote verbatim in Polish (short).
- **Competitors**: Brainly, Photomath, Gauth, ChatGPT/Gemini, zadania.info, tutoring (see `context/company.md`). Read their real pages (pricing, onboarding, paywall). Note the date seen.
- **Regulation/market**: UOKiK, curriculum reform, exams. Use official sources (gov.pl, CKE, uokik.gov.pl).
- Use `WebSearch` "standard" first; "extended" for niche or very recent facts. For broad scans, fan out with subagents.

## 2. Synthesis
- Group findings into **themes**; for each: insight (1 line) · evidence (sources, counts) · confidence (high / medium / low) · so-what for conversion.
- Separate **facts**, **interpretation** and **guesses**. No invented stats or quotes; small samples are labelled as such.
- End with **Opportunities**: user win · business win · effort ("bez developmentu" / "wymaga developmentu").
- **⚖️ Devil's advocate**: what would make this conclusion wrong (sampling bias, review skew to angry users, seasonality, survivor bias).

## 3. Output
- Quick question → chat: TL;DR (3 lines) + key findings + sources.
- Scan or deep dive → **Doc artifact** with sources linked inline and a "Metoda" section (what was checked, when, sample sizes). Offer it in one line for quick answers.
- If research confirms or corrects a fact in `context/`, propose the update (designer-confirmed facts win).
