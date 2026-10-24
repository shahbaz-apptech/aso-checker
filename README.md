# ASO Metadata Validator Agent Skills (`npx skills` Ready)

Validate and optimize **Apple App Store** (Title, Subtitle, 100-Char Keyword Field, Secondary Localizations, Apple Search Ads) and **Google Play Store** (Title, Short Description, Long Description Keyword Density) metadata against 18 data-backed rules from Appfigures ASO guides (2026 Edition).

Every validation audit outputs:
- **Pass / Warn / Fail Status**
- **Exact Rule Number & Title**
- **Article Title, URL, and Publication Date**
- **Exact character counts, duplicate token checks, 175+ Apple stop-word filtering, and 3%–5% keyword density math**

---

## Quick Install via `npx skills` (Claude Code, Gemini CLI, Cursor, Codex, Windsurf)

This repository follows the official **Agent Skills Specification** (`skills/<skill-name>/SKILL.md`), so anyone can install it directly from GitHub with a single `npx` command:

### 1. Install All ASO Skills (Interactive)
```bash
npx skills add shahbaz-apptech/aso-checker
```

### 2. Install Only a Specific Modular Skill
```bashS
# Install ONLY the iOS App Store & Apple Ads Validator
npx skills add shahbaz-apptech/aso-checker --skill ios-app-store-aso-validator

# Install ONLY the Google Play & Keyword Density Validator
npx skills add shahbaz-apptech/aso-checker --skill google-play-aso-validator

# Install the combined All-in-One Validator
npx skills add shahbaz-apptech/aso-checker --skill aso-metadata-validator
```

### 3. Install Globally for All Projects
```bash
npx skills add shahbaz-apptech/aso-checker --all --global
```

### 4. List Available Skills in This Repo
```bash
npx skills add shahbaz-apptech/aso-checker --list
```

---

## Repository Layout (Required for `npx skills` Discovery)

For `npx skills add` to detect each skill automatically, every skill folder name inside `skills/` **must exactly match** the `name:` field in its `SKILL.md` frontmatter, and the file inside must be named `SKILL.md`:

```text
aso-checker/
├── README.md
├── package.json                                  # Optional npm / skills pack manifest
├── SKILL.md                                      # Root entry point (All-in-One skill)
└── skills/
    ├── aso-metadata-validator/
    │   └── SKILL.md                              # Combined iOS + Google Play (18 Rules)
    ├── ios-app-store-aso-validator/
    │   └── SKILL.md                              # iOS App Store & Apple Search Ads only (16 Rules)
    └── google-play-aso-validator/
        └── SKILL.md                              # Google Play & Keyword Density only (8 Rules)
```

---

## Using in Web Chat UIs (Gemini Web, Claude.ai, ChatGPT)

If someone isn't using a terminal/CLI agent, they can also upload any `SKILL.md` directly into:
- **Google Gemini:** Ask *"Create a skill from this file"* and attach `SKILL.md`, or paste into a **Gem**.
- **Claude.ai Web / Desktop:** Go to **Settings -> Capabilities -> Skills** (or upload to a Claude Project).
- **ChatGPT:** Paste into **Custom GPT Instructions** or upload to a ChatGPT Project.

---

## Example Prompt

```text
Validate my iOS metadata:
App Name: Waya: AI Meeting Notes & Recorder
Subtitle: Transcribe Voice to Text App
Keywords: meeting, notes, transcribe, audio, voice, recorder, minutes, summary, speech, text
```

---

## Authoritative Source Articles Indexed
1. [ASO Strategy: Improving App Store Page Conversion by Optimizing for People](https://appfigures.com/resources/guides/secret-to-aso-optimizing-for-people) (Jun 17)
2. [8 Tips to Optimize Your Keywords List in App Store Connect](https://appfigures.com/resources/guides/keyword-optimization-app-store-connect) (Jun 17)
3. [9 Common ASO Mistakes That Hurt Your Downloads](https://appfigures.com/resources/guides/common-aso-mistakes) (Jun 17)
4. [ASO Checklist 2026: App Store Optimization Steps (with Examples)](https://appfigures.com/resources/guides/app-store-optimization-checklist) (Jun 24, 2026)
5. [How to Improve Your ASO by Analyzing Your Competitors' Keywords](https://appfigures.com/resources/guides/competitor-keyword-analysis) (Jun 24)
6. [App Store Optimization (ASO): The Complete Guide for 2026](https://appfigures.com/resources/guides/app-store-optimization) (Jun 24, 2026)
7. [App Name ASO: Optimize Your App Name & Subtitle for Downloads](https://appfigures.com/resources/guides/app-name-optimization) (Jun 29)
8. [How to Choose ASO Keywords That Drive Downloads on the App Store & Google Play](https://appfigures.com/resources/guides/which-keywords-to-optimize-for) (Jun 29)
9. [ASO Keyword Research: 9 Steps for the App Store & Google Play](https://appfigures.com/resources/guides/keyword-research) (Jun 29)
10. [13 Ways to Promote Your App and Get More Downloads](https://appfigures.com/resources/guides/13-ways-to-promote-your-mobile-app) (Jun 29)
11. [How to 10x Your App Store Keyword List with Secondary Localizations](https://appfigures.com/resources/guides/extend-keyword-list) (Jun 29 / Updated Apr 25, 2023)
12. [Advanced ASO Tips for the App Store & Google Play](https://appfigures.com/resources/guides/advanced-aso-secrets) (Jun 29)
13. [Optimizing Your Apple Search Ads Campaign](https://appfigures.com/resources/guides/optimizing-your-apple-search-ads-campaign) (Jun 29)
