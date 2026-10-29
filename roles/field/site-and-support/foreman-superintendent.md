# Role: Foreman / Crew Lead / Superintendent (field-office hybrid)

Answer key: `answer-keys/field/site-and-support/foreman-superintendent-KEY.md`
Benchmarks:
- OSHA "competent person" duties (for example, silica 1926.1153 requires a written exposure control plan and a competent person to implement it).
- OSHA 30-hour Outreach. It's a course card, not a certification.
- The CMAA Standards of Practice (quality, safety, schedule).
- AGC Supervisory Training Program topics.

## Position tuning
```yaml
position_title: Foreman            # Crew Lead | Foreman | General Foreman | Superintendent
seniority: senior               # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: n/a   # see trade_focus
trade_focus: [polish, striping, low_voltage, multi-trade]
crew_size_expected: "?"            # ask
software_we_use: [time app?, daily report app?, Procore?, CompanyCam?]
license_required: n/a
must_have_certs: [OSHA 30 card preferred, valid driver's license if driving company vehicles]
nice_to_have: [AGC STP, ASCC CPC Craftsman (polish), ATSSA (striping), first aid/CPR]
interview_length_min: 50
sections: {A_leadership: on, B_safety: on, C_production_quality: on, D_systems_and_reporting: on, E_core: on, F_trade_module: on}   # F = 3–4 ★ items from the matching trade file
knockouts: [tolerates unsafe work to hit schedule, falsifies time/daily reports, falsified credentials]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Leadership
| ID | Type | Question |
|---|---|---|
| FS-A1 ★ | B | "Tell me about a time a crew member wasn't performing or kept showing up late. What did you do?" |
| FS-A2 | B | "How do you plan tomorrow's work before you leave today?" |
| FS-A3 | S | "The GC super wants you to start in an area that isn't ready (other trades, wet slab, no power). What do you do?" |
| FS-A4 | B | "How have you trained a new helper on the job?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| FS-B1 ★ | B | "Walk me through your morning safety routine: JHA or pre-task plan, toolbox talks." |
| FS-B2 ★ | S | "A crew member refuses to wear a respirator during grinding because it's hot. What do you do?" |
| FS-B3 | S | "There's an injury on your crew. Walk me through the first 30 minutes." |

## C. Production and quality
| ID | Type | Question |
|---|---|---|
| FS-C1 ★ | B | "How do you track production (SF per day, LF per day) against the estimate? What do you do when you're behind?" |
| FS-C2 | B | "How do you do quality control before you call the GC for inspection?" |

## D. Systems and reporting
| ID | Type | Question |
|---|---|---|
| FS-D1 ★ | B | "What goes in your daily report, and what app or system have you used to submit it? What do the photos need to show?" |
| FS-D2 | B | "How have you documented extra work or a change in the field so the company gets paid?" |
| FS-D3 | B | "How do you check that your crew's time is coded to the right job and cost code?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Trade module
| ID | Type | Question |
|---|---|---|
| FS-F | — | Pull 3–4 ★ questions from the trade file that matches the crew: MEP (mechanical, plumber, electrician/LV), carpenter, drywall, painter, finishes, flooring (including polisher), or striping. |
