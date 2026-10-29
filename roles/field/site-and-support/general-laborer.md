# Role: General Laborer / Helper

Answer key: `answer-keys/field/site-and-support/general-laborer-KEY.md`
Benchmark: the NCCER Core Curriculum (basic safety, hand and power tools, construction drawings intro, communication, employability, material handling).

## Position tuning
```yaml
position_title: General Laborer    # Helper | Laborer | Apprentice
seniority: entry                # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: n/a   # see crew_assignment
crew_assignment: [polish, striping, low_voltage, general]
essential_physical_tasks: "e.g., lift/carry 50 lb, kneel/stand on concrete 8–10 hrs, push/pull grinder, work outdoors"  # confirm with the hiring manager
schedule: "?"   # nights/weekends/travel; ask
license_required: n/a
must_have_certs: n/a
must_have: [reliable transportation?, driver's license?]   # only if job-related
nice_to_have: [OSHA 10, NCCER Core]
interview_length_min: 25
sections: {A_skills: on, B_safety: on, C_reliability: on, D_field_tech_module: on, E_core: off}
knockouts: [refuses PPE/safety rules, dishonesty]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Skills
| ID | Type | Question |
|---|---|---|
| LAB-A1 ★ | B | "What construction or physical work have you done? What tools did you use every day?" |
| LAB-A2 | T | "Name the power tools you're comfortable with, and how you check one before using it." |
| LAB-A3 | T | "Read this tape measure: show me 7' 3-5/8"." (hand them a tape) |
| LAB-A4 | S | "The foreman tells you to do something you've never done before. What do you do?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| LAB-B1 ★ | T | "What PPE do you wear on a site where we're grinding concrete?" |
| LAB-B2 | S | "You see a coworker doing something unsafe. What do you do?" |
| LAB-B3 | T | "How do you lift something heavy, like a 60-lb bucket or a grinder head?" |

## C. Reliability
| ID | Type | Question |
|---|---|---|
| LAB-C1 ★ | B | "Tell me about a time you had to show up early, stay late, or travel for a job. How did you handle it?" |
| LAB-C2 | — | "Here are the essential tasks for this job [read the list]. Can you perform them, with or without reasonable accommodation?" (Ask every candidate the same way. **Don't** ask about health or medical history.) |

## D. Field tech module
| ID | Type | Question |
|---|---|---|
| LAB-D | — | FT-1 and FT-3 from the field tools module. |

## E. Core (off by default)
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.
