# Source register

Every fact elsewhere in this repository cites a source ID from this table.
All access dates are **2026-10-28** unless stated otherwise.

**Verification status**

| Code | Meaning |
|---|---|
| `V` | Verified: page/document/registry record read directly; quoted text checked. |
| `S` | Search-only: seen only as a web-search result summary in the first session. Content **not** checked against the page. Do not cite as fact. |
| `B` | Blocked: the page could not be read in this session (host refused by the session's network policy, a bot challenge, or a server error – reason given). |
| `N` | Not found: searched for, no result (query and date given). |

**Source class** (evidence weight, highest first)

1. `MFR` – manufacturer's own material (IFU, website, press release issued by Cardiolyse)
2. `REG` – official regulator / registry / legal text (EUR-Lex, EC, Fimea, Finlex, PRH, EUDAMED, NANDO, patent office)
3. `SCI` – peer-reviewed or preprint scientific literature
4. `3P` – independent third party (news, hospital, partner company)
5. `AGG` – commercial data aggregator – lowest weight; often contradictory

How the reading was done: each page/file was downloaded into its own scratch directory and
converted to text with a standard-library parser (HTML) or `pdftotext` (PDF). JavaScript
registries (NANDO, EUDAMED) were rendered in a headless browser and their public JSON API
responses were read. Nothing downloaded was executed.

---

## A. Manufacturer material

| ID | Class | Title / description | URL | Status | Notes |
|---|---|---|---|---|---|
| S01 | MFR | Cardiolyse website – all 31 pages listed in its `sitemap.xml` were read. Cited as `S01 /<path>` (e.g. `S01 /certifications`). | https://cardiolyse.com/ | V | Pages read: `/` (home), `/about-us`, `/for-healthcare-providers`, `/for-device-manufacturers`, `/for-clinical-trials`, `/contact`, `/case-studies`, `/media-kit`, `/faq`, `/resting-ecg`, `/holter-ecg`, `/ecg-digitization`, `/cardiolyse-ecg-workspace`, `/cvd-hrd`, `/ecg-api`, `/clinical-trials-pharma`, `/ecg-reporting`, `/research-development`, `/eu-projects`, `/blogs`, `/clinical-evidence`, `/white-papers`, `/certifications`, `/privacy` (dated "Last updated: 6 October 2026") and 7 blog posts (`/blogs/...`, see S01-B1…B7 below). Website footer: "© 2026 Cardiolyse". |
| S01-B1 | MFR | Blog: "Cardiolyse Launches AI-Powered ECG Workspace for 12-Lead ECG Review…" (dated "October 29, 2026" on the home page; no date on the post itself) | https://cardiolyse.com/blogs/cardiolyse-launches-ai-powered-ecg-workspace-for-12-lead-ecg-review-from-first-read-to-clinician-sign-off | V | Date shown is one day after the access date – recorded as displayed. |
| S01-B2 | MFR | Blog: "Cardiolyse Risk of Heart Disorders score predicts heart failure outcomes in the MyoVasc study" (undated) | https://cardiolyse.com/blogs/cardiolyse-risk-of-heart-disorders-score-predicts-heart-failure-outcomes-in-the-myovasc-study | V | Summarises a conference poster (Carstens D.C. et al., Mainz). The poster itself was not found/read. |
| S01-B3 | MFR | Blog: "Cardiolyse and MedicubeX deepen their collaboration" (28 August 2025) | https://cardiolyse.com/blogs/cardiolyse-and-medicubex-deepen-their-collaboration | V | Republishes the press release S04. |
| S01-B4 | MFR | Blog: "Cardiolyse improves cardiovascular care at Oxford University Hospitals" (home page date: June 1, 2023) | https://cardiolyse.com/blogs/cardiolyse-improves-cardiovascular-care-at-oxford-university-hospitals | V | |
| S01-B5 | MFR | Blog: "CRANE: pre-commercial procurement for remote chronic care" (H2020, 2021–2026) | https://cardiolyse.com/blogs/crane-pre-commercial-procurement-for-remote-chronic-care | V | |
| S01-B6 | MFR | Blog: "…AnyECG project" (Eurostars, HeartEye + Cardiolyse; undated) | https://cardiolyse.com/blogs/bringing-an-innovative-pocket-sized-12-lead-ecg-with-ai-automated-interpretation-to-the-market-anyecg-project | V | |
| S01-B7 | MFR | Blog: "Post-ablation telemonitoring with GVM Care & Research at Maria Cecilia Hospital" (April 2022) | https://cardiolyse.com/blogs/post-ablation-telemonitoring-with-gvm-care-research-at-maria-cecilia-hospital | V | Cites an internal pilot report "not publicly available". |
| S02 | MFR (provenance: see note) | "10. User manual – Instruction of Use", device "Standalone software Cardiolyse.me", CARDIOLYSE OY, "Issue 1 of 15.05.2019", published Google Doc | https://docs.google.com/document/d/e/2PACX-1vS817GWrt2ZzVWzk9AF3cNBv8ygWu2fqwIYxP_nM9_KLcSYNZIQ8Jt1cw-F1VdQdBSK1kd1oGvjYd1W/pub | V | Read in full; extract in `03_product/ifu-2019-extract.md`. Provenance: names Cardiolyse Oy as manufacturer and carries a CE mark image followed by "0197", but it is not linked from the current website – whether it is/was an official controlled IFU must be confirmed (Q08). |
| S03 | MFR | Old web dashboard named in S02 | https://dashboard.cardiolyse.com/ | B | HTTP 502 from the upstream host (host allowed, server did not answer). |
| S28 | MFR | Current sign-in app linked from the website | https://ecg.cardiolyse.com/ | B | Host not allowed by the session's network policy. |
| S29 | MFR | API documentation named in S01 /ecg-api ("api.cardiolyse.com/docs") | https://api.cardiolyse.com/docs | B | Host not allowed by the session's network policy. |

## B. Press, partners and third parties

All hosts in this section were refused by the session's network policy on 2026-10-28
(`CONNECT tunnel failed, response 403`). Contents are therefore **not verified**.

| ID | Class | Title / description | URL | Status |
|---|---|---|---|---|
| S04 | MFR | Press release 28 Aug 2025: Cardiolyse and MedicubeX (EIN Presswire). Its text is republished on S01-B3 (V). | https://www.einpresswire.com/article/843620684/cardiolyse-and-medicubex-announce-deepened-collaboration-to-tackle-global-cardiovascular-disease-prevention | B |
| S05 | MFR | Press release 14 Jul 2025: "Cardiolyse Issues Call for Action on Arrhythmia Risks…" | https://www.medicalindustrytoday.com/article/830524324-cardiolyse-issues-call-for-action-on-arrhythmia-risks-following-the-heart-disease-mortality-study | B |
| S06 | 3P | Vitals4Pets × Cardiolyse partnership (pet ECG), Jul 2025 | https://vitals4pets.com/vitals4pets-and-cardiolyse-partner-to-deliver-instant-ecg-reporting-for-pets-heart-health-insights-in-just-5-minutes/ | B |
| S07 | 3P | Beurer press release (DE), Mar 2020 | https://www.beurer.com/web/we-bilder/presse/2020/200319_Cardiolyse/Beurer-StartUp-Cardiolyse_0320.pdf | B |
| S08 | 3P | HTWorld, Mar 2022: NHS Digital Health Partnership Award | https://www.htworld.co.uk/?p=9309 | B |
| S09 | 3P | Cardiomyopathy UK – iCARE study page | https://cardiomyopathy.org/our-research-campaigns/understanding-more/supporting-research/icare-study | B |
| S10 | 3P | Health Capital Helsinki – Cardiolyse article | https://healthcapitalhelsinki.fi/cardiolyse/ | B |
| S11 | 3P | Oxford "Big Healthcare Challenges" – Cardiolyse PDF | https://innovation.ox.ac.uk/wp-content/uploads/2014/08/Cardiolyse-Wenming-Ji.pdf | B |

## C. Patents and scientific literature

| ID | Class | Title / description | URL | Status |
|---|---|---|---|---|
| S12 | REG | US 10,512,412 B2 (Google Patents) | https://patents.google.com/patent/US10512412B2/en | B (host not allowed) |
| S13 | REG | Same patent, USPTO mirror | https://uspto.report/patent/grant/10,512,412 | B (host not allowed) |
| S14 | SCI | Boreiko, Budnyk, Chaikovskyy et al. (ResearchGate) | https://www.researchgate.net/publication/352971357_Development_of_the_Remote_Heart_Health_Monitoring_System | B (host not allowed) |
| S15 | SCI | PubMed 41835868 (Frontiers in Psychology 2026) | https://pubmed.ncbi.nlm.nih.gov/41835868/ | B (host not allowed) |
| S16 | SCI | PubMed 42571296 | https://pubmed.ncbi.nlm.nih.gov/42571296/ | B (host not allowed) |
| S30 | SCI | Carstens D.C. et al., poster "Clinical relevance of the 'Risk of Heart Disorders' Score from a cloud-based analysis of Holter ECG data (Cardiolyse™)…", D-A-CH Dreiländertreffen Herzinsuffizienz – known only from S01-B2 | – | N (not searched for directly; no URL given in S01-B2) |
| S31 | SCI | MyoVasc study registration NCT04064450 – known only from S01-B2 | – | not opened (clinicaltrials.gov not on the allowlist) |

## D. Company registries, directories, aggregators

All hosts below were refused by the session's network policy on 2026-10-28.

| ID | Class | Title / description | URL | Status |
|---|---|---|---|---|
| S17 | AGG | Funnelfeedr – Cardiolyse Oy | https://funnelfeedr.com/en/company/fi/cardiolyse-oy-27732113 | B |
| S18 | AGG | PitchBook | https://pitchbook.com/profiles/company/174980-71 | B |
| S19 | AGG | CB Insights | https://www.cbinsights.com/company/cardiolyse | B |
| S20 | AGG | Dealroom | https://app.dealroom.co/companies/cardiolyse | B |
| S21 | AGG | Crunchbase | https://www.crunchbase.com/organization/cardiolyse | B |
| S22 | AGG | Tracxn | https://tracxn.com/d/companies/cardiolyse/__D7yNdkdEVy0zsrN2WgSeodZVfxhMposnApGNBm_tYgo | B |
| S23 | AGG | EU-Startups directory | https://www.eu-startups.com/directory/cardiolyse/ | B |
| S24 | AGG | Capterra | https://www.capterra.com/p/196092/Cardiolyse/ | B |
| S25 | AGG | MedicalExpo | https://www.medicalexpo.de/soc/cardiolyse-126751.html | B |
| S26 | 3P | Ukrainian Startup Fund – Pitch Day results (May 2020) | https://merezha-tt.ukrintei.ua/en/2020/06/10/ogolosheni-startapi-peremozhczi-shostog/ | B |
| S27 | 3P | Google blog – Ukrainian startups | https://blog.google/around-the-globe/google-europe/ukrainian-startups-are-building-for-the-future/ | B |

## E. Official registries

| ID | Registry | Query and result (2026-10-28) | URL | Status |
|---|---|---|---|---|
| R01 | PRH / YTJ (Finnish Trade Register) | Not queried – host not allowed. The business ID 2773211-3 is confirmed by S01 /privacy, S01 /media-kit and R02 instead. | https://tietopalvelu.ytj.fi/ | B |
| R02 | EUDAMED – Actor (economic operator) | Search "Name or abbreviated name" = `cardiolyse` → 1 result: **Cardiolyse Oy, SRN FI-MF-000017174**, role Manufacturer. Actor page read (public information, version 5, last update 2026-02-16). | https://ec.europa.eu/tools/eudamed/#/screen/search-eo/b174cfab-6415-430e-8f81-8570e9bfdf6c | V |
| R03a | EUDAMED – Device (legacy, MDD) | Device search by SRN FI-MF-000017174 → 2 devices. This one: EUDAMED DI `B-CardiolyseECGsoftwareBH`, applicable legislation MDD. Detail page read. | https://ec.europa.eu/tools/eudamed/#/screen/search-device/01505afe-01a2-46b7-b000-61cff2908a38 | V |
| R03b | EUDAMED – Device (MDR) | Second device: Basic UDI-DI `640649CardiolyseECGB4` (GS1), UDI-DI `06429830147008`, applicable legislation MDR. Detail page read. | https://ec.europa.eu/tools/eudamed/#/screen/search-device/d3d748ec-3f21-4ef2-a904-9b634f5d4a7a | V |
| R03c | EUDAMED – Certificates module | Certificate search, "Economic operator Actor ID/SRN" = FI-MF-000017174: **0 certificates, 0 refused certificates** (current versions). The "include historical versions" variant timed out (not answered). The same API filter returned 6 certificates for a control SRN (Philips, NL-AR-000001422), so the filter works. | https://ec.europa.eu/tools/eudamed/#/screen/certificates | V (0 results) |
| R04 | NANDO (Single Market Compliance Space) | NB number **0197** = **TÜV Rheinland LGA Products GmbH**, Tillystraße 2, 90431 Nürnberg, Germany; notification status Active; notified under, among others, *93/42/EEC Medical devices* (with the EC warning that since 26 May 2021 it can only carry out surveillance of MDD certificates) and *Regulation (EU) 2017/745 on medical devices*. | https://webgate.ec.europa.eu/single-market-compliance-space/notified-bodies/notifications?organizationRefeCd=EPOS_43519 | V |
| R05 | FDA 510(k) database | Not queried – host not allowed. | https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfpmn/pmn.cfm | B |
| R06 | MHRA PARD | Not queried – host not allowed. | https://pard.mhra.gov.uk/ | B |

## F. Legal and guidance references

EUR-Lex (L01, L02, L03, L08, L14) answered every request with an empty HTTP 202 bot-challenge
page. Getting past the challenge was not attempted. **No article wording was read on
EUR-Lex.** Where an official EC/MDCG document quotes the legal text verbatim, that quotation
is used and marked as such.

| ID | Document | URL | Status | Notes |
|---|---|---|---|---|
| L01 | Regulation (EU) 2017/745 (MDR) | https://eur-lex.europa.eu/eli/reg/2017/745/oj | B (EUR-Lex bot challenge) | Rule 11 wording verified via L05; Art 120(3)–(3e) via L19. Every other MDR article cited in this repository is marked *(not verified)*. |
| L02 | Regulation (EU) 2023/607 | https://eur-lex.europa.eu/eli/reg/2023/607/oj | B (EUR-Lex) | Content verified via L16 and L19. |
| L03 | Regulation (EU) 2024/1860 | https://eur-lex.europa.eu/eli/reg/2024/1860/oj | B (EUR-Lex) | Content verified via L20 and L04. |
| L04 | EC news 27 Nov 2025: "The EUDAMED four first modules will be mandatory to use as from 28 May 2026" (Commission Decision (EU) 2025/2371) | https://health.ec.europa.eu/latest-updates/eudamed-four-first-modules-will-be-mandatory-use-28-may-2026-2025-11-27_en | V | |
| L05 | MDCG 2019-11 rev.1 (June 2025) – qualification and classification of software | https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en?filename=mdcg_2019_11_en.pdf | V | Quotes MDR Annex VIII Rule 11 verbatim (§4.2.1). |
| L06 | MDCG 2020-1 (March 2020) – clinical evaluation of MDSW | https://health.ec.europa.eu/document/download/19d9e24f-2808-4e00-bfeb-75892047407d_en?filename=md_mdcg_2020_1_guidance_clinic_eva_md_software_en.pdf | V (structure only) | Sections 4.2 valid clinical association, 4.3 technical performance, 4.4 clinical performance. |
| L07 | MDCG 2025-6 / AIB 2025-1 (June 2025) – MDR/IVDR and AI Act | https://health.ec.europa.eu/document/download/b78a17d7-e3cd-4943-851d-e02a2f22bbb4_en?filename=mdcg_2025-6_en.pdf | V | |
| L08 | Regulation (EU) 2024/1689 (AI Act) and any amendment of its dates | https://eur-lex.europa.eu/eli/reg/2024/1689/oj | B (EUR-Lex) | Application dates **not verified**. |
| L09 | Laki lääkinnällisistä laitteista 719/2021, Finlex (consolidated, "Ajantasaistettu lainsäädäntö") | https://www.finlex.fi/fi/lainsaadanto/2021/719 | V | §5 heading "Käytettävää kieltä koskevat vaatimukset" and its first paragraph read; see `05_regulatory/mdr-pathway.md` §9. |
| L10 | Fimea – national language requirements | https://fimea.fi/en/medical-devices/device-distributors-and-importers/distributors/national-language-requirements | B | fimea.fi answered HTTP 403 (refused by the Fimea server). |
| L11 | MDCG 2020-3 rev.1 (May 2023) – significant changes, Art 120 | https://health.ec.europa.eu/document/download/800e8e87-d4eb-4cc5-b5ad-07a9146d7c90_en?filename=mdcg_2020-3_en_1.pdf | V | |
| L12 | MDCG 2019-16 rev.1 (July 2020) – cybersecurity | https://health.ec.europa.eu/document/download/b23b362f-8a56-434c-922a-5b3ca4d0a7a1_en?filename=md_cybersecurity_en.pdf | listed in L21 (title/date only) | Not read. |
| L13 | MDCG 2018-1 rev.4 (April 2021) – Basic UDI-DI | https://health.ec.europa.eu/document/download/cb1bf6e5-3972-4b3a-82d9-c5946738b2a5_en?filename=md_mdcg_2018-1_guidance_udi-di_en.pdf | V (partly read) | |
| L14 | Implementing Regulation (EU) 2021/2226 – eIFU | https://eur-lex.europa.eu/eli/reg_impl/2021/2226/oj | B (EUR-Lex) | |
| L15 | Commission proposal (Dec 2025) for a targeted MDR/IVDR revision | – | N | Not found on the reachable EC pages (health.ec.europa.eu sector, new-regulations and latest-updates pages checked 2026-10-28); legislative status unknown. |
| L16 | EC Q&A rev.2 (July 2024) on Regulation (EU) 2023/607 | https://health.ec.europa.eu/document/download/592008f6-3456-4afb-a13a-733a87da1b00_en?filename=mdr_proposal_extension-q-n-a_1.pdf | V | |
| L17 | MDCG 2021-24 rev.1 (April 2026) – classification of medical devices | https://health.ec.europa.eu/document/download/cbb19821-a517-4e13-bf87-fdc6ddd1782e_en?filename=mdcg_2021-24_en.pdf | V (searched for ECG examples only) | |
| L18 | MDCG 2022-4 rev.2 – appropriate surveillance of legacy devices | https://health.ec.europa.eu/document/download/e5714b2b-e98b-4fce-b5ff-d9141a8f30e1_en?filename=mdcg_2022-4_en.pdf | V (introduction read) | |
| L19 | MDCG 2021-25 rev.1 (October 2024) – MDR requirements for legacy devices | https://health.ec.europa.eu/document/download/cbb11a6e-f0f3-4e30-af5e-990f9ef68bc1_en?filename=md_mdcg_2021_25_en.pdf | V | Quotes MDR Art 120(3)–(3e) as amended by 2023/607 verbatim (§2.1). |
| L20 | EC Q&A (November 2024) on the gradual roll-out of EUDAMED (Regulation (EU) 2024/1860) | https://health.ec.europa.eu/document/download/0e7327c7-0e06-4fbd-90d3-8ab7bb30fe9f_en?filename=md_eudamed-qa_en.pdf | V | |
| L21 | EC index "Guidance – MDCG endorsed documents and other guidance" | https://health.ec.europa.eu/medical-devices-sector/new-regulations/guidance-mdcg-endorsed-documents-and-other-guidance_en | V | Used to find current revisions of L05–L20. |
