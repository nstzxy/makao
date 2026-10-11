# Satelity Odrabiamy — Free vs Premium

2026-10-11 · Nastka · Live doc (may be newer): https://claude.ai/code/artifact/0f6ed47f-d416-44d8-80a1-6ed3da9412f3

Four of six satellites gate something behind Premium, but each does it differently and two never mention Premium at all. The quickest wins are honest copy on ustna ("w pełni darmowe", "od 20 zł") and a working upsell on kartypracy's locked levels, the one satellite written for parents.

- **Strongest:** ustna. Clear walls at useful moments (common errors, Premium-only questions), each with a benefit list.
- **Weakest:** kartypracy (locked buttons do nothing), konkursy and blog (no Premium at all), fiszki (free and Premium look the same; possible shared-progress bug ⚠).
- **Inconsistent:** four different upsell CTAs and three different benefit lists across satellites.

## Overview

| Satellite | Login | What free gets | What only Premium gets | Paywall / upsell for free users |
| --- | --- | --- | --- | --- |
| ustna | Odrabiamy SSO | 76 pytań jawnych + 20/50 niejawnych + 20/50 English sets to simulate, opracowania, PDFs | 30 niejawne + 30 English sets, all common errors, "transkrypcja PRO" | Clear walls with a benefit list; "Nauka to nie luksus" block |
| arkusze | Odrabiamy SSO | All CKE tasks and sheets, AI check, exam mode, PDFs, plan | Zadania autorskie, Odrabiak PRO tips/plan, per-task stats and common errors | Wall on authored sheets; upsell block on Moja nauka |
| fiszki | Odrabiamy SSO | Everything visible (sets, quizzes, podcast, test PDFs) | Odrabiak PRO generation (free page also claims PRO ⚠) | Upsell card on Moja nauka only |
| kartypracy | Odrabiamy SSO | Poziom Odkrywca of every worksheet | Mistrz, Ekspert, Wersja A/B | Lock icons + one line of copy; clicking a lock does nothing |
| konkursy | none (email leads) | Everything | Nothing | None |
| blog | none | Everything | Nothing | None (links to odrabiamy.pl only) |

## ustna.odrabiamy.pl: symulator matury ustnej

The simulator is "darmowy" on the landing page, but Premium unlocks 30 of the 50 pytania niejawne and 30 of the 50 English sets for simulation, all common-error lists, and a better speech-to-text model. Free users can still read every question in full.

| Funkcja | Free (Basic) | Premium |
| --- | --- | --- |
| Symulacja: 76 pytań jawnych (PL) | yes | yes |
| Pytania niejawne (50): reading the material | all 50 | all 50 |
| Pytania niejawne: simulation | 20 of 50; the other 30 are tagged "Premium" and show a wall | all 50 |
| Zestawy z angielskiego (50): simulation | 20 of 50 (30 tagged "Premium") | all 50 |
| Opracowanie pytania jawnego: omówienie, konteksty, mapa wypowiedzi | yes | yes |
| PDF: opracowanie + pełna odpowiedź | yes (both return the PDF) | yes |
| "Najczęstsze błędy" per pytanie jawne | 1 of 5, then a wall | all |
| Speech-to-text and grading | standard | "transkrypcja PRO" / "najlepszy model AI" |
| Moja nauka (/konto): progress map, daily tip, history | yes + upsell block | yes + "Masz aktywne Odrabiamy Premium" |
| Audio opracowanie | links out to an odrabiamy.pl video course (gating not checked ⚠) | same link |

**Paywall copy (free account):** "Pozostałe 4 najczęstsze błędy przy tym pytaniu są dostępne w Odrabiamy Premium" and "Symulacja tego pytania jest dostępna w Odrabiamy Premium. Masz je przed sobą w całości." Both list the same benefits and use the CTA "Aktywuj Odrabiamy Premium", which goes to odrabiamy.pl/oferta/dostep-premium/zakup-premium.

**Upsell block "Nauka to nie luksus"** (on /konto and the niejawne list, free only) compares "KURSY U KONKURENCJI kilkaset zł" with "NA ODRABIAMY od 20 zł miesięcznie". On the list page the CTA reads "Zacznij naukę z Odrabiamy"; elsewhere it is "Aktywuj Odrabiamy Premium".

**Notes**

