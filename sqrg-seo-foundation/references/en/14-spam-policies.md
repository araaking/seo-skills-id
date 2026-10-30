# 14 · Google Search Spam Policies

> Source: **"Spam policies for Google web search"** (Google Search Central, developers.google.com/search/docs/essentials/spam-policies), page last updated **Aug 28, 2026**, checked Oct 2026. This is a **separate document from SQRG**: SQRG tells raters how to judge quality, while these policies define what Google's systems and manual actions treat as spam. Rewritten and condensed in our own words, not Google's text. Cite as "Spam policies › <section name>".
> **[Application]** = added notes for SEO/content practice, not part of the policy.
> SQRG's own treatment of spam is in `03-pq-lowest.md` section 7. Indonesian counterpart: `references/id/14-spam-policies.md`.

## Contents
1. Scope and consequences
2. Map to SQRG
3. Deceiving crawlers vs users: cloaking, sneaky redirects, hidden text and links
4. Manipulating query coverage: doorway abuse, keyword stuffing
5. Content without added value: scaled content abuse, scraping, thin affiliation
6. Borrowed authority: expired domain abuse, site reputation policy (with EEA changes)
7. Link spam
8. Security and user harm: hacked content, malicious practices, misleading functionality, user-generated spam
9. Machine-generated traffic
10. Other practices that can lead to demotion or removal
11. Implications for content creators and audits

---

## 1. Scope and consequences

- **Definition of spam:** techniques that deceive users or manipulate Google's systems into featuring content prominently. This now explicitly includes **attempts to manipulate generative AI responses in Google Search**, not just rankings.
- **Scope:** all web search results (pages, images, video, news and other content), including Google's own properties. Content must also follow Google Search's overall content policies.
- **Enforcement:** automated systems plus, when needed, human review that can lead to a **manual action**. Violating sites may rank lower or disappear from results.
- Users can report spam through a search quality user report; Google mainly uses these reports to improve automated detection.
- **The list isn't exhaustive.** Google may act against any spam practice it detects.

## 2. Map to SQRG

| Spam policy | Related SQRG section (file) |
|---|---|
| Expired domain abuse | 4.6.3 (`03` §7.3) |
| Site reputation policy | 4.6.4 (`03` §7.4) |
| Scaled content abuse | 4.6.5 (`03` §7.5) |
| Scraping | 4.6.6–4.6.7 (`03` §7.6, §8) |
| Hacked content, user-generated spam | 4.6.2 (`03` §7.2) |
| Hidden text | 4.5.4 (`03` §6.4) |
| Malicious practices, scam and fraud | 4.5.3, 4.5.5 (`03` §6.3, §6.5) |
| Misleading functionality | 4.5.3 deceptive purpose/design (`03` §6.3) |
| Thin affiliation | 4.5.3, 4.6.6 (`03` §6.3, §7.6); `05` |
| Cloaking, sneaky redirects, doorway, keyword stuffing, link spam, machine-generated traffic | Not covered in detail by SQRG; this file is the main reference |

## 3. Deceiving crawlers vs users

### 3.1 Cloaking
- **What it is:** serving search engines different content from what users see, to manipulate rankings and mislead users.
- Examples: crawlers get a travel page while users get a discount-drug page; keywords inserted only when the user agent is a search engine.
- **Not cloaking:** a paywall or gated content, **if** Google can see the full content the same way an entitled user can and the site follows Flexible Sampling guidance.
- Hard-to-crawl tech (JavaScript, images) should be made accessible to both, not "solved" by showing crawlers a different version.
- Hacked sites often use cloaking so owners don't notice the hack.

### 3.2 Sneaky redirects
- **What it is:** redirecting with intent to deceive: showing search engines and users different content, or sending users somewhere that doesn't meet their original need.
- Examples: crawlers see one page while users are redirected elsewhere; desktop users get the normal page while mobile users are sent to a spam domain.
- **Legitimate redirects:** moving a site, consolidating pages, sending logged-in users to an internal page.
- Test: is the redirect meant to deceive users or search engines?

### 3.3 Hidden text and link abuse
- **What it is:** placing content only for search engines, not easily visible to people.
- Examples: white text on white; text behind an image; CSS off-screen positioning; font size or opacity 0; a link on a single tiny character (e.g., a hyphen).
- **Fine (not a violation):** accordions/tabs, sliders/slideshows, tooltips shown on interaction, screen-reader-only text that improves accessibility.

## 4. Manipulating query coverage

### 4.1 Doorway abuse
- **What it is:** sites or pages built to rank for specific similar queries that lead users to intermediate pages less useful than the final destination.
- Examples: many sites with slight URL/home page variations; many domains or pages targeting cities/regions that all funnel to one page; pages generated to funnel visitors into the usable part of a site; near-identical pages that look more like search results than a browseable hierarchy.

### 4.2 Keyword stuffing
- **What it is:** filling a page with keywords or numbers to manipulate rankings, often as lists, out of context or unnaturally.
- Examples: lists of phone numbers with no real added value; blocks listing cities/regions the page wants to rank for; repeating the same phrase until it reads unnaturally.

