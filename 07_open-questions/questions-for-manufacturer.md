# Questions to confirm with the manufacturer (Cardiolyse Oy)

**Status: first draft – not yet checked against verified online sources.** The next research
step will mark each question *answered online (source ID)*, *partly answered – confirm*, or
*unknown*.

Columns:
- **Template §** – section of *Tekniset asiakirjat* (TD) or *Laadunhallintajärjestelmä* (QMS)
  the answer feeds.
- **Why it matters** – the requirement. References marked *(template)* come from the course
  templates; all others are marked *(verify)* until checked against the primary legal text.
- **Search lead** – what web search suggested (status `S`, not verified). "–" = nothing found.
- **Priority** – P1 needed to determine the regulatory pathway at all; P2 needed for the TD/QMS
  content; P3 supporting detail.

## A. Manufacturer identity and organisation

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q01 | What is the exact legal manufacturer (name, business ID/Y-tunnus, registered address) shown on the label and EU Declaration of Conformity? | TD 1.1; QMS 1.1 | Manufacturer identification on label & DoC – Annex I §23 *(template)*; Annex IV *(verify)* | S02: "CARDIOLYSE OY", Helsinki; S17: ID possibly 2773211-3 | P1 |
| Q02 | Who is currently top management/CEO? Organisation chart, headcount, all sites (Helsinki; London; any development in Ukraine?) | QMS 1.1, 1.3; TD 3.3 | ISO 13485 §5.5 *(template)*; Annex II 3(c) *(template)* | Conflicting names across S04/S05, S08, S19, S22 | P2 |
| Q03 | Who is the PRRC (name, qualification), employed or "permanently and continuously at disposal"? | QMS 1.3 | MDR Art 15 *(template)*; Art 15(2) small-enterprise option *(verify)* | – | P1 |
| Q04 | Who is the management representative? | QMS 1.3 | ISO 13485 §5.5 *(template)* | – | P2 |
| Q05 | What is the manufacturer's EUDAMED Single Registration Number (SRN)? | TD 1.1.2; QMS 1.1 | Art 31 *(verify)*; actor module mandatory from 28 May 2026 per EC notice L04 *(verify)* | – | P1 |
| Q06 | For non-EU markets: UK Responsible Person / MHRA registration; US FDA status; others? | TD 2 | Market scope defines labelling languages and regulatory obligations *(verify)* | Not found in FDA/MHRA via search | P3 |

## B. Product identity, intended purpose and scope

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q07 | Which product names/components are on the market (e.g. "Cardiolyse", "Cardiolyse.me", web dashboard, Android/iOS apps, API/SDK for partners)? Which are within the CE-marked device and which are non-medical modules? | TD 1.1.1, 1.1.9, 1.1.10 | Annex II 1.1(a),(i),(j) *(template)*; modular software in MDCG 2019-11 rev.1 *(verify)* | S02, S10: dashboard + Android/iOS apps; S24: device-agnostic B2B | P1 |
| Q08 | What is the current software version and its release history since IFU Issue 1 (15 May 2019)? | TD 1.1.7, 1.2.1 | Annex II 1.1(g), 1.2(a) *(template)* | S02 (Issue 1, 2019) | P2 |
| Q09 | What are the Basic UDI-DI and UDI-DI(s), and which issuing entity is used? | TD 1.1.2 | Annex II 1.1(b); Annex VI Part C *(template)*; Art 27 *(verify)* | – | P1 |
| Q10 | What is the current intended purpose statement, verbatim (current IFU/DoC)? | TD 1.1.1, 1.1.3 | Annex II 1.1(a) *(template)*; basis of classification | S02 (2019 wording); marketing wording differs across S08, S23, S24, S25 | P1 |
| Q11 | Who are the intended users (cardiologists, GPs, nurses, patients/lay users) and use environments (hospital, home, remote)? | TD 1.1.1 | Annex II 1.1(a) *(template)*; lay-user requirements Annex I §22 *(verify)* | S02: doctor and patient accounts; S09: patients use app at home | P1 |
| Q12 | Patient population (adults only? paediatric?), indications, contraindications, warnings? | TD 1.1.3 | Annex II 1.1(c) *(template)* | S02 warnings (EDF/EDF+, signal quality) | P2 |
| Q13 | Which outputs are medical claims within the CE-marked intended purpose: arrhythmia list (19 or 20 types? which?), Universal ECG Score, Personal Baseline, HRV stress/fatigue/emotion indicators, "prognosis", heart-failure detection? Which are wellness/non-medical? | TD 1.1.1, 1.1.5, 1.1.7 | Annex II 1.1(a),(e) *(template)*; qualification Art 2 *(template)* | "19 types" (S24, S23); 20 vs 19 (S07); S02: some features "not validated as a medical device" | P1 |
| Q14 | Is the veterinary offering (Vitals4Pets) the same software/version? How is it separated from the human medical device (labelling, intended purpose, configuration)? | TD 1.1.5, 1.1.9 | MDR scope is human use – Art 1/2 *(verify)* | S06 (Jul 2025) | P2 |
| Q15 | In partner products (MedicubeX eHealth stations, Beurer, wearables), is Cardiolyse supplied as OEM/white-label/integrated module? Who is the legal manufacturer of the combined product and who holds the CE for the analysis? | TD 1.1.8, 6.2(g) | Annex II 1.1(h), 6.2(g) *(template)*; Art 16 *(verify)* | S04, S07 | P1 |
| Q16 | Which ECG acquisition devices are validated as inputs (list), with what minimum specs (leads, sampling rate, file formats), and was performance validated per device combination? | TD 1.1.8, 1.1.12, 6.2(g) | Annex II 1.1(h),(l), 6.2(g) *(template)*; MDCG 2020-1 per software–device combination *(verify)* | S02: BLE, ≥200 Hz, EDF/EDF+, up to 12 leads | P1 |
| Q17 | Does the analysis use machine learning? If so, locked or adaptive, training/test data provenance, change control for model updates? | TD 1.1.4, 1.1.7 | Annex II 1.1(d),(g) *(template)*; AI Act Art 6(1) high-risk link via MDCG 2025-6 *(verify)* | Press releases describe "AI-powered" analytics (S04) | P1 |
| Q18 | Where is data hosted (cloud provider, EU region)? GDPR roles (controller/processor), DPIA? | TD 1.1.10, 3.3; QMS 1.6 (supplier) | Annex II 1.1(j), 3(c) *(template)*; GDPR *(verify)* | – | P2 |

