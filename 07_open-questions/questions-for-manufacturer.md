# Questions to confirm with the manufacturer (Cardiolyse Oy)

**Status: refined on 2026-10-28** against the sources verified this session
(`01_sources/source-register.md`).

Columns:
- **Status**: *answered online (ID)* · *partly answered – confirm* · *unknown*.
- **Found online** – what the verified sources say (short; details in `02_`–`05_` files).
- **Template §** – TD = *Tekniset asiakirjat*, QMS = *Laadunhallintajärjestelmä*.
- **Why it matters** – *(template)* = reference taken from the course template; *[V …]* =
  verified this session; *[not verified]* = still to check on EUR-Lex.
- **Priority** – P1 needed to determine the regulatory pathway at all; P2 needed for the
  TD/QMS content; P3 supporting detail.

## P1 at a glance

| ID | Short question | Status |
|---|---|---|
| Q19 | Which legislation does the current CE marking rely on – the MDD legacy certificate, an MDR certificate, or both? DoC? | partly answered – confirm |
| Q21 | Notified body and certificate(s): MDD HD 601455120001 found; any MDR certificate? | partly answered – confirm |
| Q22 | Were the Art 120(3c) conditions met (QMS and NB application by 26 May 2024; written agreement by 26 Sep 2024)? Certificate issue date? | unknown |
| Q23 | Was the 2024 rebuild / were new features a significant change? Is the rebuilt software a "substitute device"? | partly answered – confirm |
| Q13 | Which outputs are inside the certified intended purpose (RoHD, triage categories, prognostic scores, digitisation)? | partly answered – confirm |
| Q10 | Current intended-purpose statement, verbatim | partly answered – confirm |
| Q11 | Intended users: professionals only, or also patients/lay users (patient app, MedicubeX self-check)? | partly answered – confirm |
| Q07 | Which products/modules are inside which EUDAMED registration? | partly answered – confirm |
| Q20 | Classification rationale (Rule 11 sub-rule, why not IIb) | partly answered – confirm |
| Q15 | OEM / white-label: who is the legal manufacturer of combined products? | partly answered – confirm |
| Q16 | Validated input devices and formats; per-device performance | partly answered – confirm |
| Q17 | AI/ML: locked or adaptive; data; change control | partly answered – confirm |
| Q36 | Algorithm validation data and performance per arrhythmia/device | partly answered – confirm |
| Q38 | Clinical evaluation route; equivalent device; use of MyoVasc/pilots | partly answered – confirm |
| Q24 | ISO 13485 certificate: body, scope, validity | unknown |
| Q03 | PRRC qualification | partly answered – confirm |
| Q09 | Basic UDI-DI / UDI-DI coverage | partly answered – confirm |
| Q26 | EUDAMED registrations – complete and correct? | answered online (R03a, R03b) – confirm discrepancies (Q51) |
| Q05 | SRN | answered online (R02) |
| Q01 | Legal manufacturer details on label/DoC | partly answered – confirm |

---