## 5. Content without added value

### 5.1 Scaled content abuse
- **What it is:** generating many pages mainly to manipulate rankings rather than help users, typically unoriginal, low-value content, **no matter how it's created**.
- Examples: generative AI or similar tools producing many pages with no added value; scraping feeds/search results/other content into many pages, including via synonymizing, translating or other obfuscation; stitching content from different pages without adding value; spreading content over multiple sites to hide the scale; many pages that make little sense to readers but contain search keywords.
- If such content is hosted on your site, exclude it from Search.

### 5.2 Scraping
- **What it is:** taking content from other sites (often automatically) and hosting it to manipulate rankings.
- Examples: republishing without original content or value, sometimes without even citing the source; copying with light edits (synonym swaps, automated rewriting); reproducing feeds without unique benefit; sites that just embed or compile others' videos/images/media without substantial added value.

### 5.3 Thin affiliation
- **What it is:** pages with affiliate links where product descriptions and reviews are copied straight from the merchant, with no original content or value.
- Often part of programs distributing the same content across many affiliates: cookie-cutter templates repeated within a site or across domains and languages.
- **Being an affiliate isn't the problem.** Good affiliate pages add value: extra price info, original reviews, rigorous testing and ratings, product/category navigation, comparisons.

## 6. Borrowed authority

### 6.1 Expired domain abuse
- **What it is:** buying an expired domain and repurposing it mainly to manipulate rankings with content of little or no value.
- Examples: affiliate content on a former government agency domain; commercial medical products on a former non-profit medical charity domain; casino content on a former elementary school domain.

### 6.2 Site reputation policy
- **What it is:** third-party content published on a host site **mainly because of the host's established ranking signals** (earned from its first-party content), so it ranks better than it could on its own.
- **Third party** = an entity separate from the host: site users, freelancers, white-label services, people not directly employed by the host.
- **Third-party content alone is fine.** It's a problem only when the main reason for hosting it is to ride the host's ranking signals.

| Inconsistent with the policy | Not inconsistent |
|---|---|
| An education site hosting sponsored payday-loan reviews that a third party distributes to many sites | Wire services, press-release services |
| A medical site hosting a low-quality, non-integrated third-party "best casinos" ad page to exploit the host's signals | News publications carrying syndicated news |
| | Sites built for UGC (forums, comment sections) |
| | Columns, opinion pieces, articles and other editorial work |
| | Advertorials/native ads aimed at readers (e.g., promoted inside the publication), not at manipulating rankings |
| | Affiliate links treated properly (see §7); third-party ad units |

**How a human review judges integration** (applies globally). The question: was the content made with enough input, editorial oversight or contribution from the host to be fully integrated? Factors considered may include:
1. **Presentation:** design, formatting, typography and UX consistent with the host.
2. **Quality:** issues on the page that the main domain doesn't have.
3. **Authorship:** explicit ownership/responsibility for the content; any signs contradicting the stated authorship.
4. **Duplication:** identical or near-identical content on multiple other sites.

No single factor is necessary or sufficient on its own; other evidence can count too (e.g., pages being part of third-party ranking-manipulation material).

**Worked examples from the policy (paraphrased):**
- **Unlikely to act: integrated coupons section.** A publisher runs a deals section with a specialist partner (even on a different CMS) in a subfolder linked from the homepage and articles, organized into its own categories, clearly disclosed as commercial, with the publisher named as editorially responsible, cross-referenced in its editorial content/newsletters, and with an easy way to report bad codes.
- **Likely to act: unauthored, non-integrated affiliate article.** A major business publication hosts a CBD-oil marketplace article with no author or responsible editor, no commercial disclaimer, unreachable from the homepage or sections, and duplicating content from the third-party marketplace.
- **Unlikely to act: authored, original freelance affiliate content.** A news site's new cooking section by an identified freelancer interviewing chefs, under clear editorial responsibility and consistent branding. The freelancer writes for others too, but this selection is specific to the host; affiliate links are clearly marked.

**Consequences depend on the user's location** (changes announced Aug 2026):
- **Outside the EEA:** pages found inconsistent may receive a **manual action** in results shown to users outside the EEA.
- **Inside the EEA:** pages may be **categorized as separate from the main domain** and ranked on their own merits (e.g., casino content competes with other casino content), with **no manual-action impact**.
- Google normally presumes new and individual pages match the quality of the rest of the domain; separate categorization removes that presumption. The section doesn't instantly lose the main site's signals; systems learn over time to rank the parts independently. The categorization itself isn't a ranking signal.
- Affected sites are notified in the Search Console Manual actions report and message center, and can fix the issue or file a reconsideration request. In the EEA there's a faster reconsideration process with more detailed reasoning, and eligible sites can use mediation (alternative dispute resolution).
- **FAQ points:** a non-EEA manual action doesn't affect EEA rankings and isn't used as an EEA signal; `noindex` on content under a non-EEA manual action isn't required and not doing it isn't treated as circumvention; previous EEA manual actions under this policy are lifted and past actions aren't used as a ranking signal.

## 7. Link spam

