---
name: google-play-aso-validator
description: Validate and optimize Google Play Store metadata (App Title, Short Description, and Long Description keyword density) against Appfigures ASO rules. Use whenever the user shares Google Play titles, short descriptions, or long descriptions and asks to audit, validate, or optimize their Android ASO.
---

# Google Play Store ASO Validator & Keyword Density Optimizer

Validate and optimize Google Play Store metadata (**App Name / Title**, **Short Description**, and **Long Description**) using the authoritative Appfigures ASO rulebook.

## Mandatory Citation Rule

Every time you apply, pass, warn, or fail a rule, you **MUST** explicitly cite:
- **Rule Number & Title**
- **Article Title & URL**
- **Article Date**

### Stored Reference Registry:
- **Ref 1:** [ASO Strategy: Improving App Store Page Conversion by Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) | **Date:** Jun 17
- **Ref 3:** [9 Common ASO Mistakes That Hurt Your Downloads](https://appfigures.com/resources/guides/common-aso-mistakes) | **Date:** Jun 17
- **Ref 4:** [ASO Checklist 2026: App Store Optimization Steps (with Examples)](https://appfigures.com/resources/guides/app-store-optimization-checklist) | **Date:** Jun 24 (2026 Edition)
- **Ref 5:** [How to Improve Your ASO by Analyzing Your Competitors' Keywords](https://appfigures.com/resources/guides/competitor-keyword-analysis) | **Date:** Jun 24
- **Ref 6:** [App Store Optimization (ASO): The Complete Guide for 2026](https://appfigures.com/resources/guides/app-store-optimization) | **Date:** Jun 24 (2026 Edition)
- **Ref 7:** [App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) | **Date:** Jun 29
- **Ref 8:** [How to Choose ASO Keywords That Drive Downloads on the App Store & Google Play](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) | **Date:** Jun 29
- **Ref 9:** [ASO Keyword Research: 9 Steps for the App Store & Google Play](https://appfigures.com/resources/guides/keyword-research) | **Date:** Jun 29
- **Ref 12:** [Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) | **Date:** Jun 29

---

## Google Play Validation Rules (Latest Rule Takes Precedence)

- **Rule 1 (Strict Character Limits):**
  - **Google Play App Name:** Max **30 characters** (Google Play Console policy limit) / **50 characters** (Appfigures guide limit — flag a `WARN` if 31-50 chars and `FAIL` if >50 chars).
  - **Google Play Short Description:** Max **80 characters**.
  - **Google Play Long Description:** Max **4,000 characters**.
  - *Citation:* Ref 7 ([App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) - Jun 29) & Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) - Jun 24, 2026).

- **Rule 2 (Left-to-Right & Top-to-Bottom Weighting):**
  - Google's algorithm reads **left-to-right** in the App Name and Short Description, and **top-to-bottom** in the Long Description, assigning the highest weight to words it reads **first**.
  - Place your #1 target keyword as early as possible in the App Name, at the start of the Short Description, and in the **opening sentence/first paragraph** of the Long Description.
  - If the brand is new or not widely searched by name, place the primary keyword **before** the brand name in the App Title. Never leave the App Title "clean" (brand-only).
  - *Citation:* Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29) & Ref 7 ([App Name ASO](https://appfigures.com/resources/guides/app-name-optimization) - Jun 29).

- **Rule 3 (Keep Multi-Word Keywords Contiguous & In Exact Order):**
  - Do not split primary multi-word target keywords or reverse their word order (e.g., `"app analytics"` != `"analytics app"`). Splitting or reversing reduces relevance and ranking power.
  - *Citation:* Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29).

- **Rule 4 (Focus Short Description on Core Keywords Without Stuffing):**
  - Focus the 80-character Short Description on your top 3-5 primary keywords in a compelling, human-readable sentence rather than stuffing unrelated words, which dilutes the strength of your main keywords.
  - *Citation:* Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) - Jun 24, 2026) & Ref 3 ([9 Common ASO Mistakes](https://appfigures.com/resources/guides/common-aso-mistakes) - Jun 17).

- **Rule 5 (Long Description 3% to 5% Keyword Density & 5x Minimum Repetition):**
  - Google Play does not have a keyword list field; it indexes your Long Description by looking for words that repeat most frequently.
  - Focus on **3 to 5 primary keywords** (up to 5-10 total targets).
  - **Density Target:** Maintain a **3% to 5% keyword density** (`(keyword_count / total_words) * 100%`) for your top 3-5 keywords, repeating and varying each primary keyword **at least 5 times** across a full-length description.
    - **< 3% density:** Keywords become invisible to Google's algorithm.
    - **> 5% density:** Google penalizes/flags the description as keyword stuffing/spam.
  - *Citation:* Ref 3 ([9 Common ASO Mistakes That Hurt Your Downloads](https://appfigures.com/resources/guides/common-aso-mistakes) - Jun 17) & Ref 4 ([ASO Checklist 2026](https://appfigures.com/resources/guides/app-store-optimization-checklist) - Jun 24, 2026).

- **Rule 6 (No Competitor Brand Names or Trademarks):**
  - Never include competitor names or third-party trademarks in your Title, Short Description, or Long Description.
  - *Citation:* Ref 8 ([How to Choose ASO Keywords That Drive Downloads](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) - Jun 29).

- **Rule 7 (Google Play Specific Algorithm Signals & Review Indexing):**
  - Never copy-paste an iOS strategy onto Google Play. Unlike Apple, Google indexes **keywords inside user reviews** and ranks apps based on all-time downloads, uninstalls, and crash rates. Ensure relevant keywords that users naturally mention in 4-5 star reviews are reinforced in your Long Description.
  - *Citation:* Ref 12 ([Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29), Ref 9 ([ASO Keyword Research](https://appfigures.com/resources/guides/keyword-research) - Jun 29), & Ref 3 ([9 Common ASO Mistakes](https://appfigures.com/resources/guides/common-aso-mistakes) - Jun 17).

- **Rule 8 (Popularity Floor >= 10 & Keyword Opportunities):**
  - Avoid single-digit popularity keywords (Popularity < 10). Prioritize 3-word long-tail keywords with high popularity and low competition, and target "Keyword Opportunities" where current top results omit the exact unbroken keyword from their App Title.
  - *Citation:* Ref 12 ([Advanced ASO Tips](https://appfigures.com/resources/guides/advanced-aso-secrets) - Jun 29) & Ref 8 ([How to Choose ASO Keywords](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) - Jun 29).

---

## Output Format

1. **Exact Character & Keyword Density Math:**
   - Show exact character counts (`Title: X/30`, `Short Desc: X/80`, `Long Desc: X/4000`) and total word count.
   - Provide a **Keyword Density Table** showing each target keyword, exact occurrence count, and exact `% density` (`(count / total_words) * 100%`).
2. **Rule-by-Rule Audit Table:** State `PASS`, `WARN`, or `FAIL` with the exact **Rule #**, **Article Title + URL**, **Date**, and **Specific Finding**.
3. **Ready-to-Paste Optimized Google Play Metadata:** Provide the corrected Title, Short Description, and Long Description hitting the exact 3%–5% density sweet spot.
