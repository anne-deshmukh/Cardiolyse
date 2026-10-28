# Template mapping – *Laadunhallintajärjestelmä – Cardiolyse* (EN ISO 13485:2016)

Structure and requirement references come from the course template ("(template)"). Findings
cite source IDs from `01_sources/source-register.md` (accessed 2026-10-28); unknowns cite
question IDs from `07_open-questions/questions-for-manufacturer.md`.

A QMS is internal to the manufacturer, and almost none of it is public. The findings below
are the manufacturer's **claims** and registry facts. They are not evidence of how the QMS
actually works.

## 1 Laatukäsikirja (quality manual)

Requirement (template): EN ISO 13485:2016 §4.2.2; MDR Art 10(9).

| § | Finnish title | Requirement (template) | Findings (source IDs) | Unknowns |
|---|---|---|---|---|
| 1.1 | Organisaation kuvaus | – | Cardiolyse Oy, 2773211-3, Haartmaninkatu 4, Helsinki (S01 /privacy, R02); SRN FI-MF-000017174 (R02); product lines (S01); see `02_company/company-profile.md` | Q01, Q02 |
| 1.2 | Laatujärjestelmän laajuus | ISO 13485 §4.2.2 | "ISO 13485:2016" claimed, no certificate details (S01); QMS-related claims (S01 /certifications); scope questions: reporting service, container editions, OEM variants (S01 /ecg-reporting, /for-device-manufacturers). Legacy condition: MDR QMS by 26 May 2024 (L19) | Q14b, Q24, Q31 |
| 1.3 | Keskeiset vastuut ja roolit (Taulukko 2) | ISO 13485 §5.5; MDR Art 15 | CEO Normunds Daudiss (S01 /about-us); PRRC in EUDAMED Normunds Daudiss (R02); CCO Iryna Zharuk "Runs quality, regulatory and information-security programmes" (S01 /about-us); CTO Poornima Soundara Rajan (S01 /about-us) | Q02, Q03, Q04 |
| 1.4 | Laatupolitiikka ja laatutavoitteet (Taulukko 3) | ISO 13485 §5.3, §5.4.1 | Not found | Q50 |
| 1.5 | Prosessikartta | ISO 13485 §4.2.2 | Not found | Q50 |
| 1.6 | Viittaukset laadunhallinnan menettelyihin (Taulukko 4) | see below | Claimed processes: "Controlled design and development records; Risk management across the software lifecycle; Change control and release documentation; Post-market surveillance and complaint handling" (S01 /certifications) | Q44–Q49, Q52 |

### Taulukko 4 – procedures listed in the template

| Menettely | EN ISO 13485:2016 (template) | Related MDR / guidance point found this session | Findings | Unknowns |
|---|---|---|---|---|
| Dokumenttien hallinta | 4.2.4 | – (MDR Art 10(8) retention not verified) | Not found. The 2019 IFU is still publicly published as a Google Doc (S02) – whether it is controlled or obsolete is unknown | Q44, Q08 |
| Riskienhallinta | 7.1 (EN ISO 14971) | AI-specific risk management for high-risk MDAI (L07) | "Risk management across the software lifecycle" (S01 /certifications) | Q45, Q52 |
| Muutostenhallinta | 7.3.9 | Significant-change criteria for legacy devices, Chart C software (L11) | "Change control and release documentation" (S01 /certifications); "Signed image releases with QMS-controlled versioning" (S01 /for-device-manufacturers); 2024 rebuild (S01-B1) | Q46, Q23 |
| Korjaavat ja ehkäisevät toimenpiteet (CAPA) | 8.5.2 ja 8.5.3 | MDR vigilance/PMS apply to legacy devices (L19, Art 120(3d) quoted) | "complaint handling" claimed (S01 /certifications); pilot feedback led to roadmap changes (S01-B7) – an example of feedback, not of CAPA | Q47, Q39 |
| Sisäinen auditointi | 8.2.4 | NB "appropriate surveillance" of legacy devices (L18, L19 Art 120(3e)) | "Documented. Audited." (S01 /certifications) – no audit details | Q48 |
| Toimittajien hallinta | 7.4 | – | Critical suppliers not named; cloud provider not named (S01 /faq); device partners named (S01 /clinical-trials-pharma) | Q49, Q31, Q18 |

## 2 Prosessi: [prosessin nimi] – SOP, työohje, esimerkkitallenne

The template asks the group to pick 1–3 of the six processes above and, for each, write an SOP
(tarkoitus, soveltamisala, vastuut, määritelmät, menettely, tallenteet [ISO 13485 §4.2.5],
viitteet), a work instruction and a filled example record.

The group has **not yet chosen** its processes. Public information is thin for every process.
Where the manufacturer's own website gives the most concrete material, the useful pointers are:
- **Change management:** the 2024 rebuild (S01-B1) and MDCG 2020-3 rev.1 Chart C (L11) give a
  real-world case for a change-assessment example.
- **Risk management:** concrete hazards and controls are named on the website (signal quality,
  unreadable images, clinician sign-off – S01 /holter-ecg, /ecg-digitization, /certifications).

Inputs needed from the manufacturer: Q44–Q49, Q52.
