# Calibration Log

Record every change to questions, anchors, ★ flags, weights, thresholds, or the practical test. Do a quarterly review: compare interview scores with the 90- and 180-day results in the feedback log.

**Rules for changes**
1. Wait for at least **5 hires** in a role (or 10 interviews) before you change thresholds for that role.
2. A question with no variance (everyone scores the same) or no link to on-the-job results is a candidate for rewording or removal.
3. **Adverse impact check:** If selection rates for any group fall below **4/5 (80%)** of the highest group's rate, review the questions and the test for job-relatedness (Uniform Guidelines, 29 CFR 1607.4D). Use voluntary, separately stored self-ID data only. Never use it in the interview.
4. Cite the source of any external change (a standard revision, a new law).

## Template
```markdown
### [YYYY-MM-DD] — v[x.y]
- File(s) changed:
- What changed (before → after):
- Why (evidence: N interviews/hires, pattern seen, or external source + URL):
- Approved by:
```

## Entries
### 2026-10-29 — v1.0
- Initial kit created. Anchors are expert-drafted from public standards (see `sources.md`). They have **not yet been validated** against local hire results.

### 2026-10-29 — v1.1
- **File(s) changed:** field roles reorganized into trade-group folders.
  - **New:**
    - `roles/field/mep/mechanical-hvac-sheet-metal-piping.md` and `roles/field/mep/plumber.md`
    - `roles/field/drywall/drywall-metal-framing.md`
    - `roles/field/painter/painter.md`
    - `roles/field/finishes/finishes-installer.md`
    - `roles/field/flooring/flooring-installer.md` and `roles/field/flooring/flooring-scope-reference.md`
    - A matching key for each role under `answer-keys/field/<group>/`
  - **Moved (mv, not deleted):**
    - The electrician file to `mep/`
    - The carpenter file to `carpenter/`, expanded to rough plus finish (new CAR-G1–G6)
    - The polisher file to `flooring/`
    - Striping, laborer, operator, and foreman to `site-and-support/`
  - **Archived:** the HVAC file and key went to `archive/`. Its content was folded into Mechanical S1, with the HV- IDs unchanged.
- **What changed:** new questions and anchors for the trades above. HVAC anchors are unchanged. Carpenter now has a `scope` toggle. Flooring has a `floor_types` selector.
- **Why:** owner request to organize by MEP / Carpenter / Drywall / Painter / Finishes / Flooring and to add mechanical and plumber roles. Sources are in `sources.md` §7.
- **Validation status:** the new anchors are expert-drafted from public standards and **not yet validated**. Per the change rules, wait for 5 hires per role before changing thresholds.
- **Approved by:** Michael Indelicato, 2026-10-29 13:48 ET (relayed by Chief Of Staff; quoted "Approve v1.2 as the working version")