## A. Manufacturer identity and organisation

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q01 | What exact legal manufacturer name, business ID and address appear on the current label, IFU and EU Declaration of Conformity? | partly answered – confirm | Cardiolyse Oy, 2773211-3, Haartmaninkatu 4, 00290 Helsinki (S01 /privacy, R02); EUDAMED adds "Building 14" (R02); the 2019 IFU shows "GE Health Innovation Village, 2 Kuortaneenkatu, Helsinki, 00510" (S02) | TD 1.1; QMS 1.1 | Manufacturer identification on label & DoC – Annex I §23 *(template)* | P1 |
| Q02 | Organisation chart, headcount, all sites (Helsinki and any others, incl. outsourced development locations)? | partly answered – confirm | Management: CEO Normunds Daudiss, CTO Poornima Soundara Rajan, CCO Iryna Zharuk (S01 /about-us). Headcount and other sites: not found. "Global team" (S01 /about-us) | QMS 1.1, 1.3; TD 3.3 | ISO 13485 §5.5 *(template)*; Annex II 3(c) *(template)* | P2 |
| Q03 | What qualification does the PRRC have (MDR Art 15)? Is a deputy appointed? | partly answered – confirm | PRRC registered in EUDAMED: Normunds Daudiss, who is also the CEO (R02). Qualification not public. 719/2021 allows Fimea to set national PRRC qualification requirements (L09) | QMS 1.3 | MDR Art 15 *(template)* [Art 15 wording not verified] | P1 |
| Q04 | Who is the management representative (ISO 13485 §5.5.2)? Is it the Chief Compliance Officer? | unknown | CCO Iryna Zharuk "Runs quality, regulatory and information-security programmes" (S01 /about-us) – her ISO role is not stated | QMS 1.3 | ISO 13485 §5.5 *(template)* | P2 |
| Q05 | What is the manufacturer's EUDAMED SRN? | **answered online (R02)** | FI-MF-000017174, registered 2021-11-26, active | TD 1.1.2; QMS 1.1 | Actor module mandatory from 28 May 2026 [V L04] | – |
| Q06 | Non-EU markets: UK (MHRA registration, UK Responsible Person), USA (FDA), Switzerland, others? | unknown | UK: NHS DSP Toolkit claim only (S01 /faq). Switzerland named for the reporting service (S01 /ecg-reporting). FDA/MHRA registries blocked (R05, R06) | TD 2 | Market scope drives labelling and obligations | P3 |

