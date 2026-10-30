# 11 · SQRG Core Summary (Quick Reference)

> A map of the most important concepts in SQRG Sep 11, 2025, in our own words. Enough for most tasks. For detail and examples, open the numbered files cited in each section.
> Indonesian counterpart: `references/id/11-core-summary.md`.

## 1. What SQRG is and isn't

- Guidelines for **human raters** who assess Google's search quality. Their ratings are used to **measure and improve** search systems, not to raise/lower specific pages. A single rating has no direct ranking impact.
- Value for SEO: it shows **the quality standard Google's systems aim for**. Don't call it a "ranking factor" list.
- Two main assessments: **Page Quality (PQ)**, query-independent, and **Needs Met (NM)**, query-dependent. → `01`, `10`

## 2. Page Quality on one page

**Three steps:** (1) is the real purpose harmful or deceptive? → Lowest. (2) Potentially harmful, untrustworthy or spammy? → Lowest. (3) If not, rate how well the page achieves its purpose. → `02`

**Scale:** Lowest · Low · Medium · High · Highest (plus in-between values). Torn between two → choose the lower. → `07`

**Considerations:** page purpose; degree of YMYL; site type; info about site/creator; MC quality; title; role of ads/SC; reputation; Trust (E-E-A-T). They influence each other. → `02`

**YMYL:** topics that can significantly affect health/safety, finances, government/civics/society, or well-being. A spectrum. Quick tests: would a careful person seek experts? Would a casual chat with friends be enough? → `01`

**MC / SC / Ads:** MC = what directly achieves the purpose (including the title and content behind tabs); SC = support (navigation, etc.); Ads = all monetization, including affiliate links. **Ads existing or not is not, by itself, a reason to raise or lower a rating.** → `01`

**MC quality = effort + originality + talent/skill + accuracy** (accuracy and expert consensus are mandatory for informational/YMYL content). Uncurated mass automation ≠ effort. → `02`

**E-E-A-T:** Experience, Expertise, Authoritativeness support **Trust**, the most important. An untrustworthy page has low E-E-A-T however expert it seems. YMYL: advice and factual info should come from experts; sharing lived experience is fine if safe and consistent with consensus. → `02`, `07`

**Reputation:** from independent sources, not the site's own claims. For YMYL, from experts in the field. Traffic data isn't reputation evidence. No reputation info ≠ a bad sign for small sites. → `02`

## 3. Rating triggers (any one is enough)

**Lowest** → `03`, `04`
- Harmful/deceptive purpose; made for the owner's gain with almost no effort to help.
- Harmful to self/others, harmful to groups, or harmfully misleading.
- No info at all on who's responsible, for YMYL or sites handling money/data.
- Very negative reputation; highly untrustworthy.
- MC deliberately covered by ads/pop-ups/interstitials.
- Extremely misleading or sensational title.
- Hacked, defaced, full of comment spam; gibberish.
- **Spam:** expired domain abuse, site reputation abuse, scaled content abuse, and MC that is entirely/nearly entirely copied, paraphrased, embedded, auto/AI-generated or reposted **with no effort, originality and added value** (still Lowest even if the source is credited).
- Fake author profiles (including AI personas), fake expertise claims, fake "we tested it" claims.

**Low** → `05`
- MC lacking effort/originality/skill; mild inaccuracies.
- Much repackaged MC with little added value.
- Lots of filler, or filler so prominent the MC is hard to find.
- Somewhat misleading or exaggerated title.
- Very distracting ads/SC.
- Unsatisfying site/creator info for the purpose (especially stores and YMYL).
- Mildly negative reputation; inflated expertise claims.
- E-E-A-T inadequate for the topic. A good site reputation does **not** make up for this.

**Medium** → `05`: purpose achieved; "nothing wrong, nothing special", or a mix of High signals and mild Low signals. "Average" pages sit here.

**High** → `06`: baseline met, plus at least one: MC with high effort/originality/skill; positive reputation; high E-E-A-T.

**Highest** → `06`: the same at the "very" level: the best content on its topic, very positive reputation, or a uniquely authoritative source.

## 4. AI content according to SQRG (cross-section summary)

- Generative AI is defined as a **tool** that can help or be misused. **Using AI does not by itself determine the rating.** → `01`, `03`
- What's judged: effort, originality, added value, accuracy and honesty. Uncurated AI for mass production = scaled content abuse. Entirely AI MC with no added value = Lowest. → `03`
- Signals raters recognize: leftover chatbot sentences, truncated sentences, odd factual errors, answers that make sense sentence by sentence but don't connect, sites covering anything far outside their focus, mass Q&A formats built from "People Also Ask" questions. → `04`
- AI-generated author personas = deceptive info → Lowest. → `03`

## 5. Needs Met on one page

**Scale:** FullyM (only for queries with one specific target: a particular site or a Know Simple fact, with **nearly all** users satisfied) · HM (very helpful; **the highest possible rating for most queries**) · MM (helpful, average to good) · SM (less helpful, or helpful for an unlikely interpretation) · FailsM (fails, off-topic, wrong, stale or useless). → `09`

**Key principles:** → `09`, `10`
- Understand the query first: interpretations (dominant, common, reasonable minor, unlikely minor, no chance) and intents (Know/Know Simple, Do, Website, Visit-in-Person). → `08`
- **Missing a key aspect of the query** (year, location, "non", comparison) → FailsM, not SM.
- Useless results = FailsM even with high PQ. Very low-PQ pages (scams, gibberish) = FailsM, except for navigational queries to that very site.
- A very misleading SERP title → SM or lower.
- Queries needing fresh content (news, recurring events, prices, products): stale content → low to FailsM.
- Queries in the locale's language → users want results in that language, even when typing proper nouns or English words in Latin script. Exceptions: global official sites being sought, technical info that's normally in English.
- Diverse results (format, perspective, depth, site type) can all be HM.
- For local queries, "near" depends on the type of place.

## 6. Five core questions before publishing

1. What is this page's purpose, and is it genuinely to help readers? → `01`
2. How YMYL is the topic, and do accuracy and expertise match that level? → `01`, `02`
3. What value does this page add over the existing top results? → `03`, `05`
4. Are the author's and publisher's experience, expertise and identity visible and verifiable? → `02`
5. For the target keyword, does the page answer the dominant intent directly, completely, currently and in the right language? → `08`, `09`, `10`

For a full audit, use `12-audit-checklist.md`.
