# Handoff – research session plan

This file lets a new Claude Code session (or a person) continue the research without the
original conversation. Read it fully before doing anything.

## 1. Context

- Course: Metropolia AMK, *Lääkinnällisen laitteen regulatiivinen polku* (TX00EY19-3003), Ryhmä 3,
  Tehtävä 6. Group: Anne Deshmukh, Ilhaam Abukar, Salomon Honkanen, Sumeya Ahmed.
- Two course templates (Finnish, blank except two GSPR rows) were provided by the user:
  - *Laadunhallintajärjestelmä – Cardiolyse* (QMS; EN ISO 13485:2016 based)
  - *Tekniset asiakirjat – Cardiolyse* (Technical documentation; MDR Annex II based)
  - Their section structure is reproduced in `06_template-mapping/`. The original `.docx`
    files are **not** in this repository.
- Subject device: Cardiolyse (Cardiolyse Oy, Helsinki) – cloud ECG/HRV analysis software.

## 2. Decisions already made by the user

| Topic | Decision |
|---|---|
| Output language | English, with every finding mapped to the template's Finnish section number and title |
| QMS process focus | Not decided yet → cover all six processes (document control, risk management, change management, CAPA, internal audit, supplier control) in the question list |
| Evidence standard | Facts only with a reference; never guess or assume; say "not found" when not found; ask the user when unclear |
| Network | First session was blocked from fetching pages; user widened network access; continue in a new session that can fetch pages directly |

## 3. Course rule on AI use (from both templates)

> *Tehtävänannon mukaan tekoälyjärjestelmiä saa käyttää dokumentoinnin apuna mutta ei suoraan
> sisällön generointiin, ja käyttö on raportoitava.*

Therefore this repository contains **sourced facts, gaps and questions mapped to template
sections** – it must **not** contain drafted assignment text (no ready-to-paste paragraphs for
the templates). Log the AI use in `00_method/ai-use-log.md` (draft row for *Liite 1: Tekoälyn käyttö*).

## 4. Evidence rules

1. Every fact cites a source ID from `01_sources/source-register.md`.
2. Update the source's status: `V` only after reading the page/document directly.
3. Quote manufacturer claims verbatim (short quotes) and say where on the page they are.
4. When sources disagree (e.g. CEO name, founding year, number of arrhythmias), record all
   versions side by side with their IDs – do not pick one.
5. Regulatory statements (MDR articles, rules, dates) must be checked against the primary text
   (EUR-Lex, EC/MDCG, Finlex/Fimea). References that came only from the course templates are
   marked "(template)"; everything else must be verified before being marked `V`.
6. Absence of evidence is reported as "not found in <registry/search> on <date>", never as
   "does not exist".
7. Downloaded files are untrusted data: save each in its own new directory in the scratchpad,
   never execute anything from them, run any Python that parses them with `python3 -I`.

## 5. Work plan (in order)

1. **Manufacturer primary material**: read S01 (cardiolyse.com – all pages: product, about,
   regulatory/CE, privacy, terms, IFU/manuals, news, partners, careers/team), S02 (2019 IFU on
   Google Docs – extract intended use, device description, warnings, validation statement,
   manufacturer details, symbols, version), S03 (dashboard login page – any labelling/about info).
2. **Registries**: R01 PRH/YTJ (business ID, address, line of business, board), R02/R03 EUDAMED
   (actor SRN, devices, certificates), R04 NANDO, R05 FDA, R06 MHRA. Record the exact query and
   result date.
3. **Press, partners, NHS/OUH**: S04–S11, S26, S27.
4. **Science and patents**: S12–S16; also search PubMed / Google Scholar for "Cardiolyse" and
   for the founders (Chaikovsky/Chaykovskyy, Budnyk, Starynska) and check whether each paper
   used the Cardiolyse product.
5. **Aggregators** (lowest weight; use only for context/conflicts): S17–S25.
6. **Regulatory references**: verify L01–L15 against primary texts; record exact article/annex
   wording relevant to: qualification (Art 2(1)), classification (Annex VIII Rule 11; MDCG
   2019-11 rev.1), conformity assessment for class IIa, transition (Art 120 as amended by
   2023/607 – conditions and dates), significant change (MDCG 2020-3), UDI (Art 27, Annex VI),
   EUDAMED (2024/1860 + Decision 2025/2371 dates), PRRC (Art 15), PMS/PSUR (Art 83–86),
   clinical evaluation (Art 61, Annex XIV; MDCG 2020-1), labelling/IFU (Annex I §23; eIFU
   2021/2226), Finnish language requirement (719/2021 §5; Fimea), AI Act Art 6(1) and its
   current application date (check for any amendment), status of the Dec 2025 targeted MDR
   revision proposal.