## B. Product identity, intended purpose and scope

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q07 | Which products/modules (Resting ECG analytics, Holter analytics, ECG Workspace, ECG digitisation, HRV/risk scores, API, patient app, container edition) are inside which device registration (`B-CardiolyseECGsoftwareBH` legacy vs `640649CardiolyseECGB4` MDR)? Which are non-medical modules? | partly answered – confirm | Website lists the products (S01); certified scope list (S01 /certifications); "Resting ECG and Holter ECG run on separate platforms" (S01 /faq); 2 EUDAMED device records (R03a, R03b) | TD 1.1.1, 1.1.9, 1.1.10 | Modules must be explicitly identified [V L05 §7] | P1 |
| Q08 | What is the current software version and release history since IFU Issue 1 (15 May 2019)? Is the 2019 Google-Doc IFU still a controlled document or obsolete? | unknown | 2019 Issue 1 (S02); "full rebuild … since new management took over in 2024" (S01-B1); the 2019 doc is still publicly published (S02) | TD 1.1.7, 1.2.1, 2.2 | Annex II 1.1(g), 1.2(a) *(template)* | P2 |
| Q09 | Which UDI-DIs belong to Basic UDI-DI `640649CardiolyseECGB4`? How is the software version shown in the UDI-PI? When is a new UDI-DI assigned for software changes? | partly answered – confirm | Basic UDI-DI `640649CardiolyseECGB4`, UDI-DI `06429830147008` (GS1), UDI-PI includes "Software identification" (R03b) | TD 1.1.2 | Annex II 1.1(b); Annex VI Part C *(template)*; Basic UDI-DI as main key [V L13] | P1 |
| Q10 | What is the current intended-purpose statement, verbatim (current IFU/DoC)? | partly answered – confirm | 2019 statement (S02); current "scope of certification" bullets (S01 /certifications); the formal statement is "available under NDA" (S01 /certifications) | TD 1.1.1, 1.1.3 | Annex II 1.1(a) *(template)*; basis of classification | P1 |
| Q11 | Who are the intended users and use environments? Is any component for patients/lay users (2019 patient account; 2022 patient app; MedicubeX self-service stations; home Beurer recordings)? | partly answered – confirm | "qualified healthcare professionals" (S01 /, /certifications) versus a patient account (S02), a patient app (S01-B7), "self-check" (S01 /), home use (S01-B5, S01-B6) | TD 1.1.1 | Lay use changes requirements [not verified]; a new lay population is a "significant change" [V L11 Chart A]; patient-facing info must be in Finnish and Swedish [V L09 §5] | P1 |
| Q12 | Patient population (adults only?), indications, contraindications, warnings in the current IFU? | partly answered – confirm | 2019: "not intended for pediatric use"; cautions listed (S02). Current: not found | TD 1.1.3 | Annex II 1.1(c) *(template)* | P2 |
| Q13 | Which outputs are inside the certified intended purpose: arrhythmia list (which of the "30+"?), Holter findings, ST/T, MI, ventricular hypertrophy, triage categories (normal/review/urgent), RoHD ("Risk of SCD"), Universal ECG Score, Personal Baseline Score ("risk of dangerous cardiac events up to two months in advance"), HRV scores, ECG digitisation? | partly answered – confirm | Certified scope = "Automated analysis of digital ECG recordings…"; HRV and wellness are outside (S01 /certifications). RoHD: "not validated as a medical device" in 2019 (S02), "Independent clinical validation" now (S01 /cvd-hrd). Prognostic claim on S01 /for-healthcare-providers | TD 1.1.1, 1.1.5, 1.1.7 | Qualification and classification depend on it [V L05]; new indications = significant change [V L11] | P1 |
| Q14 | Is any veterinary offering (Vitals4Pets lead) the same software? How is it separated? | unknown | Not on any verified page; lead S06 blocked | TD 1.1.5, 1.1.9 | MDR scope is human use [not verified] | P3 |
| Q14b | ECG Reporting Service: Cardiolyse's own cardiologists sign reports. Is this service inside the QMS scope? How are their edits fed back (PMS)? | unknown | Service described (S01 /ecg-reporting) | QMS 1.2; TD 6.1.4 | QMS scope; PMS input | P3 |
| Q15 | For partners (MedicubeX, HeartEye, white-label dashboards, "Co-badged CE technical file support", OEM licensing): who is the legal manufacturer of the combined/branded product? Which DoC covers it? | partly answered – confirm | OEM/white-label models described (S01 /, /for-device-manufacturers); "your regulatory affairs team receives … declarations of conformity" (S01 /for-device-manufacturers); MedicubeX "runs inside" stations (S01-B3) | TD 1.1.8, 6.2(g) | Annex II 1.1(h), 6.2(g) *(template)*; Art 16 [not verified] | P1 |
| Q16 | Which input devices and formats are validated (list), with what minimum specs? Was performance validated per device/lead configuration? | partly answered – confirm | 1/3/6/12 leads; formats EDF, XML, DICOM-ECG, SCP-ECG, HL7 aECG, PDF, PNG, Mortara, DHeart (S01); "Performance benchmarks by device class are available under NDA" (S01 /for-device-manufacturers); 2019: EDF/EDF+ only, BLE ≥200 Hz (S02) | TD 1.1.8, 1.1.12, 6.2(g) | Annex II 1.1(h),(l), 6.2(g) *(template)* | P1 |
| Q17 | AI/ML: model type, locked or continuously learning, training/test data provenance, version control, change control for model updates? | partly answered – confirm | "deep-learning models" (S01 /about-us); "trained on multi-center, expert-labeled datasets" (S01 /); outputs "traceable to the algorithm build" (S01 /for-clinical-trials). Locked/adaptive: not stated | TD 1.1.4, 1.1.7 | Class IIa with NB → AI Act Art 6(1) high-risk conditions fulfilled [V L07]; AI Act dates [not verified] | P1 |
| Q18 | Cloud provider and region(s); GDPR roles; DPIA; on-premises/container editions – who installs, validates and updates them? | partly answered – confirm | "EU data centres", DPA, TLS, encryption at rest (S01 /faq, /certifications); container/air-gapped option, "Signed image releases with QMS-controlled versioning" (S01 /for-device-manufacturers). Provider not named | TD 1.1.10, 3.3; QMS 1.6 (supplier) | Annex II 1.1(j), 3(c) *(template)* | P2 |

