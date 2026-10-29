# Role: Plumber (Commercial and Residential, Rough-In through Trim)

Answer key: `answer-keys/field/mep/plumber-KEY.md`
Trade group: **MEP**.

## Benchmarks (verify current editions per `update-checklist.md`)

**Code**
- Use the plumbing code adopted by the state and locality where the job is.
- **TN:** the statewide plumbing code is the **2021 International Plumbing Code (IPC)**, in effect since April 17, 2025, per the State Fire Marshal's code history.
- **VA:** 2021 IPC, 2021 IMC, and 2021 IFGC, adopted through the 2021 USBC (Virginia Construction Code), effective **1/18/2024**; VA amendments are in VCC §2801.1.3 (IMC), §2801.1.4 (IFGC), and §2901.1.1 (IPC). The 2024 VA code cycle is still in rulemaking (not yet effective). https://www.dhcd.virginia.gov/codes · https://law.lis.virginia.gov/admincode/title13/agency5/chapter63/section10/ (checked 2026-10-29)
- **GA:** 2024 IPC, 2024 IMC, and 2024 IFGC with Georgia amendments, effective **1/1/2026** (DCA amendment packets marked "Revised January 1, 2026"). https://dca.georgia.gov/community-assistance/construction-codes/current-state-minimum-codes-construction (checked 2026-10-29)
- Local jurisdictions may adopt a different edition or amendments. Confirm with the local codes office.
- Some states use the **Uniform Plumbing Code (UPC, IAPMO)** instead. Ask which code applies at the job location.

**Licensing:** licensed per the state and locality where the work is (primary VA; offices GA and TN).
- **VA** (DPOR Board for Contractors, Tradesmen program):
  - journeyman and master plumber licenses
  - a Residential Plumbing license, added 4/1/2025 (no commercial work)
  - gas fitter and LP gas fitter are separate licenses
  - there's no apprentice license; unlicensed workers work under a licensed tradesman's supervision
- **GA** (Construction Industry Licensing Board, Rule 121-3-.02):
  - Journeyman Plumber
  - Master Plumber Class I (single-family and one-level two-family dwellings, and commercial structures up to 10,000 SF)
  - Master Plumber Class II (unrestricted)

**TN licensing** (Board for Licensing Contractors)
- **Limited Licensed Plumber (LLP):**
  - Who needs it: an individual license for work **under $25,000 per project**, where the local government uses the state Division of Fire Prevention for inspections. Work under $500 is exempt, but check with the local government first. Authority: T.C.A. §62-6-403.
  - Exam: 40 questions, 2 hours, based on the 2021 IPC.
- **$25,000 or more:** requires a contractor license with **CMC or CMC-A (plumbing)** classification.
  - Requirements: Board pre-approval, 3 years of experience, the trade exam, and the Business & Law exam.
  - Trade exam: 100 questions, 5 hours. Weights include DWV 20, Isometrics 18, Code 10, Fuel Gas 10, and Water Supply 10.
- **Journeyman and master licenses** are issued by local jurisdictions (cities and counties), not by the state. Verify the local card.

**Training**
- **UA apprenticeship:** typically 5 years of paid on-the-job training plus related classroom instruction. Hours vary by local.
- **NCCER Plumbing:** Levels 1–4.

**Certifications**
- **ASSE 5110:** backflow prevention assembly tester.
  - Prerequisites: 5 years of experience and a 40-hour course.
  - Tests: a 100-question written exam (70% to pass) plus a practical.
  - Valid for 3 years. Verify the card on the ASSE/IAPMO registry.
- **ASSE 6010:** medical gas installer, ASSE Series 6000-2024, aligned with NFPA 99-2024. Required for med gas work in healthcare facilities.
- **OSHA 10/30**, trenching/excavation, and confined space training.