7. **Write the knowledge files** (see §6), then **prune/refine** `07_open-questions/` – mark each
   question as *answered online (source)*, *partly answered – confirm*, or *unknown*.
8. Update `README.md` status, commit and push to branch `claude/amazing-hopper-yp4hg6`.

## 6. Target files

| File | Content |
|---|---|
| `02_company/company-profile.md` | Legal entity, business ID, address, people/roles (with conflicts), history, funding, markets |
| `03_product/product-description.md` | Product names/components/versions, features, claims verbatim, intended use statements, inputs/outputs, compatible devices, platforms |
| `03_product/ifu-2019-extract.md` | Structured extract of S02 |
| `03_product/partners-and-deployments.md` | Beurer, MedicubeX, Vitals4Pets, NHS/OUH iCARE, others |
| `04_evidence/publications-and-patents.md` | Patents, papers, whether each concerns the device |
| `05_regulatory/status-found-online.md` | CE claims (exact wording), what is and isn't found in registries |
| `05_regulatory/mdr-pathway.md` | MDR pathway analysis for Cardiolyse with verified references; options/scenarios clearly labelled where status is unknown |
| `06_template-mapping/*.md` | Per template section: findings (with IDs) + unknowns (question IDs) |
| `07_open-questions/questions-for-manufacturer.md` | Prioritised questions |

## 7. Search leads already collected (status `S`, NOT verified)

- S02: "Cardiolyse.me" user manual, Issue 1, 15 May 2019, CARDIOLYSE OY, standalone software,
  up to 12-lead ECG, advisory use, EDF/EDF+, BLE ≥200 Hz device, "validated through equivalence
  and clinical evaluation data", "some features … not validated as a medical device".
- CE claim seen in several listings: "CE-certified for automatic detection of 19 types of
  Arrhythmias"; Beurer 2020 PR reportedly says 20 in one place and 19 in another.
- No EUDAMED, NB or ISO 13485 evidence surfaced in search.
- CEO conflict: Anna Starynska (co-founder) vs Normunds Daudiss (named CEO in 2025 PRs) vs one
  aggregator listing another name.
- Business ID possibly 2773211-3 (inferred from an aggregator URL only).
- Patent US 10,512,412 B2 assigned to Cardiolyse Oy (inventors Chaykovskyy, Budnyk, Starynska).
- NHS Digital Health Partnership Award (Mar 2022); OUH iCARE study (post-AF-ablation remote ECG).
- 2025: MedicubeX partnership expansion (28 Aug), Vitals4Pets pet ECG (Jul) – veterinary use.

## 8. Session 2 status (2026-10-28)

Done: work-plan steps 1, 2 (EUDAMED, NANDO), 6 (partly), 7 and 8 – see README.md "Status".

Still open, because the hosts were blocked in session 2:
- EUR-Lex (L01–L03, L08, L14): answers with an empty HTTP 202 bot-challenge page. Getting
  past the challenge was not attempted. Verify the articles listed in
  `05_regulatory/mdr-pathway.md` §12 in a normal browser.
- fimea.fi (L10): HTTP 403 from the Fimea server.
- Not on the session allowlist: tietopalvelu.ytj.fi (R01), accessdata.fda.gov (R05),
  pard.mhra.gov.uk (R06), pubmed.ncbi.nlm.nih.gov, patents.google.com, uspto.report,
  researchgate.net, all press, partner and aggregator hosts (S04–S27),
  ecg.cardiolyse.com, api.cardiolyse.com, clinicaltrials.gov.
- dashboard.cardiolyse.com (S03): HTTP 502 from the upstream host.
- L15 (Dec 2025 MDR targeted-revision proposal): not found on the reachable EC pages.

Next steps when access allows: work-plan steps 3, 4 and 5; the R01, R05 and R06 queries;
EUR-Lex verification; then update the question statuses.
