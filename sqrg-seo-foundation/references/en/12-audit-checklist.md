# 12 · SQRG-Based Content Audit Checklist

> A practical tool derived from SQRG Sep 11, 2025. The order follows the rater's logic: **check harm and spam first, then quality.** Numbers in parentheses point to reference files for detail.
> Indonesian counterpart: `references/id/12-audit-checklist.md`.

## How to use

1. Gather inputs: the page URL or text, target keyword (if any), author/site info, and if possible a few top competing results for calibration.
2. Run **Stages 0–2** in order. Red findings in Stage 1 are reported as top priority; still complete the other stages so the fix list is complete.
3. Estimate the PQ rating and, if there's a target keyword, the NM rating. Torn between two ratings → pick the lower.
4. Write the report using the template at the end.

---

## Stage 0 · Context

- [ ] **Page purpose** clear and beneficial? State it in one sentence. (01)
- [ ] **Site type**: personal blog, media, online store, institution, forum/UGC, official site? Expectations differ. (02)
- [ ] **YMYL level**: clearly YMYL / maybe / not. Category: health-safety, finance, government-civics-society, other. (01)
- [ ] **Target keyword intent**: Know, Know Simple, Do, Website or Visit-in-Person; dominant and reasonable minor interpretations. (08)
- [ ] **Locale**: readers' language and region (default: Indonesia, Bahasa Indonesia). (10)

## Stage 1 · Red-flag screen (Lowest triggers) (03, 04)

Any single "yes" = Lowest risk.

**Harm**
- [ ] Encourages actions that endanger self/others, or downplays the risks?
- [ ] Demeans or incites hatred against a group (seriously or maliciously)?
- [ ] Clearly false claims, claims against expert consensus, or baseless theories on topics that can cause harm? (A harmfully misleading title counts too.)

**Untrustworthy**
- [ ] YMYL or a site handling money/personal data with **no info at all** on who's responsible?
- [ ] Fake author profiles, invented personas, AI-generated author photos, or false credentials?
- [ ] "We tested it / independent review" claims that can't be backed up?
- [ ] Impersonating another brand, fake business info (e.g., a fictional physical store address), or fake "trust" logos?
- [ ] Ads disguised as content or navigation; deceptive buttons?
- [ ] MC covered by hard-to-close ads/pop-ups, or pushed far down by ads?
- [ ] Asks for personal data without a legitimate reason?

**Spam**
- [ ] All/nearly all MC copied, paraphrased, embedded, auto/AI-generated or reposted with no effort, originality and added value?
- [ ] Part of mass production of templated pages without curation (check several other pages on the site)?
- [ ] Unedited AI leftovers, truncated sentences, blank template sections, or incoherent text?
- [ ] Topics far outside the site's focus, especially YMYL on an unrelated site?
- [ ] Third-party content placed mainly to ride the domain's authority (site reputation abuse)?
- [ ] A former domain whose content doesn't fit its history (expired domain abuse)?
- [ ] Unnatural keyword repetition; comment spam; signs of hacking?

**Technical and link spam** (14)
- [ ] Googlebot and users get different content (cloaking), or redirects that only fire for mobile users / visitors from Google (sneaky redirects)?
- [ ] Text or links hidden from people (white-on-white, off-screen CSS, size/opacity 0, a link on one tiny character)? Accordions, tabs, tooltips and screen-reader text are fine.
- [ ] Sets of near-identical city/region or query-variant pages that funnel to one destination (doorways)?
- [ ] Paid, sponsored, product-for-review or partner links without `rel="sponsored"`/`nofollow`; keyword-rich anchors in guest posts/press releases; link exchanges or link widgets/footers spread across sites?
- [ ] Affiliate descriptions/reviews copied from the merchant with nothing added (thin affiliation)?
- [ ] Back button hijacking, malware/unwanted downloads, or a "tool" that doesn't work and funnels to ads (misleading functionality)?
- [ ] Manual actions or Security issues reported in Search Console?

## Stage 2 · Quality (Low, Medium, High) (02, 05, 06)

