# 02 — Legal Guardrails (brief; not legal advice)

## Never ask, before an offer (EEOC)
- Race, color, ethnicity, national origin, ancestry. "What language do you speak at home?" is out. You *may* ask whether they can speak, read, or write English or Spanish **if the job requires it**.
- Religion, church, religious holidays. You may state the schedule and ask whether they can work it.
- Sex, sexual orientation, gender identity, pregnancy, plans for children, childcare, marital status, spouse's name or job.
- Age or graduation year. Only confirm legal minimum age, such as 18+ for hazardous occupations.
- **Disability, medical conditions, medications, workers' comp history, or genetic and family medical history.** You *may* describe the essential physical tasks (for example, "lift 50 lb, kneel and work on concrete for long periods, work at heights, operate a 600-lb ride-on grinder") and ask: "Can you perform these tasks, with or without reasonable accommodation?" You may also ask them to *demonstrate* a task if every candidate is asked.
- Citizenship. Instead ask: "Are you legally authorized to work in the U.S.?" Verify with Form I-9 / E-Verify **after** the offer.
- Arrest records. Treat conviction questions with care: follow state and local ban-the-box rules and EEOC guidance (individualized assessment).
- Height, weight, photos, club or organization memberships that reveal a protected class.
- Financial or credit history, unless the job requires it and you follow the FCRA. This applies mainly to accounting roles.
- Unemployment status as a disqualifier.

## Allowed and encouraged
- Required licenses and certifications: driver's license with a clean MVR for driving roles, CDL, EPA 608, state or local trade licenses for the job's state (for example, TN LLE), OSHA 10/30 card, NCCCO, and so on.
- Ability to work the stated schedule, travel, overnight jobs, and night or weekend shifts.
- Drug and alcohol testing per a written company policy applied to all candidates for the role.
- Ability to perform the essential functions listed in the job description.

## Using an LLM or AI in hiring (this kit)
Source: the newest `ai-hiring-laws-by-state-*.md` in `/workspace/research/` (currently `ai-hiring-laws-by-state-2026-10-29-v4.md`; kit mirror `ai-hiring-laws-by-state.md`). Status as of 2026-10-29.
- **States:** the company is headquartered in Virginia (primary state), with offices in Georgia and Tennessee, and works in all 48 contiguous states. **For a job or hire in any state, the interviewer checks that state's row in the law reference before using an AI tool.**
- **Federal law applies to any selection tool, AI or not.** Title VII (disparate treatment and disparate impact), the ADA (no screening out people who could do the job with an accommodation), and the ADEA (no age proxies such as graduation year) apply. EEOC's AI guidance pages were removed in early 2025; the statutes didn't change. Keep a human decision-maker.
- **Adverse impact:** under the Uniform Guidelines (29 CFR 1607), a selection rate for any group below 80% of the highest group's rate is a red flag that needs review. Collect demographics only through voluntary self-ID, kept apart from interviewers and from this LLM.
- **No video, voice, or face analysis.** This kit scores answer content only.
- **States with an AI-in-employment law ("Yes" in the reference): 7.**
  - **California:** Civil Rights Council automated-decision-system regulations, effective 10/1/2025, plus later laws. See the CA row.
  - **Colorado:** SB 26-189, effective 1/1/2027, for decisions made with automated decision-making that materially influences employment. AG rules are pending, and enforcement is currently stayed in *xAI v. Weiser*. See the CO row.
  - **Connecticut:** Public Act 26-15. Using an automated employment-decision tool is no defense to a discrimination complaint (from 10/1/2026), and written pre-decision notice applies to tools deployed on or after 10/1/2027.
  - **Illinois:** 775 ILCS 5/2-102(L), effective 1/1/2026: no AI that discriminates and no zip-code proxies, with notice of AI use. The AI Video Interview Act (820 ILCS 42) requires notice, an explanation, and consent if AI analyzes video interviews for Illinois-based positions.
  - **Maryland (narrow):** no facial-recognition template during an interview without the applicant's signed waiver.
  - **New Jersey:** N.J.A.C. 13:16 disparate-impact rules cover automated employment decision tools. Test for adverse impact before use, and give applicants a way to request an accommodation.
  - **New York City:** Local Law 144. An automated employment decision tool needs a bias audit within one year before use, public audit information, and notice 10 business days before use.
