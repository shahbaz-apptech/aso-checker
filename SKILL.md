---
name: aso-metadata-validator
description: Validate and optimize Apple App Store (Title, Subtitle, Keyword List, Secondary Localizations, Apple Search Ads) and Google Play Store (Title, Short Description, Long Description) metadata against Appfigures ASO rules. Use whenever the user shares app store titles, subtitles, keyword lists, or descriptions and asks to validate, audit, check, or optimize their ASO metadata.
---

# ASO Metadata Validator & Optimizer (Portable Skill for Gemini, Claude & ChatGPT)

Validate and optimize mobile app metadata for the **Apple App Store** (App Name, Subtitle, 100-Character Keyword Field, Secondary Localizations, Apple Search Ads alignment) and **Google Play Store** (App Title, Short Description, Long Description) using the authoritative Appfigures ASO rulebook.

---

## Reference Registry (Mandatory Citations)

Whenever you apply, pass, warn, or fail a rule during validation, you **MUST** state:
1. **Rule Number & Title**
2. **Article Reference (Title + URL)**
3. **Publication / Update Date**

### Stored Source Links:
1. **Ref 1:** [ASO Strategy: Improving App Store Page Conversion by Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) | **Date:** Jun 17
2. **Ref 2:** [8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) | **Date:** Jun 17
3. **Ref 3:** [9 Common ASO Mistakes That Hurt Your Downloads](https://appfigures.com/resources/guides/common-aso-mistakes) | **Date:** Jun 17
4. **Ref 4:** [ASO Checklist 2026: App Store Optimization Steps (with Examples)](https://appfigures.com/resources/guides/app-store-optimization-checklist) | **Date:** Jun 24 (2026 Edition)
5. **Ref 5:** [How to Improve Your ASO by Analyzing Your Competitors' Keywords](https://appfigures.com/resources/guides/competitor-keyword-analysis) | **Date:** Jun 24
6. **Ref 6:** [App Store Optimization (ASO): The Complete Guide for 2026](https://appfigures.com/resources/guides/app-store-optimization) | **Date:** Jun 24 (2026 Edition)
7. **Ref 7:** [App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) | **Date:** Jun 29
8. **Ref 8:** [How to Choose ASO Keywords That Drive Downloads on the App Store & Google Play](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) | **Date:** Jun 29
9. **Ref 9:** [ASO Keyword Research: 9 Steps for the App Store & Google Play](https://appfigures.com/resources/guides/keyword-research) | **Date:** Jun 29
10. **Ref 10:** [13 Ways to Promote Your App and Get More Downloads](https://appfigures.com/resources/guides/13-ways-to-promote-your-mobile-app) | **Date:** Jun 29
11. **Ref 11:** [How to 10x Your App Store Keyword List with Secondary Localizations](https://appfigures.com/resources/guides/extend-keyword-list) | **Date:** Jun 29 (Table Updated Apr 25, 2023)
12. **Ref 12:** [Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) | **Date:** Jun 29
13. **Ref 13:** [Optimizing Your Apple Search Ads Campaign](https://appfigures.com/resources/guides/optimizing-your-apple-search-ads-campaign) | **Date:** Jun 29

---

## The 18-Rule ASO Validation Rulebook
*(Note: Where multiple articles covered the same concept, the latest article rule has been selected as authoritative.)*

### Section A: App Name / Title & Subtitle / Short Description

* **Rule 1: Strict Character Limits**
  * **iOS App Store:** App Name max **30 characters**; Subtitle max **30 characters**.
  * **Google Play Store:** App Name max **30 characters** (Google Play Console limit) / **50 characters** (Appfigures guide limit — flag a warning if >30 and a hard fail if >50); Short Description max **80 characters**.
  * **Reference:** Ref 7 ([App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) — Jun 29) & Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) — Jun 24, 2026).

* **Rule 2: iOS Special Character Truncation Bug (`&` Bug)**
  * Do **not** use all 30 characters in the iOS App Name or Subtitle if the text includes special characters like `&`. The App Store search algorithm counts special characters like `&` as **2 characters**, causing the 30th character to be dropped/ignored during indexing. Either avoid special characters or leave at least 1-2 characters of buffer per special character (max 28-29 chars).
  * **Reference:** Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29).

* **Rule 3: Left-to-Right Weighting & Brand vs. Keyword Placement**
  * Search algorithms read left-to-right and assign the highest ranking weight to words appearing **earliest** in the App Name, Subtitle, and Short Description.
  * Never leave the App Name "clean" (brand-only). Always combine the brand name with a 3-5 word descriptive keyword phrase separated by `:` or `-`.
  * If the brand is new or not heavily searched by name, place the primary target keyword **first** (before the brand name). Put the brand first only if users actively search for the brand name.
  * **Reference:** Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29) & Ref 7 ([App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) — Jun 29).

* **Rule 4: Do Not Split or Reverse Multi-Word Keywords**
  * Keep primary multi-word target keywords contiguous (together) and in their exact word order. Splitting a multi-word keyword reduces relevance weight, and reversing the order (e.g., `"analytics app"` vs `"app analytics"`) is treated as a different search query by the algorithm and ranks lower.
  * **Reference:** Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29).

* **Rule 5: Thematic Focus Over Keyword Stuffing in Name & Subtitle**
  * Do not stuff multiple unrelated keyword themes into the App Name and Subtitle just to fill all 30 characters (mixing unrelated themes confuses the algorithm and dilutes rank). Focus the App Name on the #1 core keyword theme, and use the Subtitle to **extend** that exact theme with natural modifiers in a human-readable 3-5 word phrase.
  * **Reference:** Ref 7 ([App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) — Jun 29) & Ref 1 ([ASO Strategy: Improving App Store Page Conversion by Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) — Jun 17).

* **Rule 6: No Competitor Brand Names or Third-Party Trademarks**
  * Never include competitor names or third-party trademarks in your metadata. Users searching a specific brand download that brand; ranking below them drives zero downloads and violates store policy.
  * **Reference:** Ref 8 ([How to Choose ASO Keywords That Drive Downloads on the App Store & Google Play](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) — Jun 29) & Ref 1 ([ASO Strategy: Improving App Store Page Conversion by Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) — Jun 17).

---

### Section B: iOS App Store Keyword Field (100-Character Field)

* **Rule 7: Zero Duplication Penalty Across Name, Subtitle, and Keyword Field**
  * **Never repeat any word** within the 100-character Keyword List, OR across the App Name, Subtitle, and Keyword List within the same localization. Since 2022+, duplicating keywords across fields wastes character space and **actively penalizes/devalues** the weight of those keywords.
  * **Reference:** Ref 8 ([How to Choose ASO Keywords That Drive Downloads on the App Store & Google Play](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) — Jun 29, Updated for 2022+).

* **Rule 8: Single Words Only, Comma-Separated, Zero Spaces**
  * Split all multi-word search phrases into single words separated strictly by commas with **zero spaces** (e.g., `buy,shoe,sneaker,shop,accessories`). Never enter spaces after commas or full phrases, as Apple automatically combines individual words within the same localization.
  * **Reference:** Ref 4 ([ASO Checklist 2026: App Store Optimization Steps](https://appfigures.com/resources/guides/app-store-optimization-checklist) — Jun 24, 2026) & Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) — Jun 17).

* **Rule 9: Left-to-Right Priority in Keyword Field**
  * The algorithm assigns more weight to words at the **beginning** of the 100-character keyword list than words at the end. Place your highest-priority extension keywords first and lower-competition/long-tail modifiers toward the end.
  * **Reference:** Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29) & Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) — Jun 17).

* **Rule 10: Do Not Pluralize Words in English**
  * Do not include both singular and plural forms (or unnecessary plural words) in an English keyword list. Prefer the singular form (e.g., `sneaker` instead of `sneakers`), as Apple's search algorithm handles pluralization automatically.
  * **Reference:** Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) — Jun 17).