**Main Content**
- [ ] **Effort** visible: research, testing, own photos/video, data, examples, careful editing.
- [ ] **Originality**: something not in the other top results (unique data, first-hand experience, analysis, local examples).
- [ ] **Skill**: explained well enough that readers can actually use it.
- [ ] **Accuracy**: correct facts; for YMYL, consistent with expert consensus and the latest official guidelines; sources cited.
- [ ] Calibration: is this page better than a typical page on the same topic? If only on par, probably **Medium**.

**Structure and experience**
- [ ] The answer or core content is at the top, not buried under a long intro.
- [ ] No filler: generic definitions, facts everyone knows, rambling preambles.
- [ ] Ads and SC don't get in the way, especially on mobile; no racy or shocking ad images.
- [ ] Features (calculators, filters, cart, forms) work.

**Title**
- [ ] The H1 and title tag honestly summarize the content; no superlatives or sensational claims the content doesn't deliver.

**E-E-A-T and identity**
- [ ] Clear author: name, role, experience/credentials relevant to the topic.
- [ ] For advice-giving YMYL: the author or reviewer has matching expertise.
- [ ] For experience content: first-hand experience is visible in the content (photos, details, process), and it doesn't give advice that should come from experts.
- [ ] Clear publisher: About, Contact, editorial policy. For media: editorial team (Redaksi). For stores: customer service, payment, shipping, returns.
- [ ] Conflicts of interest disclosed (affiliate, sponsorship, own products). Remember: disclosure doesn't rescue content with no added value.

**Reputation** (research using `-site:` operators)
- [ ] What do independent sources say about the site and author? For YMYL, what do experts or institutions in the field say?
- [ ] Customer reviews: read the content, not just the stars. Credible fraud reports = red.

## Stage 3 · Needs Met for the target keyword (08, 09, 10)

- [ ] Answers the **dominant interpretation** and main intent directly.
- [ ] All **key aspects of the query** are covered: year, location, quantity, comparison, qualifiers ("without", "for beginners", "nearest").
- [ ] Format fits: a short answer up front for Know Simple; a comprehensive guide for Know; a tool/steps/CTA for Do; accurate location info for Visit-in-Person.
- [ ] **Fresh** if the query needs recent info (prices, regulations, products, recurring events); honest update dates.
- [ ] Language fits the locale; English technical terms only where they're normal.
- [ ] For queries with no single right answer: presents diverse experiences, perspectives or options.
- [ ] For product/category queries: supports browsing and research (options, photos, specs, reviews, comparisons).
- [ ] Estimated NM: FullyM / HM / MM / SM / FailsM, with reasons.

## Stage 4 · Special cases (pick what's relevant)

- **Reviews/affiliate:** proof of direct use or testing, evaluation criteria, honest pros and cons, own photos. "Best" lists that only summarize others' reviews = Low. (03, 05)
- **Programmatic SEO/mass AI content:** unique data per page, template QA (no blank sections), human editing, sampling several pages. (03, 04)
- **E-commerce:** complete product info, user reviews, customer service, return policy; consistent across all policy pages. (01, 06, 10)
- **Forums/UGC/comment sections:** moderate spam and abusive behavior; substantive answers; sponsored answers not disguised. (07)
- **Error/404/out-of-stock pages:** explanation, search, alternatives; make sure it's not a systemic problem. (07, 10)
- **Third-party/sponsored content:** relevant to the site and its readers, clearly labeled, not posing as an independent review. (03, 04)

---

## Audit report template

Use this structure (adjust length to the request):

**Summary:** one paragraph: page purpose, YMYL level, estimated PQ rating (and NM if there's a keyword), and the biggest issue.

**Red findings (Lowest risk):** each finding with evidence from the page and the SQRG section reference (e.g., "SQRG 4.6.6, p. 42"). If none, say "none found".

**Downgrading factors:** what makes the page Low or keeps it at Medium.

**Strengths:** what's already good and should be kept.

**Needs Met:** how well the page answers the target keyword, missed query aspects, and freshness or language issues.

**Fix priorities:** ordered by impact: (1) remove Lowest triggers, (2) fix accuracy and E-E-A-T for YMYL, (3) add original value, (4) clean up structure, filler, title and ads, (5) strengthen reputation signals.

**Honest note:** ratings are estimates based on rater standards, not ranking predictions. Also note what couldn't be checked (e.g., reputation needing external research, or content behind a login).
