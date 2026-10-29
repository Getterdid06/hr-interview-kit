# Role: Electrician / Low-Voltage and Energy Management (EMS) Technician

Answer key: `answer-keys/field/mep/electrician-low-voltage-tech-KEY.md`
Benchmarks:
- NCCER Electrical assessments.
- **BICSI** Installer 1 / Installer 2 / Technician (cabling, termination, testing).
- **NICET** (fire alarm and other low-voltage systems).
- **NFPA 70 (NEC)** — use the edition adopted locally.
- **NFPA 70E** (electrical safety in the workplace).
- **Licensing:** licensed per the state and locality where the work is (primary VA; offices GA and TN). Check state and local electrical and low-voltage licensing for the job location.
  - **TN** (Board for Licensing Contractors): the Limited Licensed Electrician (LLE) covers electrical work under $25,000 where the local jurisdiction accepts it.
  - **VA** (DPOR Board for Contractors, Tradesmen program):
    - journeyman and master electrician licenses
    - there's no apprentice license
    - low voltage is a contractor-firm specialty: ESC (electronic/communication service, 50 V or less) and FAS (fire alarm systems, 50 V or less)
    - DCJS registers electronic security technicians (Va. Code §9.1-139; the DCJS site itself wasn't opened)
  - **GA** (Construction Industry Licensing Board, Rule 121-3):
    - Electrical Contractor Class I (single-phase installations up to 200 A at the service) and Class II (unrestricted)
    - Low Voltage LV-A (alarm and general), LV-G (general), LV-T (telecommunication and general), and LV-U (unrestricted)

## Position tuning
```yaml
position_title: Low-Voltage / EMS Technician   # Electrician Helper | Journeyman | LV Tech | EMS Commissioning Tech
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: n/a   # see system_types
system_types: [EMS/BAS controllers, metering/CTs, BACnet/Modbus networks, structured cabling, cellular/VPN gateways]
license_required: "?"   # per the state and locality of the job; e.g., VA: DPOR journeyman/master electrician (firm ESC/FAS for LV; DCJS for security); GA: Electrical Class I/II or LV-A/G/T/U; TN: LLE or local journeyman card; confirm with the hiring manager
must_have_certs: [OSHA 10]
nice_to_have: [BICSI INST1/INST2/TECH, NICET, NCCER Electrical, OEM controller certs]
interview_length_min: 45
sections: {A_trade_skill: on, B_safety: on, C_data_network: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [works energized without justification/PPE, no LOTO, falsified license]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Trade skill
| ID | Type | Question |
|---|---|---|
| LV-A1 ★ | B | "Tell me about the last EMS, BAS, or controls install you did. What devices, what wiring, and how did you check it out?" |
| LV-A2 ★ | T | "How do you wire and terminate an RS-485 (BACnet MS/TP or Modbus RTU) trunk? What causes communication problems?" |
| LV-A3 | T | "How do you install current transformers (CTs) for energy metering? What mistakes do you look for?" |
| LV-A4 | T | "What's the difference between Class 1 and Class 2 circuits, and why does it matter for separation and routing?" |
| LV-A5 | T | "Terminate and test a Cat6 run: what standard and what tester?" |
| LV-A6 | S | "A controller shows offline in the cloud dashboard after your install. Walk me through troubleshooting." |

## B. Safety
| ID | Type | Question |
|---|---|---|
| LV-B1 ★ | T | "You need to land CT leads or a controller power feed in an energized panel. What do you do?" |

## C. Data and network
| ID | Type | Question |
|---|---|---|
| LV-C1 | T | "What do you need to know about IP addressing, VLANs, or VPN gateways to get a site controller online without causing problems on the customer's network?" |
| LV-C2 | B | "How do you document an install so someone else can service it (point lists, labels, as-builts, photos)?" |

## D. Field tech module
Add questions from `roles/field/field-tools-tech-module.md` (FT-1 to FT-6). Score them with its key.

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
| ID | Type | Question |
|---|---|---|
| LV-F | W | Skills demo: terminate an RJ45 and test it; land a 3-wire RS-485 segment on a terminal block with the shield handled correctly; read a point list. |
