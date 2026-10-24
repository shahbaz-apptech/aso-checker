---
name: ios-app-store-aso-validator
description: Validate and optimize Apple App Store metadata (App Name, Subtitle, 100-Character Keyword Field, Secondary Localizations, and Apple Search Ads keywords) against Appfigures ASO rules. Use whenever the user shares iOS App Store titles, subtitles, keyword lists, or Apple Search Ads keywords for validation or optimization.
---

# iOS App Store & Apple Search Ads ASO Validator

Validate and optimize Apple App Store metadata (**App Name**, **Subtitle**, **100-Character Keyword Field**, **Secondary Localizations**, and **Apple Search Ads** keyword lists) using the authoritative Appfigures ASO rulebook.

## Mandatory Citation Rule

Every time you apply, pass, warn, or fail a rule, you **MUST** explicitly cite:
- **Rule Number & Title**
- **Article Title & URL**
- **Article Date**

### Stored Reference Registry:
- **Ref 1:** [ASO Strategy: Improving App Store Page Conversion by Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) | **Date:** Jun 17
- **Ref 2:** [8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) | **Date:** Jun 17
- **Ref 3:** [9 Common ASO Mistakes That Hurt Your Downloads](https://appfigures.com/resources/guides/common-aso-mistakes) | **Date:** Jun 17
- **Ref 4:** [ASO Checklist 2026: App Store Optimization Steps (with Examples)](https://appfigures.com/resources/guides/app-store-optimization-checklist) | **Date:** Jun 24 (2026 Edition)
- **Ref 5:** [How to Improve Your ASO by Analyzing Your Competitors' Keywords](https://appfigures.com/resources/guides/competitor-keyword-analysis) | **Date:** Jun 24
- **Ref 6:** [App Store Optimization (ASO): The Complete Guide for 2026](https://appfigures.com/resources/guides/app-store-optimization) | **Date:** Jun 24 (2026 Edition)
- **Ref 7:** [App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) | **Date:** Jun 29
- **Ref 8:** [How to Choose ASO Keywords That Drive Downloads on the App Store & Google Play](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) | **Date:** Jun 29
- **Ref 9:** [ASO Keyword Research: 9 Steps for the App Store & Google Play](https://appfigures.com/resources/guides/keyword-research) | **Date:** Jun 29
- **Ref 11:** [How to 10x Your App Store Keyword List with Secondary Localizations](https://appfigures.com/resources/guides/extend-keyword-list) | **Date:** Jun 29 (Updated Apr 25, 2023)
- **Ref 12:** [Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) | **Date:** Jun 29
- **Ref 13:** [Optimizing Your Apple Search Ads Campaign](https://appfigures.com/resources/guides/optimizing-your-apple-search-ads-campaign) | **Date:** Jun 29

---

## iOS Validation Rules (Latest Rule Takes Precedence)

### Part 1: iOS App Name & Subtitle Rules

- **Rule 1 (30-Character Hard Limit):**
  - iOS App Name max **30 characters**; iOS Subtitle max **30 characters**.
  - *Citation:* Ref 7 ([App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) - Jun 29).

- **Rule 2 (Special Character `&` Truncation Bug):**
  - Never use all 30 characters in the iOS App Name or Subtitle if the field contains special characters like `&`. Apple's search algorithm counts special characters like `&` as **2 characters**, silently dropping the 30th character from indexing. Avoid `&` or leave 1-2 buffer characters per special character (max 28-29 characters).
  - *Citation:* Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29).

- **Rule 3 (Left-to-Right Priority & Brand vs. Keyword Placement):**
  - Apple reads left-to-right and gives the highest ranking weight to words appearing **earliest** in the Name and Subtitle.
  - Never leave the App Name "clean" (brand-only). Combine the brand name with a 3-5 word descriptive keyword phrase separated by `:` or `-`.
  - If the brand is new or not widely searched by name, place the primary keyword **before** the brand name (Keyword First).
  - *Citation:* Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29) & Ref 7 ([App Name ASO](https://appfigures.com/resources/guides/app-name-optimization) - Jun 29).

- **Rule 4 (Keep Multi-Word Keywords Contiguous & In Exact Order):**
  - Do not split primary multi-word keywords across words/fields if avoidable, and **never reverse their word order** (e.g., `"app analytics"` != `"analytics app"`). Splitting or reversing lowers relevance weight.
  - *Citation:* Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29).

- **Rule 5 (Single Theme Focus in Name & Subtitle Extension):**
  - Do not cram unrelated keyword themes into the Name and Subtitle just to hit 30 characters (mixing themes confuses the algorithm). Focus the App Name on the #1 core keyword theme, and use the Subtitle to **extend** that exact theme with modifiers in a human-readable 3-5 word sentence.
  - *Citation:* Ref 7 ([App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) - Jun 29) & Ref 1 ([ASO Strategy: Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) - Jun 17).

- **Rule 6 (No Competitor Brand Names or Trademarks):**
  - Never include competitor names or third-party trademarks in Name, Subtitle, or Keywords.
  - *Citation:* Ref 8 ([How to Choose ASO Keywords That Drive Downloads](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) - Jun 29).

### Part 2: iOS 100-Character Keyword Field Rules

- **Rule 7 (Zero Cross-Field & Intra-Field Duplication Penalty):**
  - **Never repeat any word** inside the 100-character Keyword List, OR across the App Name, Subtitle, and Keyword List within the same localization. Since 2022+, duplicating keywords across Name, Subtitle, and Keyword List wastes characters and **actively penalizes/devalues** ranking weight.
  - *Citation:* Ref 8 ([How to Choose ASO Keywords That Drive Downloads](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) - Jun 29, Updated for 2022+).

- **Rule 8 (Single Words Only, Comma-Separated, Zero Spaces):**
  - Split all multi-word phrases into individual single words separated strictly by commas with **no spaces** (`buy,shoe,sneaker,shop,accessories`). Apple automatically combines single words within the same localization.
  - *Citation:* Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) - Jun 24, 2026) & Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) - Jun 17).

- **Rule 9 (Early Placement Priority in Keyword Field):**
  - Place the highest-priority single keywords at the **very beginning** of the 100-character keyword list, and lower-competition/long-tail modifiers toward the end.
  - *Citation:* Ref 12 ([Advanced ASO Tips](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29) & Ref 2 ([8 Tips to Optimize Your Keywords List](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) - Jun 17).

- **Rule 10 (No Plurals in English):**
  - Do not include both singular and plural variants (prefer singular, e.g., `sneaker` instead of `sneakers`), as Apple's search algorithm handles pluralization automatically.
  - *Citation:* Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) - Jun 17).

- **Rule 11 (Strip All Apple Stop Words):**
  - Remove all generic stop words that Apple ignores from the 100-character Keyword List:
    `a, about, above, after, again, against, all, am, an, and, any, app, are, aren't, as, at, be, because, been, before, being, below, between, both, but, by, can't, cannot, could, couldn't, did, didn't, do, does, doesn't, doing, don't, down, during, each, few, for, from, further, had, hadn't, has, hasn't, have, haven't, having, he, he'd, he'll, he's, her, here, here's, hers, herself, him, himself, his, how, how's, i, i'd, i'll, i'm, i've, if, in, into, is, isn't, it, it's, its, itself, let's, me, more, most, mustn't, my, myself, no, nor, not, of, off, on, once, only, or, other, ought, our, ours, ourselves, out, over, own, same, shan't, she, she'd, she'll, she's, should, shouldn't, so, some, such, than, that, that's, the, their, theirs, them, themselves, then, there, there's, these, they, they'd, they'll, they're, they've, this, those, through, to, too, under, until, up, very, was, wasn't, we, we'd, we'll, we're, we've, were, weren't, what, what's, when, when's, where, where's, which, while, who, who's, whom, why, why's, with, won't, would, wouldn't, you, you'd, you'll, you're, you've, your, yours, yourself, yourselves`
  - *Citation:* Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) - Jun 17).

