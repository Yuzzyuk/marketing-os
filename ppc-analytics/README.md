# Paid Ads Performance Analysis (PPC)

An AI skill that analyzes paid-ads (PPC) performance for marketing agencies and eCommerce businesses — business owners and marketing managers who want plain-language answers about their Facebook Ads and Google Ads results, grounded in their own connected data. Ask about ad spend, impressions, clicks, CTR, CPC, CPM, conversions, CPA, and ROAS and get numbers computed with SQL against your data — never estimated. The skill produces what a senior PPC analyst would: a per-platform funnel trace (impressions → clicks → conversions → revenue), an efficiency-first platform comparison (ranked on CPA and ROAS, never raw spend), spend-vs-budget pacing, ad-fatigue frequency checks, landing-page conversion rates, and an honest treatment of attribution — it never blends Facebook + Google conversions into one inflated number; it reports per platform, offers a directional cross-check against an independent source (never a full reconciliation), and computes blended CAC from deduplicated conversions. Other ad platforms are handled best-effort; Facebook + Google are first-class.

## What it does

- "how are my ads performing"
- "weekly PPC report" / "weekly paid ads review"
- "why did CPA spike"
- "ROAS by platform"
- "Facebook vs Google Ads" / "compare Meta and Google"
- "am I overspending my ad budget" / "ad spend pacing"
- "which campaigns should I scale or pause"
- "ad fatigue check" / "frequency too high"
- "blended CAC" / "true cost per acquisition across channels"
- ICP keyword cluster: Facebook Ads + Google Ads efficiency, PPC analytics for marketing agencies and eCommerce, ROAS, CPA, CPC, CPM, CTR, budget pacing, attribution double-counting, GA4 comparison, blended CAC

## Tool Integrations & Related Skills

**Tool integrations:** **Facebook (Meta) Ads and Google Ads first-class**, plus — best-effort — Instagram Ads, Microsoft Advertising (Bing Ads), TikTok Ads, LinkedIn Ads, Amazon Ads, Apple Search Ads, Pinterest Ads, Snapchat Ads, X (Twitter) Ads, Reddit Ads, Quora Ads, Outbrain Amplify, and Taboola, via Coupler.io MCP tools — `search-datasets`, `list-datasets`, `get-dataflow`, `get-schema`, `get-data` (SQL).

**Related skills:**
- `reporting/report-generation` — composed at the Present step for report formatting + the full validation suite (arithmetic, units, claim-vs-data, attribution logical gates).
- `create-dataflow` — the core connect skill this hands off to for the full source-connection and credential flow.
- `generate-data-set-context` — the core skill that generates a dataset's saved context (business rules, metric definitions) when it's missing.
- `marketing-analytics` — the sibling cross-channel marketing skill (email, social, SEO, cross-channel comparison); use it when the question is broader than paid ads. This skill owns the paid-ads deep dive; `marketing-analytics` owns everything cross-channel — their "use when" boundaries are mirrored so they never compete for the same question.

## Install

- **Coupler.io skills library (start here):** the skill is published in the Coupler.io skills library — browse it and its siblings on the coupler.io skills pages.
- **In-product (existing Coupler users):** connect the Coupler.io MCP; the skill is discoverable via `list-skills` and loaded via `get-skill`.
- **Claude Code plugin / marketplace:** install the `coupler-io/skills` plugin; this skill ships as the `marketing/ppc-analytics` bundle.