- **Texas: No** (TRAIGA is a general AI law and intent-only: it bars intentional AI discrimination, and disparate impact alone isn't enough).
- **Tennessee:** no AI-in-employment law was found (site-limited search, not exhaustive). The Tennessee Human Rights Act and Tennessee Disability Act apply to AI-assisted decisions the same as to human ones, for employers with **8 or more employees**. E-Verify applies at 35+ FTE (below).
- **Virginia (primary):** no private-employer AI-hiring law found as of 2026-10-29. HB 2094 was vetoed (3/24/2025) and the veto sustained (4/2/2025); the 2026 bills were left in committee or continued to 2027 (screened by short bill description only). The VCDPA profiling opt-out excludes applicant and employee data (§59.1-576(C)(14)).
- **Georgia:** no AI-in-employment law enacted in the 2025–2026 Regular Session. SB 167 and SB 164 stalled, and HB 1351 is state agencies only. The 2026 Special Session signed only SB 3EX (elections).
- The law reference lists **32 open items**. Treat anything it marks unverified as unconfirmed.
- Don't paste candidates' SSNs, DOBs, or background-check reports into the LLM. Use initials or a candidate ID in logs.

## State discrimination-law coverage (home states)
These laws apply to AI-assisted decisions the same as to human ones.
- **Virginia:** the Virginia Human Rights Act covers employers with **5 or more employees** (Va. Code §2.2-3905(A)). "Age" means 40 or older.
- **Georgia** (Justia, unofficial): there's no general private-employer anti-discrimination statute in the sections checked. The narrow statutes are:
  - sex-based pay, §34-5-2 (10+ employees)
  - age, §34-1-2 (ages 40–70)
  - disability, §34-6A-2 (15+ employees)
  - GA FEPA (§45-19-22) covers **state agencies only**.
- **Tennessee:** the THRA and TDA cover employers with **8 or more employees**.
- **Federal:** Title VII and the ADA (15+) and the ADEA (20+) still apply at their own thresholds (federal thresholds per statute, not rechecked here).

## Employment eligibility (E-Verify by state)
Check the rule for the state where the new hire will work. Primary state Virginia; office states Georgia and Tennessee.
- **Tennessee E-Verify:** private employers with **35 or more full-time-equivalent employees** must use E-Verify for new hires (Tennessee Lawful Employment Act, Tenn. Code Ann. § 50-1-703(b), per the official TN code on LexisNexis, checked 2026-10-29). In effect since **Jan 1, 2023**. Per TN.gov, the employee count includes employees inside or outside Tennessee under the same FEIN, and the page lists penalties for non-compliance. Run it after the offer, as in the Citizenship line above, and the same way for every new hire. Source: https://www.tn.gov/workforce/employers/staffing-redirect/hiring-regulations/employment-verification.html (checked 2026-10-29).
  - **Dated note (2026-10-29):** 2026 Pub. Ch. 622 (HB 1194/SB 990), effective **1/1/2027**, amends §50-1-702(13) from "at least six (6) employees" to "at least one (1) employee" and rewrites the §50-1-703(f)(3) penalty (show compliance within 45 days of a final order or the business license is suspended; until remedied for a 1st or 2nd violation, permanently for a 3rd or later). The 35-FTE threshold in §50-1-703(b) is unchanged by the act; recheck it after 1/1/2027. https://publications.tnsosfiles.com/acts/114/pub/pc0622.pdf · https://wapp.capitol.tn.gov/apps/BillInfo/Default?BillNumber=HB1194&ga=114 (checked 2026-10-29)
- **Virginia E-Verify:**
  - Va. Code §40.1-11.2 covers **state agencies only**.
  - §2.2-4308.2 covers employers with **more than an average of 50 employees** for the previous 12 months **and** a state-agency contract **over $50,000**. The penalty is debarment from state-agency contracting for **up to 1 year**.
  - §2.2-4317(E) (prequalification denial) is the only other hit. A search of all 76 Code of Virginia titles found **no private-employer E-Verify mandate**. That search used the LIS bulk Code CSVs dated **8/13/2025**, so VERIFY: recheck the VA LIS for 2026 session changes. https://law.lis.virginia.gov/law-library · Sources: https://law.lis.virginia.gov/vacode/40.1-11.2/ · https://law.lis.virginia.gov/vacode/2.2-4308.2/ (checked 2026-10-29).
- **Georgia E-Verify** (official O.C.G.A., LexisNexis for the GA Code Revision Commission, checked 2026-10-29):
  - O.C.G.A. §36-60-6 covers **private employers with more than 10 employees**, counted as of **January 1** of the year. Official text: "Every private employer with more than ten employees shall register with and utilize the federal work authorization program". An E-Verify affidavit is required for a local business license or occupational tax certificate. The section history shows an amendment by Ga. L. 2025, p. 1029; VERIFY what it changed (full text is behind a CAPTCHA).
  - §13-10-91(a) (public employers must register and participate) is confirmed in the official text. The contractor/subcontractor provisions below come from Justia (unofficial); VERIFY that subsection's text in the official O.C.G.A.: §13-10-91 requires a **signed, notarized E-Verify affidavit** for public contracts for the physical performance of services, flowed down to **every subcontractor tier**. A false affidavit conviction brings a **12-month bar** from public contracts.
  - No Georgia law on AI in hiring was found (2026 Regular and Special Sessions checked).
  - Sources: official O.C.G.A. https://advance.lexis.com/container?config=00JAAzZDgzNzU2ZC05MDA0LTRmMDItYjkzMS0xOGY3MjE3OWNlODIKAFBvZENhdGFsb2fcIFfJnJ2IC8XZi1AYM4Ne (checked 2026-10-29) · unofficial cross-check for the §13-10-91 subcontractor text: https://law.justia.com/codes/georgia/title-13/chapter-10/article-3/section-13-10-91/
- **Other states where a job is:** check that state's rule before the first hire there.
- This is a brief, not legal advice. Confirm your FTE count and obligations with employment counsel.

Sources are in `sources.md` §Legal.