## C. Regulatory status

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q19 | Under which legislation is the current CE marking – Directive 93/42/EEC (MDD) or Regulation (EU) 2017/745 (MDR)? Please share the EU Declaration of Conformity. | TD 1.1.6 | Determines whether Art 120 transitional rules apply *(verify)* | CE claims found; legislation never named | P1 |
| Q20 | What class was assigned (under MDD if legacy, and under MDR), and with which classification rule rationale? | TD 1.1.6 | Annex II 1.1(f); Annex VIII *(template)*; Rule 11 & MDCG 2019-11 rev.1 *(verify)* | – | P1 |
| Q21 | Which notified body (name, 4-digit number) and which certificates (QMS / technical documentation), scope, validity dates? | TD 1.1.6 | Class IIa+ conformity assessment involves a NB *(verify)* | Not found via search | P1 |
| Q22 | If legacy device: date of MDD DoC/certificate; did Cardiolyse meet the conditions of Reg. 2023/607 (MDR QMS, NB application and written agreement by the stated deadlines)? | TD 1.1.6 | Art 120(3)–(3f) as amended by 2023/607 *(verify)* | – | P1 |
| Q23 | What design/intended-purpose changes were made since the MDD DoC (new arrhythmias, AI features, new platforms, new input devices)? Were they assessed as "significant"? | TD 1.1.7, 1.2.1 | Legacy status lost on significant change – MDCG 2020-3 *(verify)* | – | P1 |
| Q24 | ISO 13485 certificate: certification body, scope, validity? | QMS 1.2 | ISO 13485 §4.2.2 scope *(template)* | Not found via search | P1 |
| Q25 | In which countries is the device sold, and in which languages are UI, labelling and IFU available (Finnish and Swedish for patients/consumers in Finland)? | TD 2.1, 2.2 | Annex II §2 languages *(template)*; Medical Devices Act 719/2021 §5 *(verify)* | Markets named in a 2025 PR: FI, DE, UK, LV, EE (S-level) | P2 |
| Q26 | Is the device registered in EUDAMED (UDI/device module)? | TD 1.1.2 | Art 29 *(verify)*; device module timelines L04 *(verify)* | – | P1 |
| Q27 | Is the IFU provided only electronically? How are the eIFU conditions met? | TD 2.2 | Implementing Reg. (EU) 2021/2226 *(template)* | S02 is an online document | P2 |
| Q28 | Where does the software show its label information (CE mark + NB number, UDI, manufacturer, version) – e.g. "About" screen? | TD 2.1 | Annex I §23 *(template)* | – | P2 |

## D. Design and manufacturing

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q29 | What software lifecycle is followed (IEC 62304 software safety class, design & development plan, design reviews, V&V)? | TD 3.1 | Annex II 3(a) *(template)*; IEC 62304 *(verify)* | – | P2 |
| Q30 | For software, what are the "manufacturing" steps – build, release, deployment to cloud, configuration management, release validation? | TD 3.2 | Annex II 3(b) *(template)* | – | P2 |
| Q31 | List all design/manufacturing sites and critical suppliers/subcontractors (outsourced development, cloud hosting, ECG device suppliers). | TD 3.3 (Taulukko 1); QMS 1.2, 1.6 | Annex II 3(c) *(template)*; ISO 13485 §7.4 *(template)* | – | P2 |

