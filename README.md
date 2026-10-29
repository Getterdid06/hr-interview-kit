# HR in Construction: Interview Kit (v1.2.1, 2026-10-29)

This is an LLM-ready set of Markdown files for structured hiring at Aggregate Trades LLC. Aggregate Trades LLC is a commercial general contractor headquartered in Chesapeake, Virginia, with offices in Milton, Georgia and the Knoxville, Tennessee area. It is licensed for commercial construction and works in all 48 contiguous states (not Alaska or Hawaii). Its scopes include concrete polishing, grind-and-seal, and flooring; pavement striping and line marking; low-voltage and energy-management-system (EMS) work; MEP (HVAC and mechanical, plumbing, and electrical); carpentry, drywall and metal framing, painting, and finishes; and general field support. The company can self-perform all of these scopes and also manages subcontractors when a job calls for it. It hires field trades, site and support roles, and office staff. Every hire follows the rules of the state where the job is; Virginia is the primary state, and Georgia and Tennessee are office states. Field roles are organized by trade group (v1.1): **MEP** (mechanical, plumber, electrician/LV), **Carpenter**, **Drywall**, **Painter**, **Finishes**, and **Flooring**, plus site and support roles.

## Quick start, today
0. New to the kit? Read `HOW-TO-USE.md` first. It covers one-time setup (Claude Project, Custom GPT, or Copilot agent) and interview-day steps.
1. Paste `00-system-prompt.md` into the LLM, then `01-interview-method-and-scoring.md`, `02-legal-guardrails.md`, and `03-common-core-questions.md`.
2. Paste the role file and fill in its `Position tuning` block with the hiring manager. Example below.
3. For a field role, add `roles/field/field-tools-tech-module.md`.
4. Keep the matching answer key in the interviewer's view only.
5. Score with the key, decide with `01-…` §4, and log the result in `logs/interview-feedback-log.md`.

**Example: filled-in tuning block for `roles/field/mep/plumber.md`** (sample values only; confirm each one with the hiring manager before the interview):
```yaml
position_title: Plumber            # Helper/Apprentice | Journeyman | Lead/Foreman | Service Plumber
seniority: mid                     # entry | mid | senior
delivery: self-perform             # default; the company can self-perform every listed scope
sub_coordination_qa: off           # on only when the job is subbed
work_types: [commercial rough-in, water heaters, gas piping, service/repair]
code_at_job: "2021 IPC (TN statewide)"   # sample for a TN job; VA: 2021 IPC (USBC, eff. 1/18/2024); GA: 2024 IPC + GA amendments (eff. 1/1/2026); confirm local amendments
license_required: "TN LLP"         # sample for a TN job; VA/GA classes in plumber.md; confirm per job location
must_have_certs: [OSHA 10]
nice_to_have: [UA/NCCER Plumbing level, ASSE 5110, competent person - excavation]
interview_length_min: 45
sections: {A_trade_skill: on, B_safety: on, C_code_and_test: on, G_backflow: off, H_med_gas: off, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [skips required tests/inspections before cover, enters unprotected trench > 5 ft, falsified license/certs, med gas work without 6010 when required]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: "Service-heavy opening; ask the gas piping questions."
```


## How to use it
1. Load **`00-system-prompt.md`** into the LLM first, as the system prompt or first message.
2. Add `01-interview-method-and-scoring.md`, `02-legal-guardrails.md`, and `03-common-core-questions.md`.
3. Add the **role file** for the opening. Edit its `Position tuning` YAML block (seniority, project type, certifications, section on/off toggles).
4. For field roles, also add `roles/field/field-tools-tech-module.md`.
5. Add the matching **answer key** from `answer-keys/`. It's for the interviewer only: **never share it with candidates**. Store it in a folder candidates can't reach.
6. After each interview, append an entry to `logs/interview-feedback-log.md`. Fill in the 30/90/180-day results later.
7. Every quarter, say "run the update check" and work through `update-checklist.md`. Record changes in `logs/calibration-log.md`.

