# Regulatory status – what is and is not found online

All checks done on **2026-10-28**. Sources: `01_sources/source-register.md`.

## 1. Manufacturer's own claims

| Claim (verbatim) | Source |
|---|---|
| "Cardiolyse is CE-marked as Class IIa medical device software under EU Regulations." | S01 /, /certifications, /faq, /media-kit |
| "CE · GDPR – CE-marked medical device software · Class IIa – ISO 13485:2016 quality system" | S01 / |
| "Technical file and clinical evaluation available under NDA." | S01 /certifications |
| "The CE certification covers the European Economic Area" | S01 /faq |
| 2019 IFU: CE mark image followed by "0197"; manufacturer symbol "as defined in EU Directives 93/42/EEC" | S02 |

The website names neither the legislation (MDD 93/42/EEC or MDR 2017/745), nor the notified
body, nor any certificate number.

## 2. Registries

### 2.1 EUDAMED – actor (R02)
- Cardiolyse Oy, **SRN FI-MF-000017174**, Manufacturer, Finland, registered 2021-11-26, actor status active.
- PRRC registered: **Normunds Daudiss** ("Responsible for Regulatory Compliance").
- Competent authority: Fimea, Medical Device Unit.

### 2.2 EUDAMED – devices (R03a, R03b)

Device search by SRN → **2 devices**, both "CardiolyseECGSoftware", risk class **IIa**,
status "On the EU market".

| Field | Legacy device (R03a) | MDR device (R03b) |
|---|---|---|
| Applicable legislation | "MDD (Directive 93/42/EEC on Medical Devices)" | "MDR (REGULATION (EU) 2017/745 on medical devices)" |
| Identifier | EUDAMED DI `B-CardiolyseECGsoftwareBH` / EUDAMED ID `D-CardiolyseECGsoftwareBH` (issuing entity EUDAMED) | Basic UDI-DI `640649CardiolyseECGB4`; UDI-DI `06429830147008` (issuing entity GS1) |
| Special device type | Software | Software |
| Active device | **No** | **Yes** |
| Measuring function | **No** | **Yes** |
| Nomenclature (EMDN) | Z12030682 "Vital signs telemetry instruments - software accessories" | Z12050392 "Electrocardiographs - medical device software" |
| Certificates shown | NB **0197, TÜV Rheinland LGA Products GmbH**; type "**Directive 93/42/EEC Annex II excluding section 4**"; certificate no. **HD 601455120001**; revision "-"; issue date "-"; **expiry date 2024-05-26** | "There is no reference to this Basic UDI-DI in any certificate", with the three possible reasons EUDAMED gives: it "does not require a certificate", or it requires only a certificate that does not reference the Basic UDI-DI (e.g. a QMS certificate), or "The required certificate(s) referencing this Basic UDI-DI is(are) not registered yet" |
| Record dates | device version 1 (history); market distribution Finland "From 2020-10-01 to -" | Basic UDI-DI and UDI-DI version 1, "Last update date: 2026-09-22"; market distribution Finland "From 2020-01-01 to 2026-09-22" |

### 2.3 EUDAMED – certificate module (R03c)
- Search by economic-operator SRN FI-MF-000017174: **0 certificates, 0 refused certificates**
  (current versions). The control search for another SRN returned results, so the filter works.
- Interpretation limits (L20, Q10): the obligation to register certificates in the NB/CRF
  module applies to certificates **issued after** the module became mandatory (28 May 2026,
  L04), and to later updates and decisions on certificates issued before that date. So an
  MDR certificate issued **before** 28 May 2026 and not updated since would not necessarily
  appear. **The absence is not proof that no MDR certificate exists.**
- The legacy MDD certificate HD 601455120001 is visible only inside the device record (R03a),
  not in the certificate search.

