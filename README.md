# Exclusion Lists — Danish Prospecting

This repository contains exclusion data originally sourced from the Google Sheet [Dental Clinics — Exclusion List and Prospecting Rules](https://docs.google.com/spreadsheets/d/1r00Lppx_1IDU-qiPkbbRvaGekEJeL8hqxrboWz6pdZw/edit), first synced on 2026-11-16 and subsequently updated in GitHub.

**Source of truth:** `excluded_clinics.csv` on the default branch. The live count is the number of non-header CSV records, not a fixed number in this README. As of 2026-11-24 the file has 491 rows, including 14 businesses newly added from the user's consolidated lead list on that date. Read the live CSV for the latest count. Do not delete or disregard records merely to match an expected count.

## Exclusion sources

- `excluded_clinics.csv` — canonical exclusion records (read the file for the current count). Includes dentists, cosmetic clinics, and other businesses in the original list, with the newest names from the latest chat merged in. Clinics or people on this list should **not** be proposed again. Includes aliases and available KRAK Personer numbers/URLs.
- `blocked_chains.csv` — 4 blocked dental chains; applies to all their locations.
- `lead_qualification_rules.csv` — 14 existing qualification and verification rules.

## Additional source tabs

- `new_leads_2026-11-16.csv` — 30 lead records from the existing workbook.
- `non_owner_leads_2026-11-16.csv` — 9 existing manager/contact records.
- `cross_industry_managers_2026-11-16.csv` — 30 cross-industry leads.
- `low_review_manager_leads_2026-11-16.csv` — 7 existing low-review manager leads.

## Using exclusions in ChatGPT and lead-generation tools

Before presenting new prospects, read the latest `excluded_clinics.csv` from this repository's `main` branch, not an old README count or a previous chat's cached list. Read `blocked_chains.csv` as well. Check business/clinic names, known aliases, contact names, business phone numbers, and location. New exclusions must be written to the canonical CSV and verified by fetching the changed file after the commit.

**Important:** Updating this GitHub repository does **not** automatically update ChatGPT memory, other conversations, or the Making Leads application's independent saved-exclusions database. Those consumers need an explicit read/synchronization step before research. Do not claim they have synced without verifying their own stored exclusions.

## Duplicate policy

Before researching another lead, check the exclusions by clinic/business name, known aliases, clinic phone number, named dentist/contact, and location, then apply the blocked chains list. The same clinic may appear under multiple names; do not count it as new if the clinic phone or name matches an exclusion.

KRAK Personer identity matching in the user-supplied chat data may be **Probably** or **Possible**, not definitively verified. User-supplied Google review counts and ratings may not be API-verified and can change. Some entries are intentionally name-only because the user explicitly excluded those names without specifying a clinic.

This is a public GitHub repository. Do not add API keys or other credentials.
