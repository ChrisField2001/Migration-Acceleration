# How Migration Acceleration Works

## The Flow In Plain English

A customer tells you they want to migrate. Here is exactly what you do, in order.

---

### Stage 1: Run one discovery call (30 minutes)
You ask the customer 10 core questions from the SE guide.
You write down answers as you go. Mark anything unknown as "Unknown".
You do not need all the answers. Unknowns are fine at this stage.

File to use: `docs/se-instructions-5-minute.md`

---

### Stage 2: Score what you heard (10 minutes)
After the call, score each answer 0, 1, or 2:
- 0 = Unknown or not started
- 1 = Partial or at risk
- 2 = Confirmed and evidenced

Calculate the weighted score and get a status:
- 0-49: Not Ready
- 50-79: Needs Pre-Work
- 80-100: Ready to Nominate

---

### Stage 3: The score tells you what to do next

**If score is Not Ready (0-49):**
- You have significant gaps
- Use the RACI doc to identify which specialist to bring in immediately
- Work with the customer PM to name an owner and date for every blocker
- Run a follow-up call to close the top gaps, then re-score

**If score is Needs Pre-Work (50-79):**
- You are close but not ready to nominate yet
- Work through the pre-work list with the customer before sending to Factory
- Bring in Security or Network specialists if those domains are scoring low
- Re-score once pre-work is done

**If score is Ready to Nominate (80-100):**
- Fill the nomination pack and send it to Factory
- No further pre-work needed before handoff

File to use: `docs/raci-and-escalation-matrix.md`

---

### Stage 4: Fill two output documents (10 minutes)
Regardless of status, always produce both outputs after the call:

Output 1: Readiness summary
- What is the score and status
- What are the top blockers with owner and date
- What is the dependency sequence
- What are the next 5 actions

Output 2: Factory nomination pack
- What is the scope
- What Azure services are expected
- What are the delivery assumptions
- What decisions are still open

File to use:
- `templates/loop-readiness-output-template.md`
- `templates/factory-nomination-pack-template.md`

---

### Stage 5: Share and track (5 minutes)
Send both outputs to CSU and Factory.
Log who you sent them to and whether rework was requested.
Submit 1-minute feedback on what friction you hit.

File to use:
- `templates/feedback-form-template.md`
- `docs/pilot-kickoff-and-tracker.md`

---

### Stage 6: Delivery teams take over
Once Factory accepts the nomination, the pre-sales acceleration is complete.
CSA, Factory, and delivery teams run the migration from here.
Your role is done until the next wave or the next account.

---

## Summary (One Line Per Stage)

| Stage | What You Do | Time |
|---|---|---|
| 1 | Ask 10 questions on a customer call | 30 min |
| 2 | Score each answer and get a status | 10 min |
| 3 | Act on the status: fix gaps or nominate | Varies |
| 4 | Fill readiness output and nomination pack | 10 min |
| 5 | Share outputs and log feedback | 5 min |
| 6 | Hand off to Factory and delivery teams | Done |

Total SE time for a clean engagement: approximately 55 minutes.

---

## Short Answer
This framework is a pre-delivery accelerator.
It does not migrate workloads itself.
It removes the delays that usually happen before migration delivery can start.

It is explicitly a pre-sales structure for better discovery, gap identification, and faster specialist engagement.

It does that by forcing fast clarity on:
- Scope
- Dependencies
- Ownership
- Readiness
- Nomination quality for CSU or Factory

## What Problem This Solves
Most migrations slow down before engineering starts because:
- Scope is vague
- Dependencies are not sequenced
- No named owner for blockers
- Landing zone and security readiness are unclear
- Intake to delivery teams is incomplete, causing rework

This toolkit is designed to reduce those failures in week 1 to week 3 of an engagement.

## What This Is Not
- Not a replacement for CSA services
- Not a replacement for Factory services
- Not a replacement for delivery engineering
- Not a replacement for customer governance

## What This Is
- A way to capture complete pre-sales information in one pass
- A way to identify gaps before nomination
- A way to trigger the right specialist teams early
- A way to improve handoff quality so delivery can start faster

## The Operating Structure

### Step 1: Discovery Capture (One Call)
Owner: SE
Duration: 30 minutes

Action:
- Ask 10 core questions once
- Record unknowns clearly

Output:
- Raw Q1-Q10 discovery answers

### Step 2: Readiness Scoring
Owner: SE with AI support
Duration: 10 minutes

Action:
- Score each answer 0, 1, or 2
- Apply weighted scoring
- Classify status

Output:
- Readiness score
- Status band: Not Ready / Needs Pre-Work / Ready to Nominate

### Step 3: Pre-Work Definition
Owner: SE + customer PM + technical owners
Duration: 15 minutes

Action:
- Convert gaps into blocker list
- Add owner and date for each blocker
- Define dependency sequence

Output:
- Actionable pre-work plan

### Step 4: Factory Intake Generation
Owner: SE with AI support
Duration: 10 minutes

Action:
- Transform discovery + pre-work into nomination pack
- Separate facts, assumptions, and open decisions

Output:
- Nomination-ready handoff for CSU or Factory

### Step 5: Share and Feedback
Owner: SE + CSU or Factory
Duration: 5 minutes

Action:
- Share the two outputs
- Capture friction in 1-minute feedback

Output:
- Fast quality loop for process improvement

## Specialist Engagement Triggers
Use these triggers to bring in the right team quickly.

- Bring in CSA when:
	- Scope or architecture assumptions are unclear
	- Modernization path is undecided
	- Platform readiness is partial and needs technical design support

- Bring in Factory when:
	- Nomination pack has stable scope and dependencies
	- Blockers have named owners and target dates
	- Delivery assumptions are clear enough for planning

- Bring in Security specialists when:
	- Identity controls are incomplete
	- Compliance obligations are unclear
	- Security baseline decisions are blocking progress

- Bring in Network specialists when:
	- DNS/routing ownership is unclear
	- Connectivity design is not approved
	- External dependency lead times threaten the timeline

## Why This Accelerates Migration
Acceleration comes from reducing time lost in rework.

Without structure:
- Multiple calls to gather basic facts
- Handoffs rejected for missing detail
- Blockers discovered too late

With this structure:
- One call to get baseline clarity
- One pass to generate handoff artifacts
- Early visibility of blockers and ownership
- Better nomination quality and less rework

## What "Done" Looks Like For One Account
You are done with the acceleration stage when all are true:
- Wave-1 scope is explicit
- Top dependencies are sequenced
- Top blockers have owner and date
- Readiness status is clear
- Nomination pack is sent and reviewable by CSU or Factory

## Files To Use In This Repo
- Start guide for SE run: docs/se-instructions-5-minute.md
- Readiness output template: templates/loop-readiness-output-template.md
- Nomination pack template: templates/factory-nomination-pack-template.md
- Feedback template: templates/feedback-form-template.md
- Detailed program spec for leads: docs/merged-prototype-spec.md

## Practical Example Timeline (First 5 Business Days)
- Day 1: Run 30-minute discovery interview
- Day 1: Produce readiness score and blocker list
- Day 2: Confirm owners and due dates
- Day 2: Generate nomination pack
- Day 3: Review with CSU or Factory
- Day 4-5: Close highest-risk pre-work items

## Success Metrics
- Time from first call to first nomination pack
- Number of rework requests from CSU or Factory
- Number of blockers with named owner and date
- Time to move from Not Ready to Needs Pre-Work or Ready
