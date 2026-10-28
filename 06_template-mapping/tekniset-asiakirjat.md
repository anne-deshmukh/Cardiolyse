# Template mapping – *Tekniset asiakirjat – Cardiolyse* (MDR Annex II)

Structure and requirement references come from the course template ("(template)"). For each
section: what is known (source IDs from `01_sources/source-register.md`, all accessed
2026-10-28) and what is unknown (question IDs from
`07_open-questions/questions-for-manufacturer.md`). Findings are short pointers to sourced
facts, not text to paste into the assignment.

## 1 Laitteen kuvaus ja eritelmä, mukaan lukien variantit ja lisälaitteet

| § | Finnish title | Requirement (template) | Findings (source IDs) | Unknowns |
|---|---|---|---|---|
| 1.1.1 | Tuotenimi, yleiskuvaus ja käyttötarkoitus | Annex II 1.1(a) | Names: "Cardiolyse.me" (S02, 2019); "CardiolyseECGSoftware" (R03a, R03b); website product names (S01). 2019 intended use verbatim (S02); current certified-scope bullets (S01 /certifications); users "qualified healthcare professionals" (S01 /) vs patient accounts/app (S02, S01-B7) – conflict | Q07, Q10, Q11, Q13 |
| 1.1.2 | Perus-UDI-DI ja tunnistetiedot | Annex II 1.1(b); Annex VI Part C | MDR: Basic UDI-DI `640649CardiolyseECGB4`, UDI-DI `06429830147008`, GS1, UDI-PI incl. "Software identification" (R03b). Legacy: EUDAMED DI `B-CardiolyseECGsoftwareBH` (R03a). SRN FI-MF-000017174 (R02). Legacy devices not subject to MDR UDI (L16) | Q09, Q26, Q51 |
| 1.1.3 | Potilasryhmä, käyttöaiheet ja vasta-aiheet | Annex II 1.1(c) | 2019: "not intended for pediatric use"; cautions (S02). Current IFU: not available | Q12 |
| 1.1.4 | Toimintaperiaate | Annex II 1.1(d) | Cloud SaaS / container engine "not deployed on the device itself" (S01 /for-device-manufacturers); deep-learning models (S01 /about-us); patented scoring system (S01-B4); digitisation pipeline steps (S01 /ecg-digitization) | Q17, Q42 |
| 1.1.5 | Perustelu tuotteen määrittelylle lääkinnälliseksi laitteeksi | Annex II 1.1(e); MDR Art 2 | MDCG 2019-11 rev.1: "ECG interpretation software" as an example of support for HCPs; modules must be delineated (L05). Manufacturer separates certified vs wellness modules (S01 /certifications) | Q07, Q13, Q14 |
| 1.1.6 | Riskiluokka ja sovellettu luokitussääntö | Annex II 1.1(f); Annex VIII | Class IIa (S01; R03a; R03b). Rule 11 text (L05). MDD certificate HD 601455120001, NB 0197, Annex II excl. §4, expiry 2024-05-26 (R03a, R04). No MDR certificate visible (R03b, R03c). Transition and scenarios: `05_regulatory/mdr-pathway.md` §4 | Q19, Q20, Q21, Q22, Q23 |
| 1.1.7 | Uudet ominaisuudet | Annex II 1.1(g) | 2024 rebuild (S01-B1); ECG Workspace launch (S01-B1); digitisation (S01 /ecg-digitization); RoHD and other scores (S01 /cvd-hrd); 30+ arrhythmias (S01 /) | Q08, Q17, Q23 |
| 1.1.8 | Lisälaitteet ja yhdessä käytettävät tuotteet | Annex II 1.1(h) | Input devices and partners (S01 /, /clinical-trials-pharma, S01-B6, S02); see `03_product/partners-and-deployments.md` | Q15, Q16 |
| 1.1.9 | Kokoonpanot ja variantit | Annex II 1.1(i) | Cloud SaaS, private VPC, on-premises/air-gapped container; white-label/co-branded dashboard (S01 /, /for-device-manufacturers, /faq); resting vs Holter "separate platforms" (S01 /faq) | Q07, Q18 |
| 1.1.10 | Keskeiset toiminnalliset osat | Annex II 1.1(j) | API (29 endpoints), Workspace, Holter platform, digitisation, scores (S01) | Q07, Q18 |
| 1.1.11 | Raaka-aineet ja materiaalit | Annex II 1.1(k) | Standalone software (S02; R03a/R03b "Special device type: Software") – no body-contact materials; the justification must be the group's own | – |
| 1.1.12 | Tekniset eritelmät | Annex II 1.1(l) | Leads, formats, deployment, security (S01 /, /ecg-api); 2019 browser list and BLE ≥200 Hz (S02) | Q16, Q36 |
| 1.2.1 | Aiemmat sukupolvet | Annex II 1.2(a) | "Cardiolyse.me" 2019 Issue 1 with Android app and dashboard.cardiolyse.com (S02); MDD legacy device (R03a); 2024 rebuild (S01-B1) | Q08, Q23 |
| 1.2.2 | Samankaltaiset laitteet markkinoilla | Annex II 1.2(b) | Not found in verified sources; the equivalent device of 2019 is not named (S02) | Q38 |

