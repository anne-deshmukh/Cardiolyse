# MDR regulatory pathway – analysis inputs for Cardiolyse

Purpose: verified regulatory reference points and the Cardiolyse facts they apply to, so the
group can make and justify its own analysis. **This is not assignment text.** Where the
regulatory status of Cardiolyse is unknown, the options are shown as clearly labelled
scenarios.

**Verification note (2026-10-28):** EUR-Lex could not be read (L01 – a bot-challenge page).
Legal wording is marked as follows:
- **[V-quoted in Lx]** – the legal text was read verbatim inside an official EC/MDCG document Lx;
- **[V]** – read in the primary source (EC notice, Finlex);
- **[not verified]** – from memory or the templates only; check against EUR-Lex before using it.

---

## 1. Qualification as a medical device (TD 1.1.5)

| Reference point | Status | Cardiolyse facts |
|---|---|---|
| MDCG 2019-11 rev.1 gives "ECG interpretation software" as an example of software that "can provide support for healthcare professionals" | [V] L05 | Intended use: ECG analysis and interpretation "offered to physicians on an advisory basis" (S02); "decision support alongside clinical judgement" (S01 /) |
| MDCG 2019-11 rev.1 §7 "Modules": "Modules subject to MDR or IVDR must be explicitly identified"; manufacturers "must provide users with clear information regarding the scope, regulatory status and coverage of each module"; non-medical functions needed for the medical purpose must be assessed with it | [V] L05 | The website separates "certified" analysis from "HRV and wellness analytics" (S01 /certifications). It does not say which side RoHD, the triage categories, digitisation or the Workspace fall on (Q07, Q13) |
| MDCG 2019-11 rev.1 Annex: a pre-hospital ECG system that only stores and transfers data is "not qualified as medical devices"; modules that "create and provide new patient treatment information" are | [V] L05 | Relevant to the split between transfer/storage features and analysis features |
| MDR Art 2(1) definition of "medical device" | [not verified] | – |
| MDR scope is human medical purpose (veterinary products outside) | [not verified] | Vitals4Pets lead (S06) blocked; Q14 |

## 2. Classification (TD 1.1.6)

**Rule 11 (MDR Annex VIII)** – [V-quoted in L05 §4.2.1]:
> "Software intended to provide information which is used to take decisions with diagnosis or
> therapeutic purposes is classified as class IIa, except if such decisions have an impact
> that may cause: death or an irreversible deterioration of a person's state of health, in
> which case it is in class III; or a serious deterioration of a person's state of health or a
> surgical intervention, in which case it is classified as class IIb.
> Software intended to monitor physiological processes is classified as class IIa, except if
> it is intended for monitoring of vital physiological parameters, where the nature of
> variations of those parameters is such that it could result in immediate danger to the
> patient, in which case it is classified as class IIb.
> All other software is classified as class I."

Guidance points [V] L05:
- Rule 11 has three sub-rules: 11a (decisions with diagnosis/therapeutic purposes), 11b
  (monitoring), 11c (all other → class I).
- Sub-rule 11b is "a specific rule for MDSW intended only for monitoring purposes". "Vital
  physiological processes and parameters include, for example, respiration, heart rate…"
- The IIb/III exceptions depend on whether decisions based on incorrect information "are
  reasonably likely to have an impact that may cause" the listed harms. Annex III of L05 maps
  the IMDRF risk categories to Rule 11.
- L17 (MDCG 2021-24 rev.1, April 2026) lists "Electrocardiographs" as a class IIa example under
  the rule for active diagnostic devices – a hardware example, given only as context.

Cardiolyse facts:
- Class IIa is declared by the manufacturer (S01) and registered in EUDAMED for both device
  records (R03a, R03b).
- Features the group should weigh against the exceptions and sub-rule 11b (no conclusion is
  drawn here): "urgent" triage category (S01 /resting-ecg); VT among the 30+ arrhythmias
  (S01 /); a "Risk of SCD" score (S01 /cvd-hrd); "risk of dangerous cardiac events up to two
  months in advance" (S01 /for-healthcare-providers); remote monitoring of home patients
  (S01-B4, S01-B7); the "advisory basis" and clinician sign-off (S02, S01 /certifications).
- The manufacturer's classification rationale is not public (Q20).

## 3. Conformity assessment (TD 1.1.6; QMS 1.2)

