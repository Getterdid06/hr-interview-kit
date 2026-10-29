# How to Use This Kit

For Michael and the hiring managers at Aggregate Trades LLC. Plain steps, start to finish.

## What this is
A set of files that turns an AI assistant into a structured-interview helper. It builds the question sheet, helps you score answers, and gives a Go / Hold / No-Go **recommendation**. **You make the hiring decision. The AI only recommends.**

## One-time setup (pick one option)
Use a **business or enterprise plan** with **model training turned off**. Settings move around, so check each product's current settings and admin docs to confirm training is off before you add any candidate information.

**What every option gets:**
- **Instructions:** paste the whole of `00-system-prompt.md`.
- **Knowledge files (upload these five):**
  1. `01-interview-method-and-scoring.md`
  2. `02-legal-guardrails.md`
  3. `03-common-core-questions.md`
  4. `ai-hiring-laws-by-state.md` (the kit's copy of the newest law reference)
  5. `roles/field/flooring/flooring-scope-reference.md`

**Don't upload answer keys (`answer-keys/`) as shared knowledge.** Anyone who can use the project, GPT, or agent can get the AI to quote or summarize its knowledge files, and a key could end up on a candidate sheet. Keys stay interviewer-only, so paste the one you need into that candidate's chat only.

### Option A: Claude Project
1. Create a new Project.
2. Paste `00-system-prompt.md` into the project instructions.
3. Upload the five knowledge files.
4. Share the Project only with interviewers.

### Option B: Custom GPT (ChatGPT)
1. Create a new GPT.
2. Paste `00-system-prompt.md` into its instructions.
3. Upload the five knowledge files.
4. Keep it private to your workspace. Don't publish it publicly.

### Option C: Microsoft Copilot agent
1. Create a new agent.
2. Paste `00-system-prompt.md` into its instructions.
3. Add the five knowledge files.
4. Share it only with interviewers.

## Interview day (one candidate)
1. **Pick the role file** from `roles/office/` or `roles/field/`.
2. **Fill in its `Position tuning` block** with the hiring manager: seniority, sections on/off, certifications, interview length, and so on. For field roles, leave `delivery: self-perform` as is. Turn `sub_coordination_qa` on only if the job will be subbed. Then coordination and QA get more weight.
3. **Open a NEW chat for this one candidate.** Never mix candidates in a chat.
4. **Paste in:**
   - the filled-in role file
   - for field roles, `roles/field/field-tools-tech-module.md`
   - the matching answer key from `answer-keys/` (plus `answer-keys/03-common-core-KEY.md`, and the field-tools module key for field roles)
5. **Ask it:** "Build the interviewer sheet and the candidate sheet."
   - The **interviewer sheet** has the questions, anchors, and space for notes. It's for you only.
   - The **candidate sheet** has only what the candidate may see (such as the practical test instructions). Check that it has no anchors or answers.
6. **Keep the key on your side only.** Never print, show, or send it to a candidate.
7. **Estimator only, the 10-minute practical:**
   - Give the candidate `tests/estimator-10-minute-practical.md` (the scenario, the four "Tell us" prompts, and the one-page mock of sheet A-101 in its appendix), plus paper and a basic calculator.
   - Time it: 2 minutes to read, 7 minutes to talk or write, 1 minute for the top 3 RFIs. Just listen and take notes.
   - Paste `answer-keys/tests/estimator-10-minute-practical-KEY.md` into the chat to score it.
8. **Score.** Paste your notes. The AI scores each question 1–5 with quoted evidence.
9. **Get the recommendation:** Go, Hold, or No-Go, with strengths, risks, and reference-check questions. **Review it and make the decision yourself.**
10. **For every hire, check the law-reference row for the state where the job is** (Virginia, Georgia, Tennessee, or any of the 48 states) before using any AI tool for the hire.

## After the interview
- Save the log entry the AI drafts into `logs/interview-feedback-log.md`, using the **candidate ID only** (initials or the ATS ID), never a full name or ID numbers.
- For hires, add the supervisor's 1–5 rating at **30, 90, and 180 days**.

## Changes to the kit
**Send every change to HR Director.** Don't edit the kit files yourself. HR Director checks the source, archives the old file, makes the edit, and logs it.

## Do's and don'ts
- **Do** use a new chat for each candidate.
- **Do** use candidate IDs, not names, in logs.
- **Do** make the final call yourself.
- **Don't** paste SSNs, dates of birth, driver's license or other ID numbers, background checks, or medical information.
- **Don't** paste a resume until you've removed protected information such as a photo, age, date of birth, or marital status.
- **Don't** use recordings, video, or voice for scoring. Score what was said, from your notes.
- **Don't** ask about age, family, health, religion, national origin, citizenship (only "authorized to work in the U.S."), arrests, or credit. See `02-legal-guardrails.md`.
- **Don't** send anything to a candidate without Michael's yes.

---
Not legal advice. Confirm with employment counsel for each state where you hire.
