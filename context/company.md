# Odrabiamy — company & market context

Sources: designer's input in past sessions (treated as truth) + public web research Oct 2026 (marked ⚠ = unverified / from search snippets). Facts checked against odrabiamy.pl / regulamin on 2026-10-11 are marked ✓. When the designer says otherwise, update this file.

## Company
- **Odrabiamy.pl**, operated by **MAKALU MEDIA sp. z o.o. sp. k.**, Kraków (Zabłocie 43A). Founded as Dajspisac.pl (~2013), rebranded 2015 when paid access started.
- Leadership (public LinkedIn ⚠): Paweł Kruszelnicki (CEO, co-founder), Łukasz Wedel (COO), Piotr Pilch (education & customer service). Product Owner Lead: Aleksandra Obiezierska. Team ~51–200.
- Public financials (KRS ⚠): revenue ~29 mln zł (2023, 2024) → ~22 mln zł (2025), loss in the latest year. Growth/retention of paying users is the business priority.
- **Current priority (designer, 2026-10-11): conversion** (free → Premium). Judge ideas by their conversion effect first.
- **Stakeholders:** ideas go to the CEO. The focus is on strong ideas, not polished presentations.
- **Brand:** no brand book or tone-of-voice guide exists; `copy-pl` is the de facto tone. Odrabiak mascot illustrations live in Figma files (link pending); the visual direction is **3D**.
- "Grupa Odrabiamy" = the main product + satellite sites (brand label, not a separate legal entity ⚠).