**What it is:** creating links to or from a site mainly to manipulate rankings. Examples:
- Buying/selling links for ranking: money, goods or services for links or link-containing posts, including sending free products in exchange for a write-up with a link.
- Excessive link exchanges, or partner pages that exist just for cross-linking.
- Automated programs or services that create links.
- Requiring a link in terms of service or contracts without letting the content owner qualify (nofollow) the outbound link.
- Text ads or text links that don't block ranking credit.
- Paid advertorials/native ads with links that pass ranking credit, or keyword-optimized anchors in articles, guest posts or press releases distributed to other sites.
- Low-quality directory or bookmark links.
- Keyword-rich, hidden or low-quality links in widgets distributed across sites.
- Widely distributed links in footers or templates of various sites.
- Forum comments with optimized links in the post or signature.
- Low-value content created mainly to manipulate linking signals.

**Allowed:** paid links for advertising and sponsorship are normal, **as long as they're qualified** with `rel="sponsored"` or `rel="nofollow"` on the `<a>` tag.

## 8. Security and user harm

### 8.1 Hacked content
Content placed on a site without permission through security holes. Types:
- **Code injection:** malicious JavaScript in pages or iframes.
- **Page injection:** new spam or phishing pages added to the site; existing pages may look untouched.
- **Content injection:** subtle changes to existing pages, such as hidden links/text or cloaking.
- **Redirects:** injected code sending some users to harmful pages, often conditional on referrer, user agent or device (e.g., redirecting only visitors who come from Google results).

### 8.2 Malicious practices
Practices that create a gap between what users expect and what happens, hurting experience, security or privacy:
- **Malware:** software designed to harm devices or users. Owners sometimes host it without realizing.
- **Unwanted software:** deceptive or disruptive executables/apps, e.g., changing the home page or leaking personal data without disclosure.
- **Back button hijacking:** manipulating browser history so users can't go straight back to where they came from.

### 8.3 Misleading functionality
Sites that pretend to offer content or a service they don't deliver. Examples: a fake "app store credit generator"; a "PDF merge", timer or dictionary tool that actually funnels users to deceptive ads.

### 8.4 User-generated spam
Spam added by users through channels meant for user content, often without the owner noticing: spam accounts on open hosting services, spam forum posts, blog comment spam, spam files on file hosts.

## 9. Machine-generated traffic

Sending automated queries to Google without express permission, including **scraping search results for rank checking**. It violates the spam policies and Google's Terms of Service.

**[Application]** Relevant when choosing rank trackers and SERP tools: prefer official APIs or providers that operate within permitted access.

## 10. Other practices that can lead to demotion or removal

- **Legal removals:** a high volume of valid copyright removal requests can lead to demotion of other content on the same site. Similar signals apply to defamation, counterfeit goods and court-ordered removals. CSAM is always removed, and sites with a significant share of it are demoted.
- **Personal information removals:** sites with exploitative removal practices (e.g., charging to remove personal data) and a high volume of removals get demoted, and Google looks for the same pattern on other sites. Similar demotions can apply to doxxing content and non-consensual explicit imagery, including fake explicit content.
- **Policy circumvention:** continuing to violate via new or existing subdomains, subdirectories or sites, or other methods to keep distributing violating content. Possible consequences: losing eligibility for features such as Top Stories and Discover, and broader removal of site sections.
- **Scam and fraud:** impersonating official businesses or services, deliberately false business information, or luring users on false pretenses. Examples: imitating a well-known company so payments go to the wrong party; fake "official customer support" sites or fake contact details.

## 11. Implications for content creators and audits

**[Application]**
- **Spam policies vs SQRG:** SQRG describes quality judgment; spam policies describe what can trigger demotion or manual action. An audit should check both: SQRG for quality, this file for technical, link and distribution spam.
- **Programmatic and location pages:** city/region page sets must each offer real local value (actual service availability, local data, local proof). Templates that only swap the city name look like doorways and possibly scaled content abuse.
- **Paid and partnership links:** every sponsored post, product-for-review deal, partner placement and affiliate link should carry `rel="sponsored"` (or `nofollow`). Never request do-follow links as a condition of a deal.
- **Guest posts and press releases:** avoid keyword-rich anchors pointing back to money pages.
- **Third-party sections** (coupons, partner reviews, freelance content in new topics): integrate them into navigation, design and editorial responsibility; name the author and responsible editor; label commercial content; don't publish the same text the partner distributes elsewhere.
- **AI content:** the policy targets volume without value "no matter how it's created", and now explicitly covers manipulating generative AI answers. Don't build pages whose main purpose is to be picked up by AI Overviews/AI Mode without serving readers.
- **Technical audit checks:** compare what Googlebot gets vs what users get (URL Inspection, user-agent switching); test redirects on mobile and desktop and from Google referrals; look for hidden text/links in the DOM; check Search Console for Manual actions and Security issues.
- **Security and UGC:** monitor for injected pages (e.g., `site:` searches for odd URLs), moderate comments and forums, use `rel="ugc"`/`nofollow` on user links.
- **Rank tracking:** avoid tools that scrape Google without permission (machine-generated traffic).