### 2026-10-29 — v1.2 (working version; renamed from v1.2-draft on approval)
- **File(s) changed:** `README.md`, `00-system-prompt.md`, `02-legal-guardrails.md`, `sources.md`, `update-checklist.md`, this log, every role file under `roles/`, every answer key under `answer-keys/`, and `tests/estimator-10-minute-practical.md`. Snapshot of v1.1 before the edits: `archive/v1.1-2026-10-29/` and `archive/hr-construction-interview-kit-v1.1.zip`.
- **What changed (before → after):**
  - **Company description:** unchanged. A `PENDING MICHAEL: company description` comment sits above README line 3 and 00 §1.
  - **Law reference:** README and 00 point to `/workspace/research/ai-hiring-laws-by-state-2026-10-29.md` as canonical; `ai-hiring-laws-by-state.md` in the kit is labeled a mirror. Both copies kept (byte-identical on 2026-10-29).
  - **README:** v1.2; "Quick start, today" block with a sample plumber tuning block; field-tools module moved to its own "Field add-on (all field roles)" row; archive rows added for the v1.1 snapshot and zip.
  - **00:** v1.2 line; §2 table reordered to the README load order with `archive/**` last; Type legend (B/T/S/W) from 01 §1; §3 timing points to 01 §6; §5 threshold table removed ("use the thresholds in 01 §4"); §7 "Probes (if the role file has them)".
  - **Thresholds reconciled to 01 §4:** labels Entry/apprentice, Mid/journeyman, Senior/lead/foreman; Hold bands 2.2–2.49, 2.7–2.99, 3.2–3.49 (the same as 00's old "within 0.3 below"). No numeric change.
  - **Format (Document Creator review):** `## <Code>. <Name>` section headings in the ten flat role files and every key; shared letters B Safety, D Tools/tech, E Core, F Skills demo; section order A, B, C, optional trade sections, D, E, F; toggle keys `<Code>_<short_name>`; one tuning-key set in every role file (`n/a` where a key doesn't apply; extra keys kept); key titles `KEY — Role`; flooring "Floor types" line above the YAML.
  - **ID renames (role file and key together; anchors unchanged):** drywall DRY-B1–B3 → DRY-H1–H3 (Hanging) and DRY-S1–S3 → DRY-B1–B3 (Safety); painter PNT-S1–S3 → PNT-B1–B3; finishes FIN-S1–S2 → FIN-B1–B2. Toggle renames: drywall `B_hanging` → `H_hanging`, `S_safety` → `B_safety`; painter and finishes `S_safety` → `B_safety`; finishes `CL/TL/MW/DR/SP/WC` → `CL_ceilings, TL_wall_tile, MW_millwork, DR_doors_hardware, SP_div10_specialties, WC_wall_coverings`; mechanical `S1/S2/S3` → `S1_hvac_r, S2_sheet_metal, S3_piping`.
  - **History moved here from the question files:** `concrete-finisher-polisher.md` was moved from `roles/field/` to `roles/field/flooring/` in v1.1. `mechanical-hvac-sheet-metal-piping.md` replaces the archived `hvac-refrigeration-minisplit-tech.md`; its questions are kept as sub-specialty S1 with the same HV- IDs (HV-B1 stays in S1).
  - **Anchors added:** electrician/LV key LV-F parts 1–3 (RJ45, RS-485, point list) and an FT-3 lens; striping key STR-D/E row and STR-F test-line option. Uncited numbers are marked `VERIFY:`.
  - **Estimator practical (Lead Estimator review):** "Tell us" cut from 6 to 4 prompts; prioritization line added; AI/automation added to the approach prompt; one-page text mock of A-101 added. Key rebuilt to 10 criteria (5 double-weighted, maximum 30, same bands), with a gate (mastic ≥ 1 and scale or area ≥ 1; senior mastic at 2), an old → new mapping, an ADA 208.2 interviewer aid, and a new hard-fail line. `estimator.md` notes: score EST-B1, EST-B2, and EST-D1 independently of the practical; LV is covered by interview questions only.
  - **Legal:** Tennessee E-Verify (35+ FTE, since 2023-01-01) added to `02-legal-guardrails.md` and `sources.md`; the statute section number is marked VERIFY.
  - **sources.md:** "Pending primary-source verification" section; no unverified citations added. **update-checklist.md:** v1.1 trade items verified present; Carpenter, TN E-Verify, and ADA parking lines added.
  - **Must-ask wording:** not changed to "2-4 per enabled section". Several enabled sections have 0–1 ★ questions (for example carpenter B, foreman sections, office sections), and 01 has no "2–4" text, so the wording wouldn't match how the files are built.
- **Why:** owner-directed format and content review. Credits: **Document Creator** (format review), **Lead Estimator** (practical test and estimator review). External sources: 2010 ADA Standards §208 (https://www.access-board.gov/ada/#ada-208) and TN.gov employment verification (https://www.tn.gov/workforce/employers/staffing-redirect/hiring-regulations/employment-verification.html), both checked 2026-10-29.
- **Scores:** no past interview scores changed. The new practical key applies to future interviews only.
  - **Standards check folded in (Data Specialist, `/workspace/research/construction-standards-verification-2026-10-29.md`):**
    - Tile coverage now reads "80% minimum, 95% for exterior or shower" (was "wet areas") in FIN-TL2, FLR-TILE1, and the scope reference.
    - Large-format flatness now reads "any edge 15 in.+: 1/8 in. in 10 ft and 1/16 in. in 2 ft", per A108.02 as quoted by CTEF (was "1/16 in. in 24 in."; same value).
    - NFPA 80 clearances added to FIN-DR3 and CAR-G4, tagged "per NFPA 80 2019; 2025 edition revised clearances, verify".
    - The C636 4 ft o.c. value in FIN-CL2 is tagged VERIFY.
    - PLB-C1 test values filled in from IPC §312. Its old "air test only where the manufacturer allows" line became "plastic piping may not be air-tested" (§312.3).
    - PLB-A2 gained the grease-interceptor footnote, and the plumber key gained a local TN jurisdiction note.
    - INSTALL is marked union (UBC) only, and FCICA CIM is marked a manager credential; neither is scored as a must-have for non-union installers.
    - F1344-21a and the CSI division titles were updated.
    - sources.md: confirmed items moved to §7 citations; partial items remain in Pending, with their evidence marked secondary/older edition.
  - **00 rewrite and HOW-TO-USE (Michael, via Chief Of Staff):**
    - `00-system-prompt.md` was rewritten as the complete master instructions. New sections cover the load order, how to read the tuning block, the end-to-end flow, keys staying interviewer-only, scoring with the practical's must-catch gate, a legal summary of 02, data privacy, one candidate per chat, the 30/90/180-day feedback and four-fifths loop, and staying current (next due 2027-01-31; all edits through HR Director). Not-legal-advice line added.
    - Kept: the Type legend, the file table, and the thresholds (in `01-…` §4 only).
    - New `HOW-TO-USE.md`: setup for a Claude Project, Custom GPT, or Copilot agent (no answer keys as shared knowledge), interview-day steps, follow-up logging, change routing, and do's and don'ts. Added to the README quick start and index.
  - **Law reference v2:**
    - Canonical file is now `/workspace/research/ai-hiring-laws-by-state-2026-10-29-v2.md`. The old kit mirror is archived as `archive/ai-hiring-laws-by-state-v1.md`; the new mirror is v2 plus a one-line header.
    - 00, README, and HOW-TO-USE point to v2, or to the newest file.
    - `02-legal-guardrails.md` AI section matches v2:
      - "Yes" states are 7: CA, CO (effective 1/1/2027), CT, IL, MD (narrow), NJ, and NYC. Texas is No (a general, intent-only law).
      - Tennessee has no AI-in-employment law; THRA and TDA cover 8+ employees.
      - The vendor-liability line from withdrawn EEOC guidance was removed. Colorado's 3-year retention line was dropped (not in v2).
      - Check the state's row before using an AI tool.
    - Credits: Data Specialist's recheck and Chief Of Staff's review. The reference lists 27 open items.
  - **Company correction (Michael, 2026-10-29, relayed via Chief Of Staff):**
    - Aggregate Trades LLC: commercial GC, HQ in Chesapeake, VA, with offices in Milton, GA and the Knoxville, TN area. Licensed for commercial construction in all 48 contiguous states. Replaces the "specialty contractor" description and the PENDING markers in README and 00 §1.
    - Michael: "we have the ability to self perform all." Every field role's tuning block gets `delivery: self-perform` (the default, so hands-on skill is scored) and an optional `sub_coordination_qa: off` toggle. When that toggle is on, the interviewer weights coordination and QA and documents the reason in `weights`.
    - Multi-state rework: Virginia is the primary state, with Georgia and Tennessee as office states. Every hire checks the rules of the job's state.
      - TN licensing and code content is kept and labeled TN. VA and GA code, licensing, license-lookup, and E-Verify items were added as VERIFY placeholders (pending Data Specialist). No VA or GA names or thresholds were added.
      - Files: 00, README, HOW-TO-USE, 02, update-checklist, sources, the plumber, electrician/LV, and mechanical role files and keys, and all 13 field role files.
      - PLB-C3's anchor now names the code of the job's state (TN 2021 IPC; VA and GA: VERIFY). No other anchor changed.
  - **VA/GA fold-in and law reference v3 (Data Specialist, `/workspace/research/va-ga-hiring-law-checks-2026-10-29.md`):**
    - Created `/workspace/research/ai-hiring-laws-by-state-2026-10-29-v3.md` from v2 (v2 untouched):
      - The home-state note now covers VA (primary), GA, and TN.
      - VA row: none found; HB 2094 veto and sustained veto, with the opening of the veto message; 2026 bills failed or continued; VCDPA exclusion.
      - GA row: nothing enacted; Special Session not searched.
      - Discrimination thresholds: VHRA 5+; GA narrow statutes; TN 8+; federal thresholds per statute, not rechecked.
      - Open items 28–32 added. The Yes count stays at 7.
    - Kit mirror: the v2 mirror was archived as `archive/ai-hiring-laws-by-state-v2.md` and the mirror refreshed to v3. Pointers in 00, README, 02, and sources now name v3.
    - `02-legal-guardrails.md`:
      - VA E-Verify (§40.1-11.2 state agencies; §2.2-4308.2 state contractors) and GA E-Verify (§36-60-6 and §13-10-91, Justia unofficial, still tagged VERIFY) replace the "pending Data Specialist" tags.
      - New home-state discrimination section.
      - VA and GA AI lines filled in.
    - Licensing VERIFY tags are filled with VA DPOR and GA Rule 121-3 classes in the plumber, electrician/LV, and mechanical role files and the README; the 00 cadence table names the boards. Keys still tag the VA and GA lookup pages (not opened). VA and GA code editions stay VERIFY and were added to the update-checklist as quarterly items.
    - `01-…` §5: the unsupported Colorado 3-year retention claim was replaced with a pointer to the job state's row (example: California's 4-year ADS records).
    - `sources.md` §8 adds every new citation (checked 2026-10-29), with GA Code items marked "Justia, unofficial".
- **Future items:** LV/EMS estimator practical variant (not written yet). FT key guidance for `expected_level` proficient/advanced. The electrician role file names no FT items for section D.
- **Validation status:** anchors are still expert-drafted and not validated against local hires.
- **Approved by:** Michael Indelicato, 2026-10-29 13:48 ET (relayed by Chief Of Staff; quoted "Approve v1.2 as the working version")

### 2026-10-29 — v1.2.1 (source corrections; working version stays usable)
- **File(s) changed:** `README.md`, `00-system-prompt.md`, `02-legal-guardrails.md`, `sources.md`, `update-checklist.md`, `ai-hiring-laws-by-state.md` (mirror of v4), this log, `roles/field/mep/plumber.md`, `roles/field/mep/mechanical-hvac-sheet-metal-piping.md`, `roles/field/flooring/flooring-scope-reference.md`, and the plumber, mechanical, electrician/LV, line-striping, and finishes keys. Snapshot of v1.2 first: `archive/v1.2-2026-10-29/`.
- **What changed:** VERIFY results folded in from `/workspace/research/hr-kit-verify-items-2026-10-29.md` (checked 2026-10-29): VA 2021 IPC/IMC/IFGC (USBC, eff. 1/18/2024) and GA 2024 IPC/IMC/IFGC (eff. 1/1/2026); DPOR and GOALS license lookups; official O.C.G.A. for GA E-Verify; VA has no private-employer E-Verify mandate (bulk data dated 8/13/2025); TN §50-1-703(b) and Pub. Ch. 622 (eff. 1/1/2027); LV untwist, bend-radius, length, and RS-485 values (secondary sources, labeled); MUTCD 4–6 in. stall lines; Setfast wet/dry mils (one product, labeled); Armstrong C636 note (secondary). New law reference `/workspace/research/ai-hiring-laws-by-state-2026-10-29-v4.md` (v3 untouched; 32 open items; Yes count 7).
- **No anchor, score, threshold, or question ID changed.** Remaining VERIFY items are listed in `update-checklist.md`.
- **Why:** primary or labeled secondary sources from the VERIFY pass Michael approved 2026-10-29 13:48 ET ("Yes, have Data Specialist check the VERIFY items").
- **Approved by:** pending Michael