| Reference point | Status |
|---|---|
| For MDR class IIa the conformity assessment involves a notified body. MDCG 2025-6 Table 1: "MDR Class IIa, IIb, III – Notified Body Involved? Yes" | [V] L07 |
| Which annexes apply to class IIa (Art 52; Annex IX chapters I and III, or Annex XI, with technical documentation assessment on a representative basis) | [not verified] |
| CE marking followed by the NB identification number (Art 20) | [not verified] |

Cardiolyse facts: MDD certificate type "Annex II excluding section 4" (R03a). No MDR
certificate is visible (R03b, R03c). NB 0197 is designated under the MDR (R04), but no source
says Cardiolyse has an MDR contract with it (Q21).

## 4. Transition from the MDD – Article 120 as amended by Regulation (EU) 2023/607

**Legal text** [V-quoted in L19 §2.1]:
- Art 120(3a)(b): devices with an MDD certificate "valid by virtue of paragraph 2" may be placed
  on the market until "31 December 2028, for class IIb devices other than those covered by
  point (a) …, for class IIa devices, and for class I devices placed on the market in sterile
  condition or having a measuring function."
- Art 120(3c), conditions – all must be met:
  (a) the devices continue to comply with the MDD;
  (b) "there are no significant changes in the design and intended purpose";
  (c) no unacceptable risk;
  (d) "no later than 26 May 2024, the manufacturer has put in place a quality management system
  in accordance with Article 10(9)";
  (e) "no later than 26 May 2024, the manufacturer … has lodged a formal application with a
  notified body … and, no later than 26 September 2024, the notified body and the manufacturer
  have signed a written agreement".
- Art 120(3d): MDR requirements on "post-market surveillance, market surveillance, vigilance,
  registration of economic operators and of devices" apply to legacy devices.
- Art 120(3e): the NB that signed the written agreement is responsible for "appropriate
  surveillance" from 26 Sep 2024 at the latest.

**Guidance** [V] L16 (EC Q&A rev.2, July 2024):
- The extension of the transitional period and of the certificate's validity "is done
  automatically by law, provided the conditions laid down in Article 120(3c) MDR are
  fulfilled" (Q7). The manufacturer "should be able to provide a self-declaration"; an NB
  "confirmation letter" is optional evidence.
- Certificates that expired **before 20 March 2023** need extra conditions (Art 120(2) second
  subparagraph: a written agreement before expiry, or a national derogation) (Q6).
- If no application was lodged by 26 May 2024, "the transition period will end on 26 May
  2024" (Q3).
- A legacy device and the corresponding MDR-certified device "can be placed on the market in
  parallel until the end of the relevant transitional period" (Q2).
- A "device intended to substitute" a legacy device "will need to undergo the full MDR
  conformity assessment before it can be placed on the market" (Q10).
- Legacy devices "are not subject to the MDR UDI requirements" (Q11.2).

**Significant changes** [V] L11 (MDCG 2020-3 rev.1, May 2023), Chart C – software. Examples of
*significant* changes include:
- "change of an algorithm which impact the operating principles … and may alter the diagnosis
  or therapy delivered";
- "new or major modification of architecture";
- "new medical feature or functionality that may change the diagnosis or the therapy delivered
  to the patient";
- "new channel of interoperability";
- new user interface that "impacts the way data is read or interpreted by the user".

Chart A – intended purpose: "additional or new indications" and a new user population (e.g.
"change from professional use to layman use") are significant.

Examples of *non-significant* changes: bug fixes, security updates, new languages,
"reporting format".

### Scenarios for Cardiolyse (the status is unknown – labelled options, not conclusions)