## Products
- **Odrabiamy.pl (web) + app "Odrabiamy – pomoc w nauce"** (iOS / Android):
  - Rozwiązania krok po kroku written by teachers, mapped to specific Polish textbooks and pages (3 000+ books). This is the moat.
  - **Kursy wideo**: 100+ courses, E8 / matura.
  - Free notes, tests and worksheets.
  - **Odrabiak** AI assistant and **Odrabiak Pro** (grounded in textbook content; explains, grades the student's solution, quizzes; accepts photos).
  - Textbook barcode scanner in the app.
- **Satellites** (drive traffic → main site → Premium; one login and one Premium cover all):
  - ustna.odrabiamy.pl: symulator matury ustnej
  - arkusze.odrabiamy.pl: Arkusze CKE; the top traffic satellite
  - fiszki.odrabiamy.pl: fiszki do nauki ✓
  - kartypracy.odrabiamy.pl: karty pracy ✓
  - konkursy.odrabiamy.pl: konkursy i stypendia
  - blog.odrabiamy.pl (no wiki link in the footer as of 2026-10-11)
- Partnerships:
  - Bezpieczny.pl / Generali Finance ✓: buying school NNW insurance gives a Premium trial + discount on annual access. Promo rules effective 7 May 2026: 14-day trial, annual access −20% or −30% (by policy variant). Source: [bezpieczny.pl regulamin](https://bezpieczny.pl/dokument/regulamin-odrabiamy-pl).
- No B2B / teacher product known.

## Audience & accounts (designer-confirmed)
- Students 7–19 (szkoła podstawowa 1–8, liceum, technikum) use the product. **Parents pay.**
- **There is no parent account, no parent "mode", no parental controls.** Premium is bought while logged into the child's account (or the parent creates an account and hands the login to the child). In the apps, the child can ask and the parent approves via Google Play / App Store "ask to buy".
- The "Jestem rodzicem / Jestem uczniem" switch on landings only changes the messaging (and routes students to their landing). Prices and package contents are identical.
- Parents often just want to see what the platform is; most don't know there are student/parent distinctions.

## Pricing & payments (designer-confirmed)
- Premium: **Miesiąc 49 zł · 3 miesiące 99 zł · Rok 249 zł** (≈ 21 zł / mies.; the 21 zł annual anchor is fixed). Order on page: Miesiąc | 3 miesiące | Rok.
- **Web = one-time payment, no auto-renewal, no stored card data.** ✓ Regulamin: access switches off when the period ends; renewing needs a new payment. Web methods: PayU przelew (online or tradycyjny, up to 3 business days), BLIK, karta, Google Pay, Apple Pay, SMS+ (Mobiltek, 48 zł one-time).
- Subscriptions exist **only in the mobile apps** ✓ (App Store / Google Play; periods 1 mies., 3 mies., rok; store rules: billed amount must be most prominent).
- 14 dni na odstąpienie od umowy ✓.
- Account = one person; max one mobile device + one computer per day, or a temporary block ✓ (regulamin).
- Usage limits in regulamin ✓: max 240 tasks viewed/day and 15 questions/day in the AI tab (worded as general limits; the designer says Premium has no limits).

## Free vs Premium (designer-confirmed 2026-10-11)
| | Free | Premium |
|---|---|---|
| Rozwiązania w podręcznikach | selected exercises only | all exercises in all books |
| Kursy wideo i lekcje | — | all |
| AI on the book page | — | yes |
| Odrabiak (AI) | basic, cheaper LLM, daily limits | stronger LLM, no limits |
| Satellites (checked 2026-10-11) | ustna: 20/50 niejawne + 20/50 EN sets, 1 of 5 common errors · arkusze: all CKE tasks, no zadania autorskie · fiszki: ~same as Premium · kartypracy: poziom Odkrywca only · konkursy, blog: no login, no difference | ustna: all sets + transkrypcja PRO · arkusze: zadania autorskie, Odrabiak PRO plan, per-task stats · fiszki: Odrabiak PRO · kartypracy: Mistrz, Ekspert, Wersja A/B |
- Never: dark patterns, decoys, strikethrough fake prices, fake urgency. Savings must be honest and say what they compare to.

## Competitors
Brainly (biggest, Kraków-born, community + AI), Photomath (maths, photo), Gauth (ByteDance AI), ChatGPT / Gemini, zadania.info, matematykaszkolna.pl, private tutoring.
Positioning: textbook- and curriculum-exact, teacher-written, plus grounded AI. It aims to be a learning platform that replaces tutoring, not just homework answers.

## Market & regulation
- **Homework limits** (since 2024): grades 1–3 no written homework; grades 4–8 optional, not graded; secondary schools unaffected. This is a headwind for "homework help" positioning, so lean into learning, exams and understanding.
- **Reforma26 "Kompas Jutra"**: new curriculum and textbooks from Sep 2026 (grades 1 and 4) and Sep 2027 (first year of liceum/technikum); old and new run in parallel until ~2031/32. Expect content-coverage and textbook-selection UX work.
- **Exams**: egzamin ósmoklasisty (E8, May), matura (from early May; oral PL + language).
- **Seasonality**: September start, January–February winter breaks by voivodeship, April–May exam peak, summer trough.
- **UOKiK**: actively fines dark patterns (hard cancellation, silent trial→paid) — up to 10% of turnover.
- **GDPR**: digital consent age in PL = 16, so under-16s need parental consent for consent-based processing. Relevant to any parent/child account ideas.
- **Accessibility**: target WCAG 2.2 AA (EAA in force since June 2025).

## Data & research
- **Analytics: GA4**, account `66621836`, two properties:
  - **Web (odrabiamy.pl)**: property `260847366`, [home](https://analytics.google.com/analytics/web/#/a66621836p260847366/reports/intelligenthome)
  - **Mobile apps (iOS + Android)**: property `442870372`, [home](https://analytics.google.com/analytics/web/#/a66621836p442870372/reports/intelligenthome). Observed 2026-10-11: ~44k active users/7 days, iOS 54% / Android 46% of key events; screen names are partly technical (`RNSScreen`, `UIViewController`), so screen-level reports need care.
  - For the whole picture (e.g. web vs app split), read **both** properties for the same date range. Read it in the built-in browser (read-only). Pull numbers from there; never invent them.
  - Observed 2026-10-11: the property is **web only** (platform WEB 100%). Products are tracked per payment method (`odrabiamy-premium_1_month_payu`, `_3_month_payu`, `_12_month_payu`, `_1_month_dcb`, `_30_day_dcb`). On the home card these showed 0 bought items while Purchases showed ~1.5k, so item-level e-commerce tracking may be broken or misnamed ⚠. Custom insights need edit rights (the designer is read-only).

## Known gaps (ask the designer before assuming)
Real metrics (MAU, paying users, conversion rate, web vs app split; get them from GA4) · who leads design/engineering · Odrabiak illustration Figma link · app tech stack · satellite owners and roadmaps (free/Premium audit: https://claude.ai/code/artifact/0f6ed47f-d416-44d8-80a1-6ed3da9412f3) · other research assets (NPS, support themes, past research) · A/B testing practice.
