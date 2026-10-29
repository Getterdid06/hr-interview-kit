# Role: Estimator (Concrete Polish / Grind-and-Seal / Striping / Low-Voltage)

Answer key: `answer-keys/office/estimator-KEY.md` · Practical test: `tests/estimator-10-minute-practical.md`
Standards this role is benchmarked against: ASPE Certified Professional Estimator (general estimating knowledge, trade-specific test, technical paper) and AACE Certified Estimating Professional (scope definition, estimate validation, risk/contingency, communicating estimates).

## Position tuning (fill in before each interview)
```yaml
position_title: Estimator            # e.g., Junior Estimator, Senior Estimator, Chief Estimator
seniority: mid                       # entry | mid | senior | lead
work_types: n/a   # see project_types
project_types: [polish, grind_and_seal, striping]   # add: low_voltage_EMS, coatings, mixed
bid_volume_expected: "X bids/week"   # ask the hiring manager; don't assume
software_we_use: [Bluebeam Revu, Excel]   # list the actual company stack, e.g., Togal, PlanSwift, STACK, ProEst
license_required: n/a
must_have_certs: []                  # e.g., none; ASPE CPE nice-to-have
nice_to_have: [ASPE CPE, AACE CEP, ASCC CPC Tradesman]
interview_length_min: 60
sections:
  A_estimating_core: on
  B_systems_and_software: on
  C_data_management: on
  D_ai_tools: on
  E_tool_impact: on        # pulls CORE-2/3
  F_practical_test: on     # 10-min test
knockouts: [falsified credentials, would bid without scope review, would share confidential bid data in public AI]
weights: equal             # document a reason if changed
notes_for_today: ""
```

## A. Estimating core
| ID | Type | Question | Probes |
|---|---|---|---|
| EST-A1 ★ | B | "Walk me through your process on the last bid you won, from invitation to submitted proposal." | Bid/no-bid decision? Plan review? Takeoff? Pricing? Review? |
| EST-A2 ★ | T/S | "On a polished concrete spec, what information do you need before you can price it?" | Class/level? Existing condition? Joints? Square footage by area? |
| EST-A3 | T | "How do you build a production rate for grinding or polishing, or for striping linear feet? Where do the numbers come from?" | Historical job cost? Equipment size? Number of passes? |
| EST-A4 ★ | B | "Tell me about a scope gap or mistake you caught before bid day, or one you missed. What happened?" | How was it found? What changed in your process? |
| EST-A5 | S | "Your price is 18% higher than the next bidder. What do you check?" | Scope comparison, quantities, rates, assumptions? |
| EST-A6 | T | "What goes in your inclusions/exclusions and clarifications for a grind-and-seal plus striping bid?" | Moisture, adhesive removal, protection, after-hours, ADA compliance, layout? |
| EST-A7 | B | "How do you handle RFIs and addenda during bidding?" | Logging, deadlines, who answers, how the change reaches the takeoff? |
| EST-A8 (senior) | B | "How do you hand a won job over to the PM and field so the estimate becomes the budget?" | Cost codes, assumptions, production rates, the handoff meeting? |

## B. Systems and software
| ID | Type | Question | Probes |
|---|---|---|---|
| EST-B1 ★ | T | "Which takeoff tools have you used (Bluebeam, Togal, PlanSwift, STACK, On-Screen Takeoff)? Walk me through setting up a takeoff in your best one." | Scale calibration? Layers or markup sets? Exporting? |
| EST-B2 | T | "How do you make sure the scale on a PDF is right?" | Dimension check, multiple sheets, "NTS" sheets? |
| EST-B3 | B | "What estimating or pricing system have you used: Excel templates, STACK, ProEst, Sage Estimating, custom? How was it set up?" | Assemblies? Locked formulas? Versions? |
| EST-B4 | T | "How do you compare revisions when a new drawing set comes out?" | Bluebeam Overlay/Compare, Togal compare, slip-sheeting? |
| EST-B5 | B | "Which systems has your estimate fed into after award (Procore, Sage, QuickBooks)?" | Did cost codes match? |

## C. Data management
| ID | Type | Question | Probes |
|---|---|---|---|
| EST-C1 ★ | B | "How do you keep a cost database or historical production rates current?" | Who updates it? How often? Job-cost feedback? |
| EST-C2 | B | "How do you organize bid folders and track bid status/hit rate?" | Bid log, CRM, win/loss reasons? |

## D. AI tools
| ID | Type | Question | Probes |
|---|---|---|---|
| EST-D1 ★ | S | "If an AI takeoff tool gives you 11,400 SF for a floor, what do you check before using it?" | Scale, excluded areas, a manual spot check, equipment pads, columns? |
| EST-D2 | B | "Have you used AI to read specs, write proposals, or summarize addenda? What went right and what went wrong?" | Hallucinated spec section? Confidentiality? |

## E. Tool impact
Use CORE-2 and CORE-3 from `03-common-core-questions.md` (estimator lens).

## F. Practical
Run `tests/estimator-10-minute-practical.md`. It counts as one ★ score.

- **Score independently:** score EST-B1, EST-B2, and EST-D1 on their own answers, independently of the practical. Don't carry a practical result (for example, the scale trap) into those scores, or the reverse.
- **Low-voltage / EMS:** the practical covers polish, grind-and-seal, and striping only. For LV/EMS estimating, use the interview questions only. An LV practical variant is logged as a future item in `logs/calibration-log.md`.