### 2.4 NANDO (R04)
- 0197 = TÜV Rheinland LGA Products GmbH (Nürnberg, DE). Active notifications include
  "93/42/EEC Medical devices" (with the warning that since 26 May 2021 NBs "are no longer
  able to issue new certificates under that Directive, but only allowed to carry out
  surveillance activities…") and "Regulation (EU) 2017/745 on medical devices".
- The scope of the MDR designation (codes) was not read.

### 2.5 Not checked (blocked)
FDA 510(k) (R05), MHRA PARD (R06), PRH/YTJ (R01), the NHS DSP Toolkit register.

### 2.6 ISO 13485
- Claimed: "ISO 13485:2016" (S01). Certification body, certificate number and scope: **not
  found** in any verified source. EUDAMED shows no QMS certificate for the SRN (R03c).

## 3. What the combination of findings shows – and does not show

Facts (with sources):
1. Under the MDD, a class IIa device was covered by NB 0197 certificate HD 601455120001
   (Annex II excluding section 4), which **expired on 2024-05-26** according to EUDAMED (R03a).
2. The manufacturer registered an **MDR** Basic UDI-DI on 2026-09-22 (R03b). No certificate
   references it (R03b), and the certificate module lists none for the SRN (R03c).
3. The manufacturer says the technology was fully rebuilt "since new management took over in
   2024" (S01-B1).

Not determinable from public sources (→ P1 questions):
- Whether HD 601455120001 was valid on 26 May 2021 and not withdrawn, and whether the Art
  120(3c) conditions were met (MDR QMS by 26 May 2024; application lodged by 26 May 2024;
  written agreement by 26 Sep 2024). Only if all were met would the certificate be deemed
  valid until **31 Dec 2028** for a class IIa device (L19, L16) – Q19, Q21, Q22.
- Whether an MDR certificate has been issued, by which NB, under which conformity assessment
  annex, and when – Q21.
- Whether the 2024 rebuild, new inputs (paper digitisation, wearables, HeartEye) or new
  outputs (RoHD, 30+ arrhythmias, triage categories) are "significant changes", which would
  end the legacy status for the changed device (L11) – Q23.
- Which device the current website calls "CE-marked … Class IIa" – the legacy MDD device,
  an MDR-certified device, or both – Q19.

## 4. Conflicts and inconsistencies (recorded side by side, not resolved)

| Topic | Version A | Version B | Version C |
|---|---|---|---|
| Arrhythmia count | "30+ arrhythmias" (S01 /, /about-us) | Holter: "7 Rhythm and beat findings" (S01 /holter-ecg) | "19 types" in aggregator listings (S23, S24 – blocked, unverified); Beurer PR 19 vs 20 (S07 – blocked) |
| RoHD status | 2019 IFU: "Risk of heart disorders" on the "LIST OF FEATURES THAT HAS NOT BEEN VALIDATED AS A MEDICAL DEVICE" (S02) | Website: "Independent clinical validation" (S01 /cvd-hrd); used for "Risk stratification" in trials (S01 /clinical-trials-pharma) | Certified scope excludes "HRV and wellness analytics" (S01 /certifications); RoHD is not named either way |
| Prognostic claim | "flag risk of dangerous cardiac events up to two months in advance" (S01 /for-healthcare-providers) | "Are the scores a diagnosis? No." (S01 /cvd-hrd) | – |
| Intended users | "qualified healthcare professionals" (S01 /, /certifications) | Patient accounts and a patient app (S02, S01-B7); MedicubeX "self-check" (S01 /) | – |
| EUDAMED device attributes | Legacy: Active No, Measuring No, EMDN Z12030682 (R03a) | MDR: Active Yes, Measuring Yes, EMDN Z12050392 (R03b) | – |
| Address | GE Health Innovation Village, Kuortaneenkatu 2, 00510 Helsinki (S02, 2019) | Terkko Health Hub, Haartmaninkatu 4, 00290 Helsinki (S01) | Haartmaninkatu 4, Building 14 (R02) |
| Product name | "Cardiolyse.me" (S02) | "CardiolyseECGSoftware" (R03a, R03b) | "Cardiolyse", "Cardiolyse ECG Workspace" (S01) |
| Market period, MDR registration | "Finland. (From 2020-01-01 to 2026-09-22)" (R03b) – an end date, and a start date before the MDR registration | Website: product currently offered (S01) | – |
| CEO | Normunds Daudiss (S01, R02 as PRRC) | Anna Starynska (first-session lead; source blocked, unverified) | – |
