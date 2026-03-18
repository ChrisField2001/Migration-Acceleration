# How Migration Acceleration Works

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
