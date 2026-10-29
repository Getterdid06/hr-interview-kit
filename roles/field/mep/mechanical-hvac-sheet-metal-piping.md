# Role: Mechanical: HVAC-R / Mini-Split, Sheet Metal and Ductwork, Mechanical Piping (Hydronic, Gas)

Answer key: `answer-keys/field/mep/mechanical-hvac-sheet-metal-piping-KEY.md`
Trade group: **MEP**.

Benchmarks (verify current editions per `update-checklist.md`):
- **EPA Section 608.** Types I, II, III, and Universal. Required to buy or handle most refrigerants. It doesn't expire.
- **AIM Act technology transitions.** These rules move new equipment to A2L refrigerants (R-454B, R-32).
- **SMACNA *HVAC Duct Construction Standards: Metal and Flexible*, 4th Ed.** Covers duct pressure classes, seal classes, reinforcement, and hangers. The SMACNA *HVAC Air Duct Leakage Test Manual* covers leakage testing.
- **NCCER** HVAC (4 levels) and Sheet Metal (4 levels) curricula. **UA** (pipefitter and HVAC-R) and **SMART/ITI** (sheet metal) registered apprenticeships.
- **Codes:** International Mechanical Code and International Fuel Gas Code, in the editions the AHJ has adopted. Use the codes adopted by the state and locality where the job is. TN's adopted codes are listed by the State Fire Marshal. **VA:** 2021 IPC, 2021 IMC, and 2021 IFGC, adopted through the 2021 USBC (Virginia Construction Code), effective **1/18/2024**; VA amendments are in VCC §2801.1.3 (IMC), §2801.1.4 (IFGC), and §2901.1.1 (IPC). The 2024 VA code cycle is still in rulemaking (not yet effective). https://www.dhcd.virginia.gov/codes · https://law.lis.virginia.gov/admincode/title13/agency5/chapter63/section10/ (checked 2026-10-29) **GA:** 2024 IPC, 2024 IMC, and 2024 IFGC with Georgia amendments, effective **1/1/2026** (DCA amendment packets marked "Revised January 1, 2026"). https://dca.georgia.gov/community-assistance/construction-codes/current-state-minimum-codes-construction (checked 2026-10-29) Confirm local amendments.
- **Licensing:** licensed per the state and locality where the work is (primary VA; offices GA and TN).
  - **VA** (DPOR Board for Contractors, Tradesmen program):
    - journeyman and master HVAC licenses
    - a Residential HVAC Mechanic license, added 4/1/2025 (no commercial work)
    - gas fitter and LP gas fitter are separate licenses
    - there's no apprentice license
  - **GA** (Construction Industry Licensing Board, Rule 121-3-.04): Conditioned Air Class I (up to 175,000 BTU heating and 60,000 BTU cooling) and Class II (unrestricted)
- **TN licensing (Board for Licensing Contractors):**
  - Jobs of **$25,000 or more** need a contractor license with **CMC or CMC-C (HVAC)** classification.
  - Under $25,000, where the Fire Marshal inspects, HVAC permits are pulled under a **Limited Licensed Electrician (LLE)** license.
  - Many cities and counties run their own licensing. Check the local codes office.
- Nice to have: NATE, A2L safety training, OEM mini-split / VRF certification, ASME Section IX or AWS brazing qualification (needed on some specs).

