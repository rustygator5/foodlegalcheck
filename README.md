# 🌍 Is My Food Legal Abroad?

A simple web app to check whether the ingredients in a U.S. food product are
**banned, restricted, or warning-labeled** in other countries (EU, UK, Canada,
Australia/Japan).

**Live:** https://rustygator5.github.io/foodlegalcheck/

## How it works

1. **Look up a food** three ways:
   - 🔍 Search by name (via the free [Open Food Facts](https://world.openfoodfacts.org) database)
   - 📷 Enter a barcode
   - 📋 Paste an ingredient list off the label
2. The app cross-references the ingredients against a **curated regulatory
   database** of controversial additives.
3. You get a per-region verdict (Banned / Restricted / Warning label / Allowed)
   with an explanation and a **"Verify" link** to a source for each ingredient.

## Important

- It flags **individual ingredients**, not whole products — a food is rarely
  "illegal" outright abroad; usually a specific additive is banned, capped, or
  warning-labeled.
- It's **informational, not legal advice.** Food regulations change and have
  many exceptions. Always confirm against the official regulator (EFSA/EU, UK
  FSA, Health Canada, FSANZ).
- Only **known controversial ingredients** are flagged. No flags ≠ certified
  legal everywhere.

## Tech

Single self-contained `index.html` (HTML + CSS + JS, no build step, no
dependencies). Ingredient data: Open Food Facts. Regulatory data: hand-curated,
cross-checked against official and reputable secondary sources (June 2026).
