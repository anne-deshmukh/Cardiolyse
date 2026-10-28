# Product description – as found online

Sources: `01_sources/source-register.md`, all accessed 2026-10-28. Manufacturer claims are
quoted verbatim with their page. Template links: TD 1.1.1–1.1.12, 1.2.1, 1.2.2.

## 1. Names and identifiers (record all versions)

| Name / identifier | Context | Source |
|---|---|---|
| "Cardiolyse.me" – "Standalone software" | 2019 IFU; Android app "Cardiolyse.me" on Google Play; web version at dashboard.cardiolyse.com | S02 |
| "CardiolyseECGSoftware" | EUDAMED device name/trade name, both registrations | R03a, R03b |
| `B-CardiolyseECGsoftwareBH` (EUDAMED DI, issuing entity EUDAMED) / `D-CardiolyseECGsoftwareBH` (EUDAMED ID) | Legacy registration under the MDD; reference/catalogue no. "CardiolyseECGSoftware" | R03a |
| Basic UDI-DI `640649CardiolyseECGB4` (GS1); UDI-DI `06429830147008` (GS1); device model "1"; reference "1"; UDI-PI type "Lot or batch, Manufacturing date, Software identification" | Registration under the MDR, Basic UDI-DI and UDI-DI "Last update date: 2026-09-22" | R03b |
| "Cardiolyse" platform; "Cardiolyse ECG Workspace"; "Resting ECG Analytics"; "Holter ECG Analytics"; "ECG Digitization & AI Analysis"; "Heart Risks & HRV Analytics"; "ECG API & Integration"; "ECG Reporting Service" | Current website product names | S01 (pages of the same names) |

Which of the website products and modules fall under which EUDAMED registration is **not
stated** anywhere (Q07).

## 2. Regulatory status claims on the website (verbatim)

| Claim | Where |
|---|---|
| "Cardiolyse is CE-marked as Class IIa medical device software under EU Regulations. Technical file and clinical evaluation available under NDA." | S01 / (home), S01 /certifications |
| "Resting ECG analysis is CE-marked as Class IIa medical device software under EU Regulations." | S01 /resting-ecg, /cardiolyse-ecg-workspace |
| "ISO 13485:2016" – "Certified quality management system for medical devices" | S01 /, /certifications |
| "ISO 27001-aligned information-security controls"; "certified by NHS Digital for Data Security and Protection compliance" | S01 /, /certifications, /faq |
| "GDPR & HIPAA-aligned" | S01 /, /certifications |
| Documents offered under NDA: "declaration of conformity, intended-purpose statement, clinical evaluation summary, ISO 13485 certificate, security and data-protection documentation, and the DPA" | S01 /certifications |
| "MDR regulation requires a strict view of our validation and model training." | S01 /faq |

Not stated anywhere on the website: the legislation (MDD or MDR) of the CE marking, the
notified body name or number, certificate numbers, the ISO 13485 certification body, the
current software version. See `05_regulatory/status-found-online.md`.

## 3. Intended purpose statements (record all versions)

### 3.1 2019 IFU (S02, section "INTENDED USE", verbatim)

> "The Cardiolyse is intended to record, store, analyze, display and transfer up to twelve
> (12) leads electrocardiogram (ECG).
> The Cardiolyse software performs QRS, Ventricular Ectopic Beats, Supraventricular ectopic
> beats detection, QRS feature extraction, interval measurement, heart rate measurement,
> rhythm analysis and abnormal ST-T changes for up to 12 leads ECG.
> Cardiolyse software also performs automatic ECG interpretation of common abnormalities,
> including ventricular hypertrophy and myocardial infarction for 12 leads ECG.
> The Cardiolyse interpretation results are not intended to be the sole means of diagnosis
> for any abnormal ECG. They are offered to physicians on an advisory basis only in
> conjunction with the physician's knowledge of ECG.
> The device has not been tested and it is not intended for pediatric use."

### 3.2 Current website – "Scope of certification" (S01 /certifications, verbatim)