- The homepage FAQ says "Korzystanie z symulatora jest w pełni darmowe", but 60 of the 100 practice items are Premium-only. That mismatch is a trust and UOKiK risk.
- "od 20 zł miesięcznie" rounds down from 249 zł / 12 = 20,75 zł; the agreed anchor is 21 zł. "Kilkaset zł" for competitors has no source shown.
- Premium users still see the "Premium" tags, but nothing marks them as unlocked (for example a "W Twoim pakiecie" label).
- Not tested: whether the random draw in /polski and /angielski skips Premium-only items for free users (starting a simulation needs a microphone) ⚠.

## arkusze.odrabiamy.pl: Arkusze CKE

All CKE tasks and sheets are free. Premium adds the authored task sheets (zadania autorskie), Odrabiak PRO tips and study plans, and per-task stats. The full step-by-step solution links out to odrabiamy.pl, where the main paywall applies.

| Funkcja | Free (Basic) | Premium |
| --- | --- | --- |
| CKE sheets (E8, matura podst./rozsz.): every task, hint, AI check "Oceń moje rozwiązanie" | yes | yes |
| Tryb egzaminacyjny (timed full sheet), PDF of the sheet, PDF generator | yes | yes |
| Zadania autorskie (e.g. 11 authored sheets in matura podst. matematyka) | the start of each task, then a wall | full, with teacher explanations |
| "Pokaż pełne rozwiązanie na Odrabiamy" | links to the textbook solution on odrabiamy.pl (main-site gating) | same |
| Per-task extras: "To zadanie poprawnie rozwiązało 67% użytkowników", "Najczęstsze błędy w tym dziale", "Twój wynik w dziale" | not shown | shown |
| Moja nauka: daily tip and study plan | by Odrabiak, with the note "Wskazówki od Odrabiaka PRO są dostępne w Premium" | by "Odrabiak PRO (Premium)" |
| Moja nauka: zadania do poprawki (repeats after 3/7/14 days), map of topics, league, ranking | yes | yes |
| Wypracowania: AI essay check against CKE criteria | available; limit not tested ⚠ | available |

**Paywall copy (authored sheet, free):** "Arkusz autorski w Premium", "Widzisz początek każdego zadania. Całe zadania z wyjaśnieniami nauczyciela są w Premium." CTA: "Odblokuj Premium na Odrabiamy". The same box also says "Masz już Premium? Zaloguj się", even though the user is already signed in.

**Upsell on Moja nauka (free):** the "Nauka to nie luksus" block, with a shorter benefit list than on ustna ("wszystkie kursy, rozwiązania wszystkich podręczników i wiele innych funkcji"), "od 20 zł miesięcznie" and CTA "Aktywuj Premium na Odrabiamy".

**Notes**

- The strongest natural upsell moment is the AI-checked open task. A free user who just lost points gets no "Najczęstsze błędy" teaser there, while on ustna the same idea is used as a teaser.
- Not tested: daily limits on the AI checks ("Oceń moje rozwiązanie", wypracowania). I didn't submit answers, to keep the test account clean ⚠.

## fiszki.odrabiamy.pl: fiszki do nauki

On screen, free and Premium are almost identical: same flashcards, quizzes, podcast, test PDFs and plan. The only promised difference is that Premium sets are built by Odrabiak PRO, yet the free upload page also says it will use Odrabiak PRO.

| Funkcja | Free (Basic) | Premium |
| --- | --- | --- |
| Ready-made public sets, fiszki, quizy (4 etapy), ranking, postępy, XP | yes | yes |
| Own set from photo / PDF / text / topic, or written by hand | yes | yes |
| Model that generates the set | upload page: "Ten zestaw wygeneruje Odrabiak PRO - nasz najmocniejszy tryb" | Odrabiak PRO ("Odrabiaka PRO do każdego zestawu fiszek") |
| Podcast per set ("Zuza i Kuba", ~7 min) | yes | yes |
| Próbny sprawdzian / kartkówka PDF (wersja A/B, with key) | yes ("Pobierz pełny sprawdzian") | yes |
| Plan do sprawdzianu (date picker) | yes | yes |
| Moja nauka | upsell card | "Masz aktywne Odrabiamy Premium" card with links to Rozwiązania książek, Kursy wideo, Moje Premium |

