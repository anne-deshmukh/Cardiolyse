# Extract of the 2019 IFU (S02)

Source: S02 – published Google Doc, read in full on 2026-10-28. It may change, because
Google shows "Updated automatically every 5 minutes" for published docs. Quotes are verbatim.
This is a 2019 document. It is **not** evidence of the current IFU (Q08, Q10).

## Identification

| Field | Content |
|---|---|
| Document title (Google Doc) | "10. User manual - Instruction of Use" (the "10." prefix suggests numbering within a larger document set – not confirmed) |
| Header | "Device: Standalone software Cardiolyse.me \| User manual \| CARDIOLYSE OY" |
| Title | "Cardiolyse.me Instructions for Use" |
| Manufacturer | "CARDIOLYSE OY, GE Health Innovation Village, 2 Kuortaneenkatu, Helsinki, 00510." – https://cardiolyse.com – "Contact: info@cardiolyse.com" |
| Version | "Issue 1 of 15.05.2019" |
| CE marking | Last line: an image of the CE mark (viewed directly) followed by the text "0197". NANDO: 0197 = TÜV Rheinland LGA Products GmbH (R04). |
| Language | English only |

## Intended use

Verbatim text in `03_product/product-description.md` §3.1. Key elements:
- record, store, analyse, display and transfer up to 12-lead ECG
- QRS, VEB and SVEB detection; QRS features; intervals; heart rate; rhythm analysis; abnormal ST-T
- automatic interpretation incl. "ventricular hypertrophy and myocardial infarction" (12-lead)
- "offered to physicians on an advisory basis only"; "not … the sole means of diagnosis"
- "not intended for pediatric use"

## Symbols table

| Symbol title | Description given (verbatim) |
|---|---|
| Manufacturer | "Indicates the medical device manufacturer, as defined in EU Directives 93/42/EEC" |
| Date of manufacture | "Indicates the date when the medical device was manufactured." |
| Caution | "Indicates the need for the user to consult the instructions for use for important cautionary information…" |
| Consult instructions for use | "Indicates the need for the user to consult the instructions for use." |

No standard (e.g. EN ISO 15223-1) is cited.

## Safety and performance (verbatim)

- "Cardiolyse.me software as a medical device safety and performance was validated based on device's equivalence and clinical evaluation data."
- "ECG algorithms were validated on widely acceptable databases MIT-BIH, NST, CU, ESC as well as CSE."
- "Algorithm's sensitivity and specificity is highly dependent on signal quality provided by device."

### "LIST OF FEATURES THAT HAS NOT BEEN VALIDATED AS A MEDICAL DEVICE"

Overall wellbeing score · Risk of heart disorders · Myocardium score · Heart rhythm
disturbances · Heart biological age · Stamina score · Stress index · Fatigue score ·
Emotional score

(Compare the current website, which says RoHD has "independent clinical validation",
S01 /cvd-hrd – see conflicts in `05_regulatory/status-found-online.md` §4.)

## Platforms and set-up

| Item | Content |
|---|---|
| Mobile | Android 6+; "Cardiolyse.me" on Google Play; sign-up in the app |
| Accounts | "doctor's account" (select/create patient, record) and "patient's account" (record) |
| ECG device | Bluetooth BLE, "at least 200 Hz sample rate"; types listed: Live Signals, NeuroSky, Solvaig, Faros (Bittium), Beurer, "HRV device – all other devices that support Bluetooth BLE protocol" |
| Recording example | Solvaig ECG: "Place your fingers on pads" → "START" |
| Web | https://dashboard.cardiolyse.com/ – browsers tested: IE 11+, Edge 16+, Firefox 52+, Chrome 57+, Safari 10.1+, Opera 44+ |
| Web functions | sign in/up; patient list; records per patient; "Detailed report, download report, download record" |

## Cautions (verbatim)

- "The ECG app cannot check for signs of a heart attack. If you believe you're having a medical emergency, call the emergency services."
- "DO NOT take recordings when in close vicinity to strong electromagnetic fields (e.g. electromagnetic anti-theft systems, metal detectors)."
- "DO NOT take recordings during a medical procedure (e.g., magnetic resonance imaging, diathermy, lithotripsy, cautery and external defibrillation procedures)."
- "DO NOT take a recording during physical activity."
- "DO NOT use ECG formats other than EDF / EDF+"
- "Read instructions before use"

## Not present in the 2019 IFU

Contraindications; intended user qualification beyond "physicians"; performance figures
(sensitivity/PPV); list of the arrhythmias detected; the software version number; a UDI;
Finnish or Swedish language versions; residual risks; cybersecurity information; an eIFU
statement. These are listed as absent only; which ones were or are legally required is not
assessed here (see `05_regulatory/mdr-pathway.md` for what could be verified).

Template link: TD 2.2 *Käyttöohjeet*, TD 1.1.1, 1.1.3, 1.1.8, 6.1.1.