## 2 Valmistajan toimittamat tiedot

| § | Finnish title | Requirement (template) | Findings | Unknowns |
|---|---|---|---|---|
| 2.1 | Merkinnät | Annex II §2; Annex I §23 | 2019: CE + "0197", manufacturer symbol (S02). Current label/"About" screen: not found | Q01, Q25, Q28 |
| 2.2 | Käyttöohjeet | Annex II §2; Reg. (EU) 2021/2226 | 2019 IFU extract (`03_product/ifu-2019-extract.md`, S02), English only, online. 719/2021 §5 Finnish/Swedish rule (L09). eIFU regulation not verified (L14) | Q08, Q25, Q27 |

## 3 Suunnittelu- ja valmistustiedot

| § | Finnish title | Requirement (template) | Findings | Unknowns |
|---|---|---|---|---|
| 3.1 | Suunnitteluvaiheet | Annex II 3(a) | "Controlled design and development records" claimed (S01 /certifications) | Q29 |
| 3.2 | Valmistusprosessit ja niiden validointi | Annex II 3(b) | "Signed image releases with QMS-controlled versioning" (S01 /for-device-manufacturers); "Change control and release documentation" (S01 /certifications) | Q30 |
| 3.3 | Suunnittelu- ja valmistuspaikat (Taulukko 1) | Annex II 3(c) | HQ Haartmaninkatu 4 (S01; R02 "Building 14"); EU data centres, provider not named (S01 /faq) | Q02, Q18, Q31 |

## 4 Yleiset turvallisuus- ja suorituskykyvaatimukset (Taulukko 2)

Template note: rows 10.1 and 10.2 are marked *Ei* with justification "software only"; 10.3 is
marked *Ei* **without** a justification yet.

| Findings | Unknowns |
|---|---|
| Only ISO 13485:2016 and "ISO 27001-aligned" controls are named (S01). No harmonised standard list or GSPR checklist is public. Security measures claimed (S01 /faq). | Q32, Q33, Q34 |

## 5 Hyöty-riskianalyysi ja riskienhallinta

| § | Finnish title | Requirement (template) | Findings | Unknowns |
|---|---|---|---|---|
| 5.1 | Hyöty-riskianalyysi | Annex II 5(a); Annex I §1, §8 | Claimed benefits: triage, throughput, earlier detection (S01 /for-healthcare-providers); outcome claims need evidence (Q43) | Q35, Q43 |
| 5.2 | Riskienhallinnan ratkaisut ja tulokset | Annex II 5(b); Annex I §3 | Risk controls claimed: per-beat signal-quality score, unreadable images rejected, clinician sign-off, audit trail (S01 /holter-ecg, /ecg-digitization, /certifications); 2019 cautions (S02) | Q35, Q45 |

## 6 Tuotteen todentaminen ja validointi

| § | Finnish title | Requirement (template) | Findings | Unknowns |
|---|---|---|---|---|
| 6.1.1 | Testitulokset ja kirjallisuuden arviointi | Annex II 6.1(a) | 2019 databases MIT-BIH, NST, CU, ESC, CSE (S02); no figures public; literature leads blocked (`04_evidence/`) | Q36 |
| 6.1.2 | Testien suunnittelu, protokollat ja johtopäätökset (Taulukko 3) | Annex II 6.1(b) | Not public ("under NDA", S01 /for-device-manufacturers) | Q36, Q37 |
| 6.1.3 | Kliininen arviointi | Annex II 6.1(c); Art 61(12); Annex XIV Part A | 2019: equivalence + clinical evaluation data (S02); MyoVasc RoHD (S01-B2); pilots (S01-B4, S01-B7); MDCG 2020-1 framework (L06) | Q38, Q43 |
| 6.1.4 | Markkinoille saattamisen jälkeinen kliininen seuranta | Annex II 6.1(d); Annex XIV Part B | PMS/complaint handling claimed (S01 /certifications); MDR PMS/vigilance apply to legacy devices (L19) | Q39 |
| 6.2 | Erityistapauksissa vaadittavat lisätiedot (Taulukko 4) | Annex II 6.2 | (a)–(e): software only, no substances or tissues; EUDAMED "No" for tissues/substances (R03a, R03b). (f) measuring function: EUDAMED MDR "Yes" vs legacy "No" (R03a, R03b) – conflict. (g) connects to many ECG devices/EHRs (S01) | Q40, Q41, Q51 |

### Taulukko 3 rows (template) – test areas

Bioyhteensopivuus · Fysikaaliset, kemialliset ja mikrobiologiset ominaisuudet ·
Sähköturvallisuus ja EMC · Ohjelmiston todentaminen ja validointi · Stabiilius ja säilyvyysaika ·
Suorituskyky ja turvallisuus

### Taulukko 4 rows (template) – Annex II 6.2

(a) lääkeaine · (b) ihmis-/eläinperäiset kudokset tai solut · (c) imeytyvät/leviävät aineet ·
(d) CMR-/hormonitoimintaa häiritsevät aineet · (e) steriili / mikrobiologinen tila ·
(f) mittaustoiminto · (g) liitetään muihin laitteisiin