"Within scope – Certified medical-device software":
- "Automated analysis of digital ECG recordings"
- "Detection and measurement of ECG findings in the recording supplied"
- "Presentation of results to a qualified healthcare professional"
- "Outputs intended to support — not replace — clinical judgement"
- "Clinician sign-off remains part of the diagnostic workflow"

"Handled separately – Analytics outside the certified purpose":
- "HRV and wellness analytics, which are not a diagnostic claim"
- "Research and retrospective dataset work, run under study agreements"
- "Investigational features, kept clearly separated from certified output"
- "Any deployment requiring approval outside the EEA and UK"

FAQ wording (S01 / home): "Our ECG & HRV analytics module is intended for use by qualified
healthcare professionals as decision support alongside clinical judgement — not as an
autonomous diagnostic system."

The formal intended-purpose statement (DoC/IFU) is offered only under NDA (Q10).

## 4. Functions and outputs claimed

| Function / output | Source (verbatim where quoted) | Inside or outside certified scope? |
|---|---|---|
| Resting ECG 1–12 leads: rhythm and arrhythmias ("Sinus rhythm, atrial fibrillation and flutter, ectopic beats, brady- and tachyarrhythmias"); intervals and axes ("Heart rate, PR, QRS, QT, QTc (Bazett and Fridericia), P/QRS/T axes"); "Conduction disturbances such as AV blocks and bundle branch blocks, plus ST-segment and T-wave changes" | S01 /resting-ecg | Stated as CE-marked (S01 /resting-ecg) |
| "Triage-ready conclusion: Each ECG is suggested into a clear category — normal, review or urgent"; Workspace: "6 Conclusion categories, from normal to urgent" | S01 /resting-ecg, /cardiolyse-ecg-workspace | Not stated |
| "AFib, MI and ventricular hypertrophy" | S01 /for-healthcare-providers | Not stated (MI and ventricular hypertrophy were in the 2019 intended use, S02) |
| Holter 1–3 leads: "7 Rhythm and beat findings classified" (NSR, 1st-degree AV block, PAC, pause, AFib, PVC, tachy-brady pattern), bradycardia runs, HR min/max/average, 4 intervals, per-beat signal-quality score | S01 /holter-ecg | Not stated. "Resting ECG and Holter ECG run on separate platforms" (S01 /faq). |
| "30+ arrhythmias detected across resting & Holter ECG"; "30+ arrhythmia classes – AFib, AFlutter, PVCs, PACs, SVT, VT, bradycardia, bundle branch blocks, and more" | S01 /, /about-us | Not stated per class |
| "300 ECG parameters and biomarkers per recording" / "up to 300" | S01 /, /resting-ecg, /faq | Not stated |
| ECG digitisation of paper/PDF/image ECGs (3×4, 6×2, 12×1 layouts; 10 s at 25 mm/s); unreadable images "flagged and not analysed" | S01 /ecg-digitization | Not stated (Q13) |
| Scores: "Risk of SCD / Risk of Heart Disorders (RoHD) – A score for the risk of sudden cardiac death and adverse cardiac outcomes"; Fatigue Score, Emotional Score, Stamina, Stress Level (Baevsky), Heart Biological Age; 21 HRV metrics, 5 ECG codes, 6 scores | S01 /cvd-hrd | HRV and wellness analytics stated as outside (S01 /certifications, /faq). RoHD: **not stated**. The 2019 IFU listed "Risk of heart disorders" as "not validated as a medical device" (S02). "Are the scores a diagnosis? No." (S01 /cvd-hrd) |
| "Universal ECG and Personal Baseline Scores flag risk of dangerous cardiac events up to two months in advance." | S01 /for-healthcare-providers | Not stated (Q13, Q43) |
| "Personal Baseline Score" returned by the "certified engine" | S01 /for-device-manufacturers | Not stated |
| ECG Workspace: worklist, 12-lead review, calipers, editable AI measurements "marked as auto", editable interpretation, sign-off, audit trail, "Multilingual interface", "Auto-populate option for medical findings" | S01 /cardiolyse-ecg-workspace | Workspace described as the review interface (S01 /faq); its regulatory status is not stated separately |
| REST API: "29 Documented API endpoints"; ECG upload sync/async; RR-interval upload; results/parameters; PDF/Excel/JSON reports; signals and annotations (incl. "send corrected annotations back"); patients and records | S01 /ecg-api | – |