## C. Regulatory status

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q19 | Under which legislation is the device currently placed on the market – the MDD legacy route (certificate HD 601455120001), an MDR certificate, or both in parallel? Please share the current DoC(s). | partly answered – confirm | Website: "CE-marked as Class IIa … under EU Regulations" (S01) – legislation not named. EUDAMED: legacy MDD device and MDR device, both "On the EU market" (R03a, R03b) | TD 1.1.6 | Decides whether Art 120 applies [V-quoted L19]; parallel placing allowed [V L16 Q2] | P1 |
| Q20 | Classification rationale: which Rule 11 sub-rule; why IIa and not IIb (e.g. "urgent" triage, VT detection, SCD risk score, remote monitoring of heart rate)? MDD class and rule? | partly answered – confirm | Class IIa in both EUDAMED records (R03a, R03b) | TD 1.1.6 | Rule 11 text [V-quoted L05] | P1 |
| Q21 | Notified body and certificates: (a) MDD: confirm HD 601455120001 (NB 0197), issue date, scope, whether withdrawn. (b) MDR: which NB, certificate number(s), conformity assessment annex, dates. (c) Why is no certificate referenced on the MDR Basic UDI-DI in EUDAMED? | partly answered – confirm | (a) found in R03a (expiry 2024-05-26; issue date "-"); NB 0197 = TÜV Rheinland LGA Products GmbH, designated under the MDD and the MDR (R04). (b) none found (R03b, R03c) – not conclusive for pre-28 May 2026 certificates [V L20] | TD 1.1.6 | NB involvement for IIa [V L07]; NB/CRF registration duties [V L20] | P1 |
| Q22 | If the legacy route is used: Was HD 601455120001 valid on 26 May 2021 and never withdrawn? By 26 May 2024, was an MDR QMS (Art 10(9)) in place and a formal application lodged with an MDR NB? Was the written agreement signed by 26 Sep 2024, and with which NB? Is there a self-declaration / NB confirmation letter? Who performs appropriate surveillance? | unknown | Only the expiry date 2024-05-26 is public (R03a) | TD 1.1.6 | Art 120(3c)(d),(e), 120(3e) [V-quoted L19]; evidence options [V L16 Q7] | P1 |
| Q23 | What changes were made since the MDD certification: the 2024 "full rebuild", new inputs (paper digitisation, wearables, HeartEye 12-lead), new outputs (30+ arrhythmias, triage categories, RoHD, Personal Baseline Score), new users (patients/self-service)? Were they assessed under MDCG 2020-3? Is the rebuilt software a "device intended to substitute" the legacy device? | partly answered – confirm | Rebuild "since new management took over in 2024" (S01-B1); new features and inputs (S01) | TD 1.1.7, 1.2.1 | Significant change ends legacy status [V-quoted L19, (3c)(b)]; software examples [V L11 Chart C]; a substitute device needs full MDR assessment [V L16 Q10] | P1 |
| Q24 | ISO 13485:2016 certificate: certification body, number, scope, validity? Is the QMS also certified against the MDR (Annex IX)? | unknown | Claimed "ISO 13485:2016" (S01); no certificate details; no QMS certificate visible in EUDAMED (R03c) | QMS 1.2 | ISO 13485 §4.2.2 *(template)* | P1 |
| Q25 | Countries of sale; languages of UI, labelling and IFU (Finnish and Swedish for safe-use information and patient-facing information in Finland)? | partly answered – confirm | Markets named (S01-B3, S01 /ecg-reporting); "Multilingual interface" (S01 /cardiolyse-ecg-workspace); 2019 IFU English only (S02); Italian localisation in the 2022 pilot (S01-B7) | TD 2.1, 2.2 | 719/2021 §5 [V L09] | P2 |
| Q26 | Are the EUDAMED device registrations complete and correct? | answered online (R03a, R03b) – confirm discrepancies in Q51 | 2 devices registered | TD 1.1.2 | UDI/DEV module mandatory; registration within 12 months of 27 Nov 2025 for devices already on the market [V L04, L20] | P2 |
| Q27 | Is the IFU electronic only? How are the eIFU conditions met? | unknown | The 2019 IFU is an online Google Doc (S02) | TD 2.2 | Reg. (EU) 2021/2226 *(template)* [not verified] | P2 |
| Q28 | Where does the software show its label information (CE + NB number, UDI, manufacturer, version)? | unknown | – | TD 2.1 | Annex I §23 *(template)* [not verified] | P2 |
| Q51 | EUDAMED discrepancies: legacy record "Active device: No / Measuring function: No / EMDN Z12030682" versus MDR record "Yes / Yes / Z12050392"; MDR market distribution "Finland (From 2020-01-01 to 2026-09-22)" – does the end date mean the MDR device is no longer made available? | unknown | R03a, R03b | TD 1.1.2, 1.1.6, 6.2(f) | Registration accuracy (Art 120(3d) registration duties [V-quoted L19]) | P2 |