## Position tuning
```yaml
position_title: Plumber            # Helper/Apprentice | Journeyman | Lead/Foreman | Service Plumber
seniority: mid                     # entry | mid | senior
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: [commercial rough-in, residential, underground, water heaters, gas piping, backflow testing, med gas, service/repair]
code_at_job: "?"                   # the code where the job is, e.g., TN: 2021 IPC statewide or local amendment; VA: 2021 IPC + VCC §2901.1.1; GA: 2024 IPC + GA amendments; UPC in some states; ask
license_required: "?"              # per the state and locality of the job; e.g., VA: DPOR journeyman/master plumber; GA: Journeyman or Master Class I/II; TN: LLP or local journeyman card, company CMC-A
must_have_certs: []                # e.g., ASSE 5110 if testing backflow; ASSE 6010 if med gas
nice_to_have: [UA/NCCER Plumbing level, ASSE 5110, ASSE 6010, OSHA 10, competent person - excavation]
interview_length_min: 45
sections: {A_trade_skill: on, B_safety: on, C_code_and_test: on, G_backflow: off, H_med_gas: off, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [skips required tests/inspections before cover, enters unprotected trench > 5 ft, falsified license/certs, med gas work without 6010 when required]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Trade skill
| ID | Type | Question |
|---|---|---|
| PLB-A1 ★ | B | "Walk me through the underground and rough-in on the last commercial restroom group you ran. What did you check before calling for inspection?" |
| PLB-A2 ★ | T | "How do you decide the slope on a horizontal drain line?" |
| PLB-A3 ★ | T | "Explain venting. Why do we vent, and what goes wrong with a fixture that isn't vented properly?" |
| PLB-A4 | T | "Where do cleanouts go, and how do you keep them accessible?" |
| PLB-A5 | T | "Which pipe materials and joining methods have you used for water and DWV (copper, PEX, CPVC, PVC, cast iron no-hub, press)? What are the limits of each?" |
| PLB-A6 | T | "Installing a commercial water heater: what safety devices and connections are required?" |
| PLB-A7 | S | "Your sleeve or penetration lands in a beam, or the core isn't where the drawing shows it. What do you do?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| PLB-B1 ★ | T | "You're laying pipe in a 6-foot trench. What has to be in place before you get in?" |
| PLB-B2 | T | "Hot work and soldering or brazing in an occupied building: what precautions do you take?" |
| PLB-B3 | T | "When do you treat a space as a permit-required confined space (vault, pit, tank)?" |

## C. Code and testing
| ID | Type | Question |
|---|---|---|
| PLB-C1 ★ | T | "How do you test the DWV system and the water supply system before cover-up?" |
| PLB-C2 | T | "What does 'lead-free' mean for pipe and fittings used for drinking water?" |
| PLB-C3 | T | "Which code book do you work to here, and how do you look something up when you're not sure?" |
| PLB-C4 | T | "Fuel gas piping: how do you size it, test it, and bond it (including CSST)?" |

## G. Backflow (turn on if the role tests or installs assemblies)
| ID | Type | Question |
|---|---|---|
| PLB-G1 ★ | T | "What's the difference between an air gap, a double check, and an RP assembly? When is each one required?" |
| PLB-G2 | T | "Walk me through a field test on an RP assembly. What readings do you record?" |

## H. Medical gas (turn on for healthcare work)
| ID | Type | Question |
|---|---|---|
| PLB-H1 ★ | T | "What's different about brazing med gas pipe compared to domestic copper?" |
| PLB-H2 | T | "Who can install, inspect, and verify a med gas system, and what credential do you hold?" |

## D. Tools and tech
| ID | Type | Question |
|---|---|---|
| PLB-D1 | B | "Which tools and tech do you use: press tools, sewer cameras and locators, laser levels, layout apps, digital test gauges?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
Pick one:
- Read a plumbing isometric and give the pipe sizes, slopes, and fixture units. (Isometrics are 18% of the TN CMC-A exam.)
- Make up a solder or press joint and pressure-test it.
- Set the slope on a 20-ft run using a level and a rule.