## 5. Inputs, platforms, deployment

| Item | Value | Source |
|---|---|---|
| Lead count | "1-, 3-, 6-, and 12-lead ECG"; Holter 1–3 leads | S01 /, /holter-ecg |
| Formats | "EDF, XML, PDF, DICOM-ECG, PNG" (home); "EDF, DICOM-ECG and device formats such as Mortara and DHeart, plus binary, CSV and JSON signals" (API); "XML, PDF, SCP-ECG, DICOM-ECG" (providers); "HL7 aECG" (home FAQ) | S01 /, /ecg-api, /for-healthcare-providers |
| 2019 restriction | "DO NOT use ECG formats other than EDF / EDF+"; BLE device "at least 200 Hz sample rate" | S02 |
| Named devices / wearables | Current: "Consumer wearables (Apple, Withings, KardiaMobile)" (S01 /); "AliveCor, Apple and similar" (S01 /for-healthcare-providers); device partners Beurer (handheld ECG), Corsano (wrist-worn), Movesense (body-worn sensor) (S01 /clinical-trials-pharma); HeartEye 12-lead (S01-B6). 2019: Live Signals, NeuroSky, Solvaig, Faros (Bittium), Beurer, "HRV device – all other devices that support Bluetooth BLE protocol" (S02) | as listed |
| Validation per device | "Performance benchmarks by device class are available under NDA on request." | S01 /for-device-manufacturers |
| Deployment | "EU-hosted managed SaaS (default)"; "Private VPC deployment"; "On-premises container option"; "Container-based deployment (Docker / Kubernetes)"; "Runs air-gapped"; "Signed image releases with QMS-controlled versioning"; "the engine is not deployed on the device itself" | S01 /, /for-device-manufacturers |
| White-label | "The review dashboard can be white-labelled or co-branded (based on regulatory requirements)"; "Co-badged CE technical file support"; "OEM licensing models" | S01 /faq, / |
| Users | Current: "qualified healthcare professionals" (S01 / FAQ). 2019: doctor's account and patient's account (S02). Patient app in the 2022 Maria Cecilia pilot: "Patient-app visibility is fully configurable" (S01-B7). MedicubeX: "self-service check", "when a patient does a self-check" (S01 /, S01-B3) | as listed |
| Patient population | 2019: "not intended for pediatric use" (S02). Current: not stated | S02 |

## 6. Technology and AI

| Item | Value | Source |
|---|---|---|
| AI / ML | "AI-powered"; "trained on multi-center, expert-labeled datasets" (S01 /); "deep-learning models behind Cardiolyse arrhythmia detection" (S01 /about-us); "Our AI is trained and validated against expert-annotated ECG data sets" (S01 /faq) | as listed |
| Locked vs adaptive model; version traceability | "Every measurement is versioned, timestamped and traceable to the algorithm build that produced it" (S01 /for-clinical-trials). Locked/adaptive: **not stated** | Q17 |
| Rebuild | "follows a full rebuild of its technology since new management took over in 2024, with the platform redesigned around the clinical user experience" | S01-B1 |
| Patent | "a patented scoring system alongside the AI analysis" | S01-B4. Patent number not given on the verified page; US 10,512,412 B2 (S12) is blocked/unverified |
| 2019 validation statement | "validated based on device's equivalence and clinical evaluation data"; "ECG algorithms were validated on widely acceptable databases MIT-BIH, NST, CU, ESC as well as CSE"; "sensitivity and specificity is highly dependent on signal quality" | S02 |

## 7. Similar devices (TD 1.2.2)

No verified source names competitor or equivalent devices. The 2019 IFU claims validation
"based on device's equivalence" without naming the equivalent device (S02; Q38).
