# Role: Drywall: Metal Framing, Hanging, Finishing (Taping), Fire-Rated Assemblies

Answer key: `answer-keys/field/drywall/drywall-metal-framing-KEY.md`
Trade group: **Drywall**.

## Benchmarks (verify current editions per `update-checklist.md`)

**Levels of finish**
- **GA-214, *Levels of Finish for Gypsum Panel Products*** (Gypsum Association; 2026 ed. published, 2021 PDF public) defines Levels 0–5:
  - **Level 1:** tape embedded. For plenums and smoke barriers.
  - **Level 2:** tile substrate.
  - **Level 3:** heavy texture.
  - **Level 4:** flat paint or light texture.
  - **Level 5:** full skim coat. For gloss or dark paint, or critical lighting.

**Application, framing, and assemblies**
- **ASTM C840:** application and finishing of gypsum board.
- **ASTM C754:** installation of steel framing.
- **ASTM C645:** non-structural steel framing members.
- **GA-216:** application and finishing of gypsum panel products.
- **GA-600**, the *Fire Resistance and Sound Control Design Manual*.
- **UL Product iQ:** fire-resistance designs, e.g., U400 walls and partitions, V400, W400. The listed design must be built exactly as written.

**CSI sections**
- 09 21 16: gypsum board assemblies
- 09 22 16: non-structural metal framing
- 09 29 00: gypsum board

**Training**
- **NCCER Drywall** (Carpentry curriculum family).
- Union carpenter / drywall finisher (IUPAT) apprenticeships.

## Position tuning
```yaml
position_title: Drywall Mechanic      # Helper | Framer/Hanger | Finisher/Taper | Lead | Foreman
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
scope: [metal_framing, hanging, finishing]    # pick one or more
work_types: [interior partitions, rated corridor/shaft walls, ceilings/soffits, patch & repair in occupied space, Level 5 walls]
license_required: n/a
must_have_certs: [OSHA 10]
nice_to_have: [NCCER, union apprenticeship completion, scissor/MEWP training, OSHA 30]
interview_length_min: 40
sections: {A_framing: on, B_safety: on, C_finishing: on, H_hanging: on, R_rated: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [changes a fire-rated assembly without approval, disregards fall protection/scaffold rules, falsified certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Metal framing
| ID | Type | Question |
|---|---|---|
| DRY-A1 ★ | B | "Walk me through laying out and framing a run of interior partitions from the drawings." |
| DRY-A2 | T | "How do you pick stud gauge and spacing? What tells you the limit?" |
| DRY-A3 | T | "Your partition goes to the deck. How do you attach the top, and why?" |
| DRY-A4 | T | "Where do you add blocking or backing, and who tells you where it goes?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| DRY-B1 ★ | T | "Working on a rolling scaffold (a Baker) or stilts: what rules do you follow?" |
| DRY-B2 | T | "How do you control dust when you sand, especially in an occupied building?" |
| DRY-B3 | T | "How do you handle and carry board safely?" |

## C. Finishing
| ID | Type | Question |
|---|---|---|
| DRY-C1 ★ | T | "The spec says Level 4 in the corridors and Level 5 in the lobby. What's the difference in what you do?" |
| DRY-C2 | T | "Walk me through taping a wall with joint compound. What coats, which compound, and what drying time?" |
| DRY-C3 | T | "Where do control joints go?" |
| DRY-C4 | S | "The painter says your walls are flashing and you can see joints under the light. What do you do?" |

## H. Hanging
| ID | Type | Question |
|---|---|---|
| DRY-H1 ★ | T | "How do you lay out the board on a wall and a ceiling: direction, joints, and around openings?" |
| DRY-H2 | T | "What board types have you hung (Type X, Type C, moisture/mold resistant, abuse, shaftliner, cement board)? Where does each go?" |
| DRY-H3 | T | "Screw spacing and depth: what's right, and what goes wrong if you overdrive?" |

## R. Fire-rated assemblies
| ID | Type | Question |
|---|---|---|
| DRY-R1 ★ | T | "The drawings say 'UL U419, 1-hour.' What does that mean for how you build the wall?" |
| DRY-R2 ★ | S | "An electrician cut an oversize hole in a rated wall. What do you do?" |
| DRY-R3 | T | "How do you handle the head of a rated wall where it meets a fluted deck?" |

## D. Tools and tech
| ID | Type | Question |
|---|---|---|
| DRY-D1 | B | "Which tools do you run: automatic tapers and boxes, laser layout, screw guns with depth nose, powder-actuated tools, HEPA sanders?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
Pick one:
- Lay out and frame a 4-ft section with the track fastened and studs at the given spacing.
- Hang one sheet and fasten it to the given spacing.
- Tape and bed an inside corner and a flat joint.