- **Rule 12 (Exclude Own App Name, Developer Name, and Category Name):**
  - Never include your own App Name, Company/Developer Name, or primary App Store Category name in the 100-character keyword list. Apple indexes them automatically.
  - *Citation:* Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) - Jun 24, 2026) & Ref 2 ([8 Tips to Optimize Your Keywords List](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) - Jun 17).

- **Rule 13 (Simplify Complex Words & Use Close to 100 Characters Wisely):**
  - Replace complicated/long words with simpler, casual terms users actually type. Aim to use close to 100 characters with relevant extension words unless adding filler dilutes focus from core keywords.
  - *Citation:* Ref 2 ([8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) - Jun 17).

- **Rule 14 (Secondary Localization Keyword Isolation):**
  - When using secondary localizations (e.g., in the US store: Spanish Mexico, Arabic, Chinese Simplified/Traditional, French, Korean, Portuguese Brazil, Russian, Vietnamese) for extra 100-character keyword fields: **Apple does NOT combine keywords across different localizations**. Words in a secondary localization only combine with words inside that *same* localization's Name, Subtitle, and Keyword field.
  - *Citation:* Ref 11 ([How to 10x Your App Store Keyword List with Secondary Localizations](https://appfigures.com/resources/guides/extend-keyword-list) - Jun 29 / Updated Apr 25, 2023).

### Part 3: Keyword Selection & Apple Search Ads Rules

- **Rule 15 (Popularity >= 10, 3-Word Long-Tails, & Keyword Opportunities):**
  - Avoid single-digit popularity keywords (Popularity < 10). Target 3-to-4 word long-tail terms with high popularity and low competition, and prioritize "Keyword Opportunities" (where top 5-10 results lack the exact unbroken keyword in their App Name) by placing that exact phrase first in your App Name.
  - *Citation:* Ref 12 ([Advanced ASO Tips](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29), Ref 8 ([How to Choose ASO Keywords](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) - Jun 29), & Ref 9 ([ASO Keyword Research](https://appfigures.com/resources/guides/keyword-research) - Jun 29).

- **Rule 16 (Apple Search Ads to Organic ASO Bridge & Exact Negative Keywords):**
  - **Paid-to-Organic Harvesting:** Take paid keywords that competitors bid on where your app already ranks organically **below #10** (or high-popularity, low-competition paid keywords) and move them into your organic metadata (Name, Subtitle, Keyword List).
  - **Pause Ads on High Organic Ranks:** Stop spending ad budget on keywords where your app already ranks at the very top organically.
  - **Exact Match Negative Keywords:** When using Search Match or Broad Match in Apple Ads, block irrelevant terms as Negative Keywords wrapped in **exact match brackets `[keyword]`**.
  - **Seasonal Extremes Strategy:** For seasonal trends, target the highest-popularity head terms and the lowest-popularity cheap long-tail terms, skipping the expensive middle tier.
  - *Citation:* Ref 13 ([Optimizing Your Apple Search Ads Campaign](https://appfigures.com/resources/guides/optimizing-your-apple-search-ads-campaign) - Jun 29).

---

## Output Format

1. **Exact Character & Token Count Summary:** Show exact character counts (`X/30`, `X/30`, `X/100`) and list all detected duplicate words, stop words, plurals, or spaces.
2. **Rule-by-Rule Audit Table:** State `PASS`, `WARN`, or `FAIL` with the exact **Rule #**, **Article Title + URL**, **Date**, and **Specific Finding**.
3. **Ready-to-Paste Optimized iOS Metadata:** Provide the corrected App Name, Subtitle, and 100-char Keyword List with exact character counts verified.