| Scenario | What it would require | Evidence for | Evidence against / unknown | Questions |
|---|---|---|---|---|
| **A. Legacy device under the extended transition until 31 Dec 2028** | HD 601455120001 valid on 26 May 2021 and not withdrawn; 120(3c)(a)–(e) met, incl. MDR QMS and NB application by 26 May 2024 and a written agreement by 26 Sep 2024; no significant change since the MDD certification | Legacy device registered "On the EU market" in EUDAMED (R03a); MDR Basic UDI-DI registered on 2026-09-22 (R03b), suggesting MDR work is under way | Certificate expiry 2024-05-26 (R03a): on that date the legacy status depends entirely on (d)/(e). Complete rebuild "since … 2024" (S01-B1), new inputs and new outputs (S01) – possibly significant changes. The issue date of the certificate is not shown (R03a). | Q19, Q21, Q22, Q23 |
| **B. MDR-certified device** | MDR certificate(s) from an MDR-designated NB | MDR registration exists (R03b); website: "MDR regulation requires a strict view of our validation" (S01 /faq) | No certificate references the Basic UDI-DI (R03b); 0 certificates for the SRN (R03c) – not conclusive for certificates issued before 28 May 2026 (L20) | Q19, Q21, Q26 |
| **C. A + B in parallel** | Both of the above (allowed per L16 Q2) | Two EUDAMED registrations (R03a, R03b) | As above | Q19, Q21 |
| **D. Neither A nor B** | – | – | Not determinable publicly; ask the manufacturer before assuming anything | Q19, Q21, Q22 |

## 5. UDI and EUDAMED (TD 1.1.2; QMS 1.1)

| Reference point | Status | Cardiolyse facts |
|---|---|---|
| Commission Decision (EU) 2025/2371 published in the OJEU 27 Nov 2025 → from **28 May 2026** the first four EUDAMED modules are mandatory: Actor registration, UDI/Devices registration, Notified Bodies & Certificates, Market Surveillance | [V] L04 | SRN registered 2021 (R02); devices registered (R03a, R03b) |
| Devices whose first unit was placed on the market before the mandatory date and which keep being placed after it: registration "within 12 months from the publication in the OJEU of the notice" (i.e. counted from 27 Nov 2025) | [V] L20 Q/A on UDI/DEV, with L04 | MDR UDI-DI registered 2026-09-22 (R03b) |
| Certificates issued after the NB/CRF module became mandatory must be registered; for earlier MDR certificates only later updates/decisions must be | [V] L20 Q10 | R03c: none listed |
| Basic UDI-DI is "the main key in the database and relevant documentation" | [V] L13 | Basic UDI-DI `640649CardiolyseECGB4` (R03b) |
| UDI requirements for software (Annex VI Part C, incl. when a new UDI-DI is needed for software changes) | [not verified] | UDI-PI type includes "Software identification" (R03b) |
| Legacy devices are not subject to MDR UDI | [V] L16 Q11.2 | The legacy record uses an EUDAMED DI, not a GS1 UDI (R03a) |

## 6. PRRC (QMS 1.3)

| Reference point | Status | Cardiolyse facts |
|---|---|---|
| MDR Art 15 (PRRC; qualification; small-enterprise option) | [not verified] | PRRC registered in EUDAMED: Normunds Daudiss, who is also CEO (R02, S01 /about-us). Qualification not public (Q03) |
| 719/2021 contains a provision that Fimea may issue regulations on national requirements for the PRRC's professional qualification under MD Regulation Art 15(1) and (6) | [V] L09 – text read; **section number not confirmed** (it appears before §5 on the Finlex page) | – |

## 7. QMS (QMS template, all sections)

| Reference point | Status | Cardiolyse facts |
|---|---|---|
| Legacy condition: QMS "in accordance with Article 10(9)" by 26 May 2024 | [V-quoted in L19] | Unknown (Q22, Q24) |
| L16 Q11.1: all Art 10(9) aspects to be addressed in principle; for legacy devices some (GSPR identification, Annex I §3 risk management, Art 61 clinical evaluation) need not be complete, but "from 26 May 2024, the manufacturer's QMS should address how compliance with those requirements will be achieved" | [V] L16 | – |
| Content of Art 10(9) (a)–(m) | [not verified] | – |
| Claimed QMS processes: "Controlled design and development records; Risk management across the software lifecycle; Change control and release documentation; Post-market surveillance and complaint handling" | [V] S01 /certifications (manufacturer claim) | ISO 13485 certificate not found (status §2.6) |

## 8. Clinical evaluation, PMS, PMCF (TD 6.1.3, 6.1.4)