* **Rule 11: Eliminate All Apple Stop Words**
  * Strip all generic stop words that Apple ignores from the 100-character Keyword List:
    `a, about, above, after, again, against, all, am, an, and, any, app, are, aren't, as, at, be, because, been, before, being, below, between, both, but, by, can't, cannot, could, couldn't, did, didn't, do, does, doesn't, doing, don't, down, during, each, few, for, from, further, had, hadn't, has, hasn't, have, haven't, having, he, he'd, he'll, he's, her, here, here's, hers, herself, him, himself, his, how, how's, i, i'd, i'll, i'm, i've, if, in, into, is, isn't, it, it's, its, itself, let's, me, more, most, mustn't, my, myself, no, nor, not, of, off, on, once, only, or, other, ought, our, ours, ourselves, out, over, own, same, shan't, she, she'd, she'll, she's, should, shouldn't, so, some, such, than, that, that's, the, their, theirs, them, themselves, then, there, there's, these, they, they'd, they'll, they're, they've, this, those, through, to, too, under, until, up, very, was, wasn't, we, we'd, we'll, we're, we've, were, weren't, what, what's, when, when's, where, where's, which, while, who, who's, whom, why, why's, with, won't, would, wouldn't, you, you'd, you'll, you're, you've, your, yours, yourself, yourselves`
  * **Reference:** Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) — Jun 17).