## E. General safety and performance requirements (GSPR) and standards

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q32 | Which harmonised standards / common specifications / other standards are applied (e.g. EN ISO 13485, EN ISO 14971, EN 62304, EN 62366-1, EN 82304-1, IEC 60601-2-25/-2-47 performance clauses, ANSI/AAMI EC57, EN ISO 15223-1, EN ISO 20417, IEC 81001-5-1)? | TD 4 | Annex II 4(c) *(template)* | – | P2 |
| Q33 | Can we see the GSPR checklist (Annex I) with justifications for non-applicable requirements? | TD 4 (Taulukko 2) | Annex II 4(a)–(d) *(template)* | – | P2 |
| Q34 | Cybersecurity: threat model, penetration testing, SBOM, vulnerability handling? | TD 4 | Annex I software/IT-security requirements *(verify)*; MDCG 2019-16 *(verify)* | – | P2 |

## F. Risk management

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q35 | What are the main identified hazards and risk controls (e.g. missed arrhythmia, false alarm, poor signal quality, wrong patient association, data delay/loss), the acceptability criteria, and the overall benefit-risk conclusion? | TD 5.1, 5.2 | Annex II 5(a),(b); Annex I §1, §3, §8 *(template)*; EN ISO 14971 *(template)* | S02 warns accuracy depends on device signal quality | P2 |

## G. Verification, validation and clinical evidence

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q36 | Which ECG databases and test methods were used for algorithm validation, and what were sensitivity/PPV per arrhythmia type, per input device and per signal quality? | TD 6.1.1, 6.1.2, 1.1.12 | Annex II 6.1(a),(b), 1.1(l) *(template)* | S02: "validated on widely acceptable databases" (not named) | P1 |
| Q37 | Is there a usability engineering file (IEC 62366-1) with summative evaluation – for both clinicians and patients? | TD 6.1.2 | Annex II 6.1(b) *(template)*; IEC 62366-1 *(verify)* | – | P2 |
| Q38 | Clinical evaluation: CEP/CER available? Route used (equivalence vs own clinical data)? Which device was claimed equivalent and on what basis? Are NHS/OUH iCARE results or publications part of the CER? | TD 6.1.3, 1.2.2 | Annex II 6.1(c); Art 61(12); Annex XIV Part A *(template)*; MDCG 2020-1 *(verify)* | S02: "validated through equivalence and clinical evaluation data"; S08, S09 | P1 |
| Q39 | PMS plan, PMCF plan/report (or justification), PSUR, vigilance reports, FSCAs, complaint trends? | TD 6.1.4; QMS 1.6 (CAPA) | Annex II 6.1(d); Annex XIV Part B *(template)*; Art 83–86 *(verify)* | – | P2 |
| Q40 | Does the device claim a measuring function (heart rate, intervals, HRV values)? Stated accuracy? | TD 6.2(f) | Annex II 6.2(f) *(template)* | S02: interval & heart-rate measurement (S-level) | P2 |
| Q41 | Interoperability: interface specifications for connected devices/systems (BLE devices, partner platforms, EHR), validated combinations? | TD 6.2(g), 1.1.8 | Annex II 6.2(g) *(template)* | S02 | P2 |
| Q42 | Is the patented "universal scoring system" (US 10,512,412 B2) part of the CE-marked function? | TD 1.1.4 | Annex II 1.1(d) *(template)* | S12, S13 | P3 |
| Q43 | What evidence supports outcome claims used in marketing (e.g. reduced readmission risk)? | TD 5.1, 6.1.3 | Claims must be supported – Art 7 *(verify)* | S09 mentions a vendor claim (S-level) | P3 |

## H. QMS processes (all six – group has not chosen yet)

| ID | Question | Template § | Why it matters | Search lead | Priority |
|---|---|---|---|---|---|
| Q44 | Document control: eQMS/tool, numbering, review/approval, retention periods; could we see an anonymised example? | QMS 1.6, 2 | ISO 13485 §4.2.4, §4.2.5 *(template)*; retention Art 10(8) *(verify)* | – | P2 |
| Q45 | Risk management procedure: risk policy, acceptability matrix, link to PMS? | QMS 1.6, 2; TD 5.2 | ISO 13485 §7.1; EN ISO 14971 *(template)* | – | P2 |
| Q46 | Change management: how are software changes assessed for regulatory significance and NB notification; release notes? | QMS 1.6, 2 | ISO 13485 §7.3.9 *(template)* | – | P2 |
| Q47 | CAPA: inputs (complaints, audits, PMS), tool, example CAPA record? | QMS 1.6, 2 | ISO 13485 §8.5.2, §8.5.3 *(template)* | – | P2 |
| Q48 | Internal audit: programme, frequency, auditor independence, recent findings; NB surveillance audits? | QMS 1.6, 2 | ISO 13485 §8.2.4 *(template)* | – | P2 |
| Q49 | Supplier control: approved supplier list, qualification of cloud host and outsourced developers, quality agreements, evaluation criteria? | QMS 1.6, 2 | ISO 13485 §7.4 *(template)* | – | P2 |
| Q50 | Quality policy text, measurable quality objectives, process map, management review frequency? | QMS 1.4, 1.5 | ISO 13485 §5.3, §5.4.1, §4.2.2 *(template)* | – | P2 |