**Upsell copy (free):** "Ucz się szybciej z Odrabiamy Premium. Każdy Twój zestaw układa Odrabiak PRO. Do tego rozwiązania wszystkich podręczników i kursy wideo do matury i egzaminu ósmoklasisty." CTA: "Aktywuj Premium na Odrabiamy".

**Notes**

- **Possible bug ⚠:** both accounts show the same 7 sets, the same 313 XP (Poziom 4 Prymus) and the same progress, in two separate browsers. One explanation is that fiszki matches accounts by base email and ignores the "+darmowe" part. Worth a check by the team, because it also makes this free-vs-Premium comparison unreliable for fiszki.
- The free upsell promises Odrabiak PRO as the Premium benefit, while the free upload page claims free sets also use Odrabiak PRO. Either free has a hidden PRO quota (not visible anywhere) or the copy contradicts itself ⚠.
- The page first renders as signed out ("Zaloguj się") and switches to the account a moment later. Users may briefly see a login prompt they don't need.

## kartypracy.odrabiamy.pl: karty pracy

Each worksheet has three difficulty levels and two extra versions. Free gets only the easiest level (Odkrywca); Premium unlocks Mistrz, Ekspert and Wersja A/B ("przygotowane przez Odrabiaka PRO"). This is the cleanest freemium split of all the satellites, but the locked buttons do nothing when clicked.

| Funkcja | Free (Basic) | Premium |
| --- | --- | --- |
| Catalogue: 772 worksheets, filters by subject, age 3–6 and klasa 1–8 | yes | yes |
| Poziom Odkrywca (PDF, with answers) | yes ("Pobierz za darmo") | yes |
| Poziomy Mistrz, Ekspert | locked (lock icon) | yes |
| Wersja A / Wersja B (Odrabiak PRO) | locked (lock icon) | yes |
| Cross-sell "Czy to książki Twojego dziecka?" (textbooks for that klasa on odrabiamy.pl) | yes | yes |
| Header account badge | email only, no "Basic" | "Premium" |

**Free copy under the levels:** "Poziom Odkrywca jest za darmo, poziomy Mistrz i Ekspert oraz wersje A i B - w Odrabiamy Premium." **Premium sees:** "Masz Odrabiamy Premium - możesz pobrać wszystkie."

**Notes**