| Reference point | Status | Cardiolyse facts |
|---|---|---|
| MDCG 2020-1: MDSW clinical evidence built from "valid clinical association / scientific validity" (§4.2), "technical performance" (§4.3) and "clinical performance" (§4.4) | [V] L06 | 2019: "validated based on device's equivalence and clinical evaluation data" (S02); MIT-BIH, NST, CU, ESC, CSE databases (S02); MyoVasc (S01-B2); pilots (S01-B7, S01-B4) |
| MDR Art 61 and Annex XIV (incl. equivalence rules, PMCF) | [not verified] | – |
| Legacy devices: MDR PMS and vigilance apply (Art 120(3d)) | [V-quoted in L19] | – |
| L20 footnote: legacy devices "do not require a PSUR in Eudamed" (per MDCG 2021-25 and MDCG 2022-21) | [V] L20 | – |
| PSUR/PMS articles 83–86 for MDR devices | [not verified] | – |

## 9. Labelling, IFU and language (TD 2.1, 2.2)

**Finland – Act 719/2021 §5 "Käytettävää kieltä koskevat vaatimukset"**, first paragraph
[V] L09 (verbatim, Finnish):
> "MD-asetuksen 10 artiklan 11 kohdan ja IVD-asetuksen 10 artiklan 10 kohdassa tarkoitettujen
> tietojen ja asiakirjojen on oltava suomen, ruotsin tai englannin kielellä, jollei tietoja ole
> annettu kansainvälisesti tunnustettujen symbolien muodossa. Laitteen turvallisen käytön
> edellyttämien tietojen on kuitenkin oltava suomen ja ruotsin kielellä. Valmistajan on
> riskianalyysin perusteella määriteltävä, mitkä ovat turvallisen käytön edellyttämiä tietoja.
> Jos laite on tarkoitettu potilaiden tai muuten kuluttajien käyttöön, käyttöohjeiden ja
> muiden turvallisen käytön edellyttämien tietojen on oltava suomeksi ja ruotsiksi. […]"

Working translation (unofficial, by the AI tool – check it against the official English
translation if Fimea/Finlex publish one): information and documents referred to in MDR Art
10(11) must be in Finnish, Swedish or English unless given as internationally recognised
symbols. Information needed for the device's safe use must, however, be in Finnish and
Swedish; the manufacturer decides by risk analysis which information this is. If the device
is intended for patients or other consumers, the IFU and other safe-use information must be
in Finnish and Swedish.

Cardiolyse facts: the 2019 IFU is English only (S02); the Workspace has a "Multilingual
interface" (S01 /cardiolyse-ecg-workspace), languages not listed; a patient app existed
(S02, S01-B7) – Q25.

[not verified]: MDR Annex I Chapter III §23 (label and IFU content); Implementing Regulation
(EU) 2021/2226 (eIFU conditions for software); Fimea's guidance page (L10, HTTP 403).

## 10. AI Act (TD 1.1.4, 1.1.7; QMS risk management)

| Reference point | Status | Cardiolyse facts |
|---|---|---|
| A medical-device AI system is high-risk under AI Act Art 6(1) if (1) it is a safety component or itself a medical device **and** (2) it is subject to third-party conformity assessment by an NB under the MDR. Table 1: MDR class IIa → "AIA High-Risk (Art. 6(1)) conditions fulfilled? Yes" | [V] L07 | Class IIa (R03a, R03b); "deep-learning models behind Cardiolyse arrhythmia detection" (S01 /about-us) |
| "The AIA does not impact the risk classification of medical devices … under the MDR" | [V] L07 Q4 | – |
| Whether the Cardiolyse software meets the AI Act definition of an "AI system" | not assessed – needs the manufacturer's model description (Q17) | – |
| Date from which Art 6(1) obligations apply, and whether it was amended (e.g. by a "digital omnibus") | **[not verified]** – EUR-Lex not readable | – |

## 11. Pending legislative change

L15 (Dec 2025 Commission proposal for a targeted MDR/IVDR revision, reportedly including
Rule 11): **not found** on the reachable EC pages on 2026-10-28; legislative status unknown.
Delegated acts "on well-established technologies" were announced on 29 June 2026 (headline
only, seen on the EC medical devices sector page; not opened).

## 12. Regulatory statements still to verify on EUR-Lex

MDR Art 2(1), 5, 10(9), 10(11), 15, 16, 20, 27, 29, 31, 52, 61, 83–86, 120(2), Annex I §23,
Annex II, Annex VI Part C, Annex IX, Annex XI, Annex XIV; Implementing Regulation (EU)
2021/2226; AI Act Art 6(1), 113 and any amending act; the status of the Dec 2025 proposal.
