# Exclusion Lists — Danish Prospecting

This repository contains the current source data from the Google Sheet [Dental Clinics — Exclusion List and Prospecting Rules](https://docs.google.com/spreadsheets/d/1r00Lppx_1IDU-qiPkbbRvaGekEJeL8hqxrboWz6pdZw/edit), synced on 2026-11-16.

## Exclusion sources

- `excluded_clinics.csv` — 205 exclusion entries. Includes dentists, cosmetic clinics, and other businesses in the original list, with the newest names from the latest chat merged in. Clinics or people on this list should **not** be proposed again. Includes aliases and available KRAK Personer numbers/URLs.
- `blocked_chains.csv` — 4 blocked dental chains; applies to all their locations.
- `lead_qualification_rules.csv` — 14 existing qualification and verification rules.

## Additional source tabs

- `new_leads_2026-11-16.csv` — 30 lead records from the existing workbook.
- `non_owner_leads_2026-11-16.csv` — 9 existing manager/contact records.
- `cross_industry_managers_2026-11-16.csv` — 30 cross-industry leads.
- `low_review_manager_leads_2026-11-16.csv` — 7 existing low-review manager leads.

## Duplicate policy

Before researching another lead, check the exclusions by clinic/business name, known aliases, clinic phone number, named dentist/contact, and location, then apply the blocked chains list. The same clinic may appear under multiple names; do not count it as new if the clinic phone or name matches an exclusion.

KRAK Personer identity matching in the user-supplied chat data may be **Probably** or **Possible**, not definitively verified. User-supplied Google review counts and ratings may not be API-verified and can change. Some entries are intentionally name-only because the user explicitly excluded those names without specifying a clinic.

This is a public GitHub repository. Do not add API keys or other credentials.