## Position tuning
```yaml
position_title: Mechanical Technician        # Helper | Installer | Service Tech | Sheet Metal Mechanic | Pipefitter | Lead
seniority: mid                                # entry | mid | senior
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: [mini_split/VRF install, RTU set & service, duct fab/install, hydronic piping, gas piping, EMS/thermostat integration]
sub_specialties: [S1_hvac_r, S2_sheet_metal, S3_piping]   # turn on only what the job needs; each maps to a section toggle
license_required: "?"      # per the state and locality of the job; e.g., VA: DPOR journeyman/master HVAC (gas fitter separate); GA: Conditioned Air Class I/II; TN: CMC-C held by the company or local mechanical journeyman card
must_have_certs: [EPA 608 Type II or Universal]   # required if S1 is on and they will handle refrigerant
nice_to_have: [NATE, A2L training, NCCER HVAC/Sheet Metal, OEM VRF cert, brazing qualification, OSHA 10]
interview_length_min: 45
sections: {B_safety: on, S1_hvac_r: on, S2_sheet_metal: off, S3_piping: off, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [venting refrigerant, handles refrigerant without 608, works energized/unlocked equipment without justification, falsified license/certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## B. Safety (all sub-specialties)
| ID | Type | Question |
|---|---|---|
| HV-B2 ★ | T | "Electrical safety on a condenser or RTU: what do you do before you open the panel?" |
| MB-2 | T | "On a roof setting or servicing a unit, what fall protection do you use?" |
| MB-3 | T | "Hot work: what has to happen before you braze or weld inside an occupied building?" |

## S1. HVAC-R / mini-split
| ID | Type | Question |
|---|---|---|
| HV-A1 ★ | B | "Walk me through a ductless mini-split install, from mounting to startup." |
| HV-A2 ★ | T | "How do you pressure test and evacuate a system? What micron level and decay test do you look for?" |
| HV-A3 | T | "How do you make a flare connection that won't leak?" |
| HV-A4 | T | "How do you charge a system? When do you use superheat, and when subcooling?" |
| HV-A5 | T | "What's different about working with A2L refrigerants like R-454B or R-32?" |
| HV-A6 | T | "What do you do when you braze copper line sets?" |
| HV-C1 ★ | S | "A rooftop unit is short-cycling and the space is warm. Walk me through your diagnosis." |
| HV-C2 | S | "A walk-in cooler is icing up on the evaporator. What do you check?" |
| HV-B1 ★ | T | "What are the rules for recovering refrigerant, and what does EPA 608 certification let you do?" |

## S2. Sheet metal and ductwork
| ID | Type | Question |
|---|---|---|
| SM-1 ★ | T | "How do you know how to build, seal, and reinforce a duct run? Where does that come from?" |
| SM-2 | T | "How do you lay out and hang a rectangular trunk line with branch takeoffs? Hanger spacing, supports, and access?" |
| SM-3 | T | "What do you do where a duct passes through a fire-rated wall or floor?" |
| SM-4 | S | "The duct shop drawing doesn't fit. There's a beam and a sprinkler main where your duct is supposed to go. What do you do?" |
| SM-5 | T | "How is a duct leakage test done, and what makes one fail?" |
| SM-6 | B | "Have you worked from coordinated BIM models or shop drawings on a tablet? How did it change your work?" |

## S3. Mechanical piping (hydronic, condensate, fuel gas)
| ID | Type | Question |
|---|---|---|
| MP-1 ★ | T | "Walk me through pressure testing a new hydronic or gas line before it's covered up." |
| MP-2 | T | "Which joining methods have you used (press, grooved, threaded, brazed, welded)? When is each one allowed?" |
| MP-3 | T | "How do you fill, flush, and purge air from a hydronic loop?" |
| MP-4 | T | "How do you size and slope condensate drains, and where do they terminate?" |
| MP-5 | S | "You smell gas near a unit you just piped. What do you do?" |

## D. Tools and tech
| ID | Type | Question |
|---|---|---|
| HV-D1 | B | "What tools or apps do you use: digital manifolds and probes, wireless gauges, manufacturer commissioning apps, service software?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo (pick one per enabled sub-specialty)
- **S1:** Make a flare and leak-test it, or read the gauge and temperature values you're given and calculate superheat or subcooling.
- **S2:** Read a duct shop drawing and identify the pressure class, seal class, gauge, and hanger spacing, or assemble a fitting with the correct seams.
- **S3:** Read a piping isometric and give the test medium, the test pressure source (spec or code), and the duration; or make up a press or threaded joint.
