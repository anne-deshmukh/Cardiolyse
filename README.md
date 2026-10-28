# Cardiolyse – public-source research for the MDR regulatory pathway

Research repository supporting Metropolia AMK course *Lääkinnällisen laitteen regulatiivinen
polku* (TX00EY19-3003), Ryhmä 3, Tehtävä 6: *Laadunhallintajärjestelmä* and *Tekniset
asiakirjat* for **Cardiolyse** (Cardiolyse Oy, Helsinki – cloud ECG/HRV analysis software).

It collects what can be found online about Cardiolyse, with a reference for every fact, maps
it to the sections of the two course templates, and lists what must be confirmed with the
manufacturer. It does **not** contain drafted assignment text (see the course AI rule in
`00_method/HANDOFF.md` §3).

## Status (2026-10-28, second research session)

| Area | Status |
|---|---|
| Source register | Updated – `01_sources/source-register.md` (V / B / N per source, with dates) |
| Manufacturer material | **Verified**: all 31 cardiolyse.com pages and the 2019 IFU (S01, S02) |
| Registries | **Verified**: EUDAMED actor, 2 device records, certificate search; NANDO (R02–R04). Blocked: PRH/YTJ, FDA, MHRA |
| Regulatory references | Verified via EC/MDCG documents and Finlex (L04–L07, L09, L11, L13, L16–L21). **EUR-Lex blocked** (bot challenge) – MDR/AI Act article wording not verified, marked in the files |
| Press, partners, literature, patents, aggregators | **Blocked** (hosts not on the session's network allowlist) – remain unverified leads |
| Knowledge files | Done – `02_company/`, `03_product/`, `04_evidence/`, `05_regulatory/` |
| Template mapping | Findings filled – `06_template-mapping/` |
| Manufacturer questions | Refined and prioritised with a status per question – `07_open-questions/` |

Key findings at a glance (details and sources in `05_regulatory/status-found-online.md`):
- EUDAMED: Cardiolyse Oy, SRN FI-MF-000017174; PRRC registered; two class IIa device records –
  a legacy MDD record (NB 0197 certificate HD 601455120001, expiry 2024-05-26) and an MDR
  Basic UDI-DI registered 2026-09-22 with no certificate referenced.
- The website claims "CE-marked as Class IIa … under EU Regulations" and ISO 13485, without
  naming the legislation, the NB or the certificates.
- Which legal route the current product uses (legacy transition until 31 Dec 2028 vs MDR
  certificate) cannot be determined from public sources → P1 questions Q19, Q21–Q23.

## Structure

| Folder | Content |
|---|---|
| `00_method/` | Handoff/research plan, evidence rules, AI-use log draft |
| `01_sources/` | Source register with IDs, class and verification status |
| `02_company/` | Company profile |
| `03_product/` | Product description, IFU extract, partners and deployments |
| `04_evidence/` | Patents and publications |
| `05_regulatory/` | Regulatory status found online; MDR pathway analysis |
| `06_template-mapping/` | Findings and unknowns per template section (TD = MDR Annex II; QMS = EN ISO 13485) |
| `07_open-questions/` | Questions for the manufacturer, prioritised |

## Verification codes

`V` verified against the page · `S` search summary only (not a fact yet) · `B` blocked ·
`N` not found. Details in `01_sources/source-register.md`.