* **Rule 12: Exclude App Name, Company Name, and Category Name**
  * Never include your own App Name, Developer/Company Name, or primary App Store Category name in the 100-character keyword list. Apple indexes those automatically.
  * **Reference:** Ref 4 ([ASO Checklist 2026: App Store Optimization Steps](https://appfigures.com/resources/guides/app-store-optimization-checklist) — Jun 24, 2026) & Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) — Jun 17).

* **Rule 13: Simplify Complex Words & Maximize 100 Characters Wisely**
  * Replace complicated/long words with shorter, simpler words users actually type. Aim to use close to 100 characters with relevant extension words, provided they do not dilute focus from your primary keywords.
  * **Reference:** Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) — Jun 17).

* **Rule 14: Secondary Localization Keyword Isolation**
  * When adding secondary localizations in App Store Connect to multiply 100-character keyword fields (e.g., US Store indexes English US + Spanish Mexico, Arabic, Chinese Simplified, Chinese Traditional, French, Korean, Portuguese Brazil, Russian, Vietnamese): **Apple does NOT combine keywords across different localizations**. Words in a secondary localization only combine with words inside that *same* localization's Name, Subtitle, and Keyword list.
  * **Reference:** Ref 11 ([How to 10x Your App Store Keyword List with Secondary Localizations](https://appfigures.com/resources/guides/extend-keyword-list) — Jun 29 / Updated Apr 25, 2023).

---

### Section C: Google Play Store Long Description

* **Rule 15: Long Description Length, Early Placement, & 3%-5% Keyword Density**
  * **Character Limit:** Up to **4,000 characters**.
  * **Top-to-Bottom Weighting:** Google reads top-to-bottom and assigns the highest weight to keywords appearing **earliest** (in the opening sentences/first paragraph) of the long description.
  * **Keyword Density & Frequency:** Focus on 3-5 core keywords (up to 5-10 total targets). Aim for a **3% to 5% keyword density** for top keywords (`(keyword_count / total_word_count) * 100`), repeating and varying each main keyword at least **5 times** in a full-length description.
    * **< 3% density:** Keywords become invisible to Google's algorithm.
    * **> 5% density:** Google treats the description as keyword stuffing/spam.
  * **Reference:** Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29), Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) — Jun 24, 2026), & Ref 3 ([9 Common ASO Mistakes That Hurt Your Downloads](https://appfigures.com/resources/guides/common-aso-mistakes) — Jun 17).

* **Rule 16: Separate iOS vs. Google Play Strategy**
  * Never copy-paste the same metadata strategy between the App Store and Google Play. Apple uses Name + Subtitle + 100-char Keyword List (zero repetition), while Google uses Name + Short Description + Long Description (requires 3%-5% repetition density) and also indexes keywords found inside user reviews.
  * **Reference:** Ref 6 ([App Store Optimization (ASO): The Complete Guide for 2026](https://appfigures.com/resources/guides/app-store-optimization) — Jun 24, 2026), Ref 12 ([Advanced ASO Tips](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29), & Ref 3 ([9 Common ASO Mistakes](https://appfigures.com/resources/guides/common-aso-mistakes) — Jun 17).

---

### Section D: Keyword Selection & Apple Search Ads Alignment

* **Rule 17: Popularity Floor (>=10), 3-Word Long-Tails, & Keyword Opportunities**
  * Avoid single-digit popularity keywords (Popularity Score < 10). Target 3-to-4 word long-tail keywords with high popularity and low competition, and prioritize "Keyword Opportunities" (keywords where current top 5-10 results do not have the exact unbroken keyword in their App Name) by placing that exact phrase first in your App Name.
  * **Reference:** Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) — Jun 29), Ref 8 ([How to Choose ASO Keywords That Drive Downloads](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) — Jun 29), & Ref 9 ([ASO Keyword Research: 9 Steps](https://appfigures.com/resources/guides/keyword-research) — Jun 29).

* **Rule 18: Apple Search Ads to Organic ASO Bridge & Exact Negative Keywords**
  * **Paid-to-Organic Harvesting:** Identify paid keywords that competitors bid on where your app already ranks organically **below #10** (or high-popularity, low-competition paid keywords) and move them into your organic metadata (Name, Subtitle, Keyword List) to earn those downloads for free.
  * **Pause Ads on High Organic Ranks:** Check organic rank for paid keywords and stop spending ad budget on keywords where you already rank at the top organically.
  * **Exact Match Negative Keywords:** When using Search Match or Broad Match in Apple Ads, block irrelevant terms as Negative Keywords wrapped in **exact match brackets `[keyword]`**.
  * **Seasonal Extremes Strategy:** For seasonal trends, target the highest-popularity head terms and the lowest-popularity cheap long-tail terms, skipping the overpriced middle tier.
  * **Reference:** Ref 13 ([Optimizing Your Apple Search Ads Campaign](https://appfigures.com/resources/guides/optimizing-your-apple-search-ads-campaign) — Jun 29).

---

## Step-by-Step Validation Instructions for the AI

When the user provides any combination of App Store (Title, Subtitle, Keyword Field) or Google Play (Title, Short Description, Long Description) metadata:

1. **Exact Measurements First:**
   * Count exact characters (including spaces and punctuation) for every provided field.
   * Tokenize all words in iOS Title, Subtitle, and Keyword List to check for:
     * Intra-field or cross-field duplicate words (Rule 7)
     * Spaces after commas or multi-word entries in Keyword List (Rule 8)
     * Plurals (Rule 10) and Apple Stop Words (Rule 11)
     * Special characters (`&`) near the 30-character boundary (Rule 2)
   * For Google Play Long Descriptions:
     * Count total words and total characters.
     * Calculate exact frequency and percentage density (`(keyword_occurrences / total_words) * 100%`) for the top 3-5 target keywords (Rule 15).
     * Check if primary keywords appear in the first sentence/paragraph (Rule 15).

2. **Output a Citation-Backed Validation Report:**
   * Present a clear table or bulleted audit checking each relevant rule.
   * **Every single finding MUST explicitly include:**
     * **Status:** `PASS`, `WARN`, or `FAIL`
     * **Rule Number & Name:** e.g., `Rule 7: Zero Duplication Penalty`
     * **Article Reference & URL:** e.g., `[How to Choose ASO Keywords That Drive Downloads](https://appfigures.com/resources/guides/which-keywords-to-optimize-for)`
     * **Date:** e.g., `Jun 29`
     * **Specific Evidence:** Show the exact offending word, character count, or density percentage.

3. **Provide Ready-to-Use Optimized Metadata:**
   * Rewrite any failed or suboptimal fields so they pass 100% of the rules above.
   * Display the final character count (e.g., `28/30 chars`, `99/100 chars`) and keyword density % alongside the rewritten fields.