## D. Design and manufacturing

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q29 | Software lifecycle (IEC 62304 software safety class, development plan, design reviews, V&V)? | partly answered – confirm | "Controlled design and development records"; "Risk management across the software lifecycle" (S01 /certifications) – no standard named | TD 3.1 | Annex II 3(a) *(template)* | P2 |
| Q30 | Software "manufacturing": build, release, deployment to cloud and to customer containers, configuration management, release validation? | partly answered – confirm | "Change control and release documentation" (S01 /certifications); "Signed image releases with QMS-controlled versioning" (S01 /for-device-manufacturers) | TD 3.2 | Annex II 3(b) *(template)* | P2 |
| Q31 | All design/manufacturing sites and critical suppliers/subcontractors (outsourced development, cloud hosting, digitisation, ECG device partners, reporting cardiologists)? | unknown | – | TD 3.3 (Taulukko 1); QMS 1.2, 1.6 | Annex II 3(c); ISO 13485 §7.4 *(template)* | P2 |

## E. GSPR and standards

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q32 | Which harmonised standards / CS / other standards are applied (e.g. EN ISO 13485, EN ISO 14971, EN 62304, EN 62366-1, EN 82304-1, IEC 60601-2-25 performance clauses, ANSI/AAMI EC57, EN ISO 15223-1, EN ISO 20417, IEC 81001-5-1)? | unknown | Only ISO 13485 and "ISO 27001-aligned" named (S01) | TD 4 | Annex II 4(c) *(template)* | P2 |
| Q33 | GSPR checklist (Annex I) with justifications for non-applicable requirements? | unknown | – | TD 4 (Taulukko 2) | Annex II 4(a)–(d) *(template)* | P2 |
| Q34 | Cybersecurity: threat model, penetration tests, SBOM, vulnerability handling, container image signing? | partly answered – confirm | TLS, encryption at rest, RBAC, audit trail, SSO/MFA (S01 /, /faq); NHS DSP Toolkit claim (S01 /certifications) | TD 4 | MDCG 2019-16 rev.1 (listed, L12) | P2 |

## F. Risk management

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q35 | Main hazards and risk controls (missed or false arrhythmia, wrong triage category, poor signal, digitisation errors, wrong patient association, wearable inputs, lay-user misinterpretation, data loss), acceptability criteria, benefit-risk conclusion? | unknown | Mitigations claimed: per-beat quality scoring, unreadable images "flagged and not analysed" (S01 /holter-ecg, /ecg-digitization); 2019 cautions (S02) | TD 5.1, 5.2 | Annex II 5; Annex I §1, §3, §8; EN ISO 14971 *(template)* | P2 |