## Index
| Path | Purpose |
|---|---|
| `HOW-TO-USE.md` | Plain-language setup and interview-day steps for Michael and hiring managers |
| `00-system-prompt.md` | Complete master instructions for the LLM: role, load order, tuning block, interview flow, scoring, legal and privacy rules, feedback loop, staying current |
| `01-interview-method-and-scoring.md` | Structured interview method, 1–5 anchors, Go/Hold/No-Go thresholds |
| `02-legal-guardrails.md` | EEOC do's and don'ts, AI-tool laws, testing rules, record retention |
| `03-common-core-questions.md` | CORE-1–10 questions for every role (data handling, AI, tool impact, safety culture) |
| **Office roles** (systems-oriented) | |
| `roles/office/estimator.md` | Takeoff and estimating systems, AI takeoff verification, bid data |
| `roles/office/project-manager.md` | PM platforms, change orders, WIP and forecasting, document control |
| `roles/office/project-coordinator-apm.md` | Submittals, RFIs, closeout, document control |
| `roles/office/accounting.md` | Job costing, WIP and revenue recognition, AP/AR, retainage, lien waivers, payroll and certified payroll |
| `roles/office/office-manager-admin.md` | Admin systems, onboarding, compliance tracking, data security |
| `roles/office/procurement-purchasing.md` | POs, vendor data, lead times, 3-way match |
| **Field roles** (skill-level), by trade group | |
| *MEP* | |
| `roles/field/mep/mechanical-hvac-sheet-metal-piping.md` | Sub-specialty toggles. **S1 HVAC-R/mini-split:** EPA 608, evacuation, A2L refrigerants. **S2 sheet metal:** SMACNA, dampers, leakage testing. **S3 piping:** hydronic, gas, condensate. Also state licensing (VA DPOR HVAC, GA Conditioned Air, TN CMC-C/LLE). |
| `roles/field/mep/plumber.md` | DWV slope and venting, testing, lead-free, fuel gas, backflow (ASSE 5110), med gas (ASSE 6010/NFPA 99), state and local licensing (VA DPOR, GA Rule 121-3, TN LLP/CMC-A), 2021 IPC (TN) |
| `roles/field/mep/electrician-low-voltage-tech.md` | EMS/BAS, RS-485, CTs, cabling, NFPA 70E, networks; state licensing (VA DPOR plus ESC/FAS/DCJS, GA Electrical and LV classes, TN LLE) |
| *Carpenter* | |
| `roles/field/carpenter/carpenter.md` | **Rough:** forms, layout, blocking, fall protection. **Finish:** trim, casework (ANSI/AWI 0620), doors, NFPA 80. Scope toggle. |
| *Drywall* | |
| `roles/field/drywall/drywall-metal-framing.md` | Metal framing (C754/C645), hanging, GA-214 levels 0–5, UL-rated assemblies, head-of-wall details |
| *Painter* | |
| `roles/field/painter/painter.md` | SSPC/AMPP surface prep, DFT (PA 2), coatings, wall coverings, EPA RRP / OSHA lead |
| *Finishes* | |
| `roles/field/finishes/finishes-installer.md` | Sub-specialty toggles: ACT ceilings (C636/E580), wall tile (TCNA), millwork, doors/frames/hardware (NFPA 80, ADA), Div 10 specialties, FRP and wall coverings |
| *Flooring* | |
| `roles/field/flooring/flooring-installer.md` | Floor-type selector covering prep, polish, grind and seal, epoxy/urethane cement, MMA, LVT/LVP, VCT, sheet vinyl, rubber, carpet, tile, terrazzo, and wood |
| `roles/field/flooring/concrete-finisher-polisher.md` | Polishing and grind-and-seal at full depth (CPC, ACI 310.1, CSP, silica) |
| `roles/field/flooring/flooring-scope-reference.md` | Reference (no key): SOW steps, CSI sections, standards, and tools for every floor type and floor prep |
| *Site and support* (not part of the six trade groups; kept as is) | |
| `roles/field/site-and-support/line-striping-pavement-marking.md` | Layout, MUTCD, ADA, equipment, materials |
| `roles/field/site-and-support/general-laborer.md` | Entry level, safety, reliability |
| `roles/field/site-and-support/equipment-operator.md` | Inspections, loading, 811, MEWPs, seat test |
| `roles/field/site-and-support/foreman-superintendent.md` | Crew leadership, safety, production tracking, daily reports |
| *Field add-on (all field roles)* | |
| `roles/field/field-tools-tech-module.md` | Add-on for every field role (FT-1–6): time, photos, plans, daily reports |
| **Tests** | |
| `tests/estimator-10-minute-practical.md` | Candidate-facing 10-minute estimator test (polish, grind-and-seal, striping) |
| **Answer keys (interviewer only)** | |
| `answer-keys/03-common-core-KEY.md` | Core question anchors |
| `answer-keys/office/*-KEY.md` | Go/No-Go anchors and knockouts per office role |
| `answer-keys/field/<trade-group>/*-KEY.md` | Go/No-Go anchors and knockouts per field role, in the same subfolders as `roles/field/` (module key at `answer-keys/field/field-tools-tech-module-KEY.md`) |
| `answer-keys/tests/estimator-10-minute-practical-KEY.md` | Worked answers and 30-point rubric (10 criteria, 5 double-weighted) |
| **Reference** | |
| Newest `ai-hiring-laws-by-state-*.md` in `/workspace/research/` (currently `ai-hiring-laws-by-state-2026-10-29-v4.md`) | **Canonical** AI-in-hiring law reference: federal, 50 states, and DC. Maintained outside the kit; read alongside `02-legal-guardrails.md`. |
| `ai-hiring-laws-by-state.md` | Kit mirror of the canonical file above. Refresh it from the canonical copy; don't edit the mirror directly. |
| **Archive** (retired; nothing deleted) | |
| `archive/roles/field/hvac-refrigeration-minisplit-tech.md` and `archive/answer-keys/field/hvac-refrigeration-minisplit-tech-KEY.md` | Folded into Mechanical S1 in v1.1, with the same HV- question IDs. Kept for reference. |
| `archive/zips/hr-construction-interview-kit-v1.0.zip` | The v1.0 zip as it was before this restructure |
| `archive/v1.1-2026-10-29/` | Snapshot of every v1.1 file, taken before the v1.2 edits |
| `archive/hr-construction-interview-kit-v1.1.zip` | The v1.1 zip as it was before the v1.2 re-zip |
| `archive/ai-hiring-laws-by-state-v1.md` | The kit law-reference mirror as it was before the v2 refresh |
| `archive/ai-hiring-laws-by-state-v2.md` | The kit law-reference mirror as it was before the v3 refresh |
| `archive/v1.2-final-pre-vaga-2026-10-29/` | Copies of files overwritten by the VA/GA fold-in and law v3 pass |
| `archive/v1.2-2026-10-29/` | Snapshot of every v1.2 file, taken before the v1.2.1 VERIFY fold-in |
| `archive/v1.2-draft-pre-rewrite-2026-10-29/` | Copies of files overwritten by the 00 rewrite, HOW-TO-USE, law v2, and multi-state passes |
| **Learning loop** | |
| `logs/interview-feedback-log.md` | Per-interview record plus 30/90/180-day results |
| `logs/calibration-log.md` | Change history and adverse-impact checks |
| `update-checklist.md` | Quarterly legal, standards, software, and data refresh |
| `sources.md` | All citations with URLs, plus known gaps |

## Adding a new trade
Put it in the matching trade-group subfolder under `roles/field/` and `answer-keys/field/`. Copy any field role file and its key. Change the benchmark line, the tuning block, and the questions. Keep the IDs unique, flag 2–4 ★ must-pass questions, write GO/NO-GO anchors, and add a line in `logs/calibration-log.md`.

## Important
- Anchors are expert-drafted from public standards. They aren't validated against your hires yet, so calibrate before relying on hard cutoffs.
- The kit gives the interviewer a recommendation. A person makes the hiring decision.
- Not legal advice. Have employment counsel review it before use, for each state where you hire, and before using any AI scoring tool.
