# Role: Equipment Operator (Skid Steer, Forklift/Telehandler, Aerial Lifts, Mini-Excavator, Ride-on Grinders/Scrubbers, Truck and Trailer)

Answer key: `answer-keys/field/site-and-support/equipment-operator-KEY.md`
Benchmarks:
- NCCER Heavy Equipment Operations assessments.
- OSHA 1926.602 (earthmoving equipment) and 1910.178 (powered industrial truck operator training, referenced for construction forklifts by 1926.602(d)).
- ANSI A92.22/A92.24 (MEWP safe use and training).
- OSHA 1926.1427 / NCCCO for crane operators only, if cranes are ever in scope.
- 811 Call-Before-You-Dig.

## Position tuning
```yaml
position_title: Equipment Operator
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: n/a   # see equipment_list
equipment_list: [skid steer, forklift/telehandler, scissor/boom lift, mini excavator, ride-on grinder, truck+trailer]   # trim to what the job uses
cdl_required: "?"           # ask: GVWR of truck + trailer combos
license_required: n/a   # CDL: see cdl_required
must_have_certs: [forklift/MEWP training records (employer evaluation will be done)]
nice_to_have: [NCCER HEO, NCCCO (crane only), OSHA 10]
interview_length_min: 35
sections: {A_skills: on, B_safety: on, C_maintenance: on, D_field_tech_module: on, E_core: on, F_seat_test: on}
knockouts: [skips pre-shift inspections, digs without locates, falsified license/CDL]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Skills
| ID | Type | Question |
|---|---|---|
| OP-A1 ★ | B | "Which machines have you run, for how many hours, and on what kind of work? Which are you best on?" |
| OP-A2 ★ | T | "Walk me through your pre-shift inspection on a skid steer or telehandler." |
| OP-A3 | T | "How do you load and secure a machine on a trailer?" |
| OP-A4 | T | "How do you read a load chart on a telehandler or forklift?" |
| OP-A5 | S | "You need to dig a trench for conduit outside the building. What do you do before the bucket touches the ground?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| OP-B1 ★ | S | "A spotter isn't available, and you have to back a machine through a busy area. What do you do?" |
| OP-B2 | T | "What are the main hazards with scissor and boom lifts, and how do you control them?" |

## C. Maintenance
| ID | Type | Question |
|---|---|---|
| OP-C1 | B | "What maintenance have you done yourself? Tell me about a breakdown you found early." |

## D. Field tech module
| ID | Type | Question |
|---|---|---|
| OP-D1 | B | "Have you used telematics, machine apps, digital inspection checklists, or GPS grade control?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Seat test
| ID | Type | Question |
|---|---|---|
| OP-F | W | Seat test: a pre-use inspection walk-around and a short maneuver course on the machine the job needs, with the same course for every candidate. |