- **Dead click:** on the free account, clicking a locked level (Mistrz) changes nothing: there's no preview, modal or CTA. It's the moment of highest intent on this site, and it has no path to Premium.
- This is the only satellite clearly written for **parents** ("dla rodziców i nauczycieli"), so it's the best entry point for the paying audience. The upsell should talk to parents, not students.
- "E-mail potwierdzasz tylko raz" is shown to signed-in users too, where it adds noise.
- Not tested: the "Darmowy generator kart pracy" and the download flow itself (I didn't download a file) ⚠.

## konkursy.odrabiamy.pl: konkursy i stypendia

There is no free/Premium difference here, and no Odrabiamy login at all. Both accounts see the same 242 entries (64 konkursy kuratoryjne for małopolskie, 84 olimpiady, 25 stypendia). The site captures email leads instead.

| Funkcja | Free | Premium |
| --- | --- | --- |
| Database, filters (województwo, poziom), calendar, poradniki | yes | yes |
| Entry page: dates, materials, past papers, links to the organiser | yes | yes |
| "Dodaj do ulubionych", Google / ICS calendar export | yes | yes |
| "Wyślij mi szczegóły" (email + marketing consent), "Powiadomienia o nowych konkursach" | yes | yes |
| Any Premium mention or gated content | none | none |

**Cross-sell:** each entry has an "Arkusze Odrabiamy" block ("Jak uczyć się skutecznie, rozwiązując arkusze CKE?", "Darmowa baza arkuszy CKE →") and a "Rozpocznij naukę" link to odrabiamy.pl on the homepage.

**Notes**

- **Mismatched cross-sell:** the konkurs kuratoryjny page is for klasy 4–8, but the arkusze block promises "prognoza na maturę". A better match would be E8 sheets or the textbook solutions for that klasa.
- Konkursy attracts motivated, high-performing students and their parents. That's a strong Premium audience, yet the site never mentions Premium (for example kursy wideo for olympiad subjects).
- Konkursy is the only satellite without an Odrabiamy account; it captures emails with marketing consent instead. That's fine for leads, but these users are never recognised as Odrabiamy users ⚠.

## blog.odrabiamy.pl: blog

The blog is a separate WordPress site with no Odrabiamy login, so free and Premium see exactly the same thing. It never mentions Premium; it links to odrabiamy.pl content instead.

- **Links out:** a header banner "Odrabiamy.pl | Serwis edukacyjny dla uczniów, który tworzą nauczyciele | Wypróbuj za darmo", a /kursy banner, and in-article links to odrabiamy.pl/pytania-i-odpowiedzi ("Zadanie 1.", "Zadanie 2.").
- **Cookie banner:** it offers "Odrzuć opcjonalne" as an equal choice, which is good. I declined optional cookies.

**Notes**

- The Facebook and LinkedIn share buttons share http://odrabiamy.pl instead of the article URL, so shared posts lose the article (seen on the Kongres wiedeński post) ⚠.
- Links still use http:// rather than https://.
- Typo in the page title on every page: "Arykuły tworzone dla uczniów" (should be "Artykuły").

## Conversion opportunities

The free → Premium nudge is strong on ustna, decent on arkusze, weak on fiszki and kartypracy, and missing on konkursy and the blog. Most fixes are copy or small UI changes.

| # | Opportunity | User win | Business win | Dev cost |
| --- | --- | --- | --- | --- |
| 1 | kartypracy: clicking a locked level shows a preview of its first page and a short Premium card written for parents | Sees what Mistrz/Ekspert looks like before paying | Turns the highest-intent click into a path to Premium | mały development |
| 2 | ustna: rewrite "w pełni darmowe" in the FAQ to say what is free and what is Premium | No surprise walls | Trust; lowers UOKiK risk | bez developmentu (copy) |
| 3 | All satellites: change "od 20 zł miesięcznie" to "od 21 zł" (249 zł / 12) and drop or source "kilkaset zł" for competitors | Honest price | Consistent anchor; no unsupported claims | bez developmentu (copy) |
| 4 | arkusze: after an AI-checked answer, show free users one "Najczęstszy błąd w tym dziale" + a wall, as ustna already does | Learns from a mistake right away | Upsell at the moment of need | mały development |
| 5 | One upsell system: same benefit list, same CTA ("Aktywuj Odrabiamy Premium"), with the satellite's own benefit first | Clear what Premium adds here | Consistent message; easier A/B tests | mały development |
| 6 | Hide "Masz już Premium? Zaloguj się" for signed-in users (arkusze) | Less confusion | Cleaner wall | mały development |
| 7 | konkursy: match the cross-sell to the entry (E8 sheets for klasy 4–8, kursy wideo for olympiad subjects) and mention Premium | Relevant help for the contest | Reaches a motivated audience that converts well ⚠ | mały development |
| 8 | Premium users: mark unlocked items ("W Twoim pakiecie") instead of a plain "Premium" tag | Feels the value they pay for | Retention / renewal on web (one-time payments) | mały development |

**Devil's advocate**

- The satellites drive traffic (arkusze is the top traffic satellite). More walls could cut SEO and top-of-funnel volume more than they add in conversion. Test every new wall as an A/B test in GA4 (web property 260847366) and measure traffic, signups and purchases together.
- Free generosity on arkusze and fiszki may be deliberate acquisition. Changing it is a product decision, not a UX fix.
- Fixes 2 and 3 are needed regardless of conversion: they're honesty issues.

## Open questions

- [ ] fiszki: why do both accounts show the same sets, XP and progress? Possible merging of "+alias" emails.
- [ ] fiszki: does the free account get a hidden Odrabiak PRO quota, or is the "wygeneruje Odrabiak PRO" copy wrong?
- [ ] ustna and arkusze: daily limits on AI grading (simulations, "Oceń moje rozwiązanie", wypracowania) for free users. Not tested, to keep the test account clean.
- [ ] ustna: does the random draw for free users skip Premium-only questions and sets?
- [ ] Main-site gating of links from satellites (the audio opracowanie course, "Pokaż pełne rozwiązanie na Odrabiamy") wasn't checked.
- [ ] Who owns each satellite? Fixes 1–8 need an owner per site.

**Method:** checked on 2026-10-11 with two accounts signed in at the same time: Premium in the Claude built-in browser, Basic (free, +darmowe) in Chrome. I read pages and clicked controls, but didn't submit answers, download files or change settings.