## G. Verification, validation and clinical evidence

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q36 | Validation datasets and methods, and sensitivity/PPV per arrhythmia type, per input device/lead count and per signal quality? | partly answered – confirm | 2019: MIT-BIH, NST, CU, ESC, CSE (S02); "trained and validated against expert-annotated ECG data sets" (S01 /faq); benchmarks "under NDA" (S01 /for-device-manufacturers); no figures published | TD 6.1.1, 6.1.2, 1.1.12 | Technical performance [V L06 §4.3] | P1 |
| Q37 | Usability engineering file (IEC 62366-1) with summative evaluation, for clinicians and (if applicable) patients? | unknown | Pilot feedback on usability (S01-B7) | TD 6.1.2 | Annex II 6.1(b) *(template)* | P2 |
| Q38 | Clinical evaluation: CEP/CER; route (equivalence vs own data); which equivalent device; are MyoVasc, Maria Cecilia, Oxford, CRANE included? | partly answered – confirm | 2019: "validated based on device's equivalence and clinical evaluation data" (S02); "clinical evaluation summary" under NDA (S01 /certifications); MyoVasc (S01-B2) | TD 6.1.3, 1.2.2 | MDCG 2020-1 components [V L06]; Art 61 [not verified] | P1 |
| Q39 | PMS plan, PMCF plan/report (or justification), PSUR, vigilance reports, FSCAs, complaint trends? | partly answered – confirm | "Post-market surveillance and complaint handling" claimed (S01 /certifications) | TD 6.1.4; QMS 1.6 | MDR PMS/vigilance apply to legacy devices [V-quoted L19]; Art 83–86 [not verified] | P2 |
| Q40 | Measuring function: which measured values (HR, PR, QRS, QT/QTc, axes) and with what stated accuracy? | partly answered – confirm | Measurements listed (S01 /resting-ecg, /holter-ecg); EUDAMED: measuring function "Yes" (MDR) vs "No" (legacy) (R03a, R03b) | TD 6.2(f) | Annex II 6.2(f) *(template)* | P2 |
| Q41 | Interoperability: API specification (29 endpoints), FHIR/HL7 outputs, validated combinations with partner devices and EHRs? | partly answered – confirm | S01 /ecg-api; API docs host blocked (S29) | TD 6.2(g), 1.1.8 | Annex II 6.2(g) *(template)*; new interoperability channel = significant change [V L11] | P2 |
| Q42 | Is the patented scoring system (US 10,512,412 B2?) part of the certified function? | partly answered – confirm | "a patented scoring system alongside the AI analysis" (S01-B4); patent pages blocked (S12, S13) | TD 1.1.4 | Annex II 1.1(d) *(template)* | P3 |
| Q43 | What evidence supports outcome/prognostic marketing claims ("risk of dangerous cardiac events up to two months in advance"; "Better patient outcomes")? | partly answered – confirm | Claims on S01 /for-healthcare-providers; RoHD study (S01-B2) | TD 5.1, 6.1.3 | Claims must be supported – Art 7 [not verified] | P2 |

## H. QMS processes (all six – the group has not chosen yet)

| ID | Question | Status | Found online | Template § | Why it matters | Priority |
|---|---|---|---|---|---|---|
| Q44 | Document control: eQMS/tool, numbering, review/approval, retention; anonymised example? | unknown | – | QMS 1.6, 2 | ISO 13485 §4.2.4, §4.2.5 *(template)* | P2 |
| Q45 | Risk management procedure: risk policy, acceptability matrix, link to PMS; AI-specific risks? | unknown | "Risk management across the software lifecycle" (S01 /certifications) | QMS 1.6, 2; TD 5.2 | ISO 13485 §7.1; EN ISO 14971 *(template)* | P2 |
| Q46 | Change management: how software/model changes are assessed for regulatory significance (MDCG 2020-3 for legacy; NB notification for MDR) and released? | partly answered – confirm | "Change control and release documentation" (S01 /certifications) | QMS 1.6, 2 | ISO 13485 §7.3.9 *(template)*; [V L11] | P2 |
| Q47 | CAPA: inputs (complaints, audits, PMS, reporting-service feedback), tool, example record? | unknown | – | QMS 1.6, 2 | ISO 13485 §8.5.2, §8.5.3 *(template)* | P2 |
| Q48 | Internal audit: programme, frequency, auditor independence; NB surveillance audits? | unknown | – | QMS 1.6, 2 | ISO 13485 §8.2.4 *(template)* | P2 |
| Q49 | Supplier control: approved supplier list; qualification of cloud host, outsourced developers, reporting cardiologists; quality agreements? | unknown | – | QMS 1.6, 2 | ISO 13485 §7.4 *(template)* | P2 |
| Q50 | Quality policy text, measurable quality objectives, process map, management review frequency? | unknown | – | QMS 1.4, 1.5 | ISO 13485 §5.3, §5.4.1, §4.2.2 *(template)* | P2 |
| Q52 | How is the QMS preparing for the AI Act high-risk obligations (data governance, logging, human oversight, post-market monitoring)? | unknown | – | QMS 1.6; TD 1.1.7 | High-risk via MDR class IIa + NB [V L07]; dates [not verified] | P2 |

Note: no question was removed. Q14b, Q51 and Q52 are new in this revision.
