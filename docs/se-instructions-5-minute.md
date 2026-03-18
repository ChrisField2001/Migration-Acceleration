# SE Instructions - First Run Guide (Beginner Friendly)

## Read This First
This page is written for any SE, including first week in role.
You do not need deep migration experience to run this.

This process is not replacing CSA, Factory, or delivery teams.
It helps you collect complete pre-sales information and escalate to the right specialists faster.

Your job is simple:
- Ask 10 questions
- Capture answers
- Share 2 outputs

## Goal
Use one workflow to quickly assess migration readiness and produce a Factory nomination pack for an active NHS account.

## What To Do In Order (No Guesswork)
1. Start customer call and ask the 10 core questions in this file.
2. Keep answers short. Mark unknowns as "Unknown".
3. Score each question 0, 1, or 2.
4. Copy results into readiness template.
5. Copy scope and assumptions into nomination template.
6. Share both files with CSU/Factory.

## What You Need Before Starting
- Current discovery notes
- Known blockers and dependencies
- Target timeline
- Customer stakeholders and owners

If you do not have all items, still continue and mark gaps as "Unknown".

## What To Say On The Call (Suggested Script)
"I will ask 10 short questions so we can quickly identify blockers, ownership, and next actions. If something is unknown, that is fine and we will capture it."

## 5-Minute Flow
1. Open your chosen entry point (Copilot prompt workflow, Copilot Studio agent, or Power App).
2. Choose one mode:
- Option 1: Run Readiness Assessment
- Option 2: Generate Factory Intake
- Option 3: Do Both (recommended)
3. Paste or upload discovery notes.
4. Answer guided questions (keep unknowns explicit).
5. Export outputs to Loop using templates in this repo.
6. Share with CSU/Factory/partner.
7. Submit feedback in under 1 minute.

## The Only Questions You Need To Ask
Ask these in order and stop there unless a trigger fires later.

1. What business outcome and deadline are we committing to in this wave?
2. Which workloads are in scope for wave 1, and what is explicitly out of scope?
3. What are the top 3 dependencies (identity, network, data) that must land before migration?
4. Are identity controls ready (MFA, CA, privileged access model)?
5. Is landing zone and networking path approved (DNS, connectivity, policy)?
6. Are platform quotas, subscriptions, and environments ready (dev/test/uat/prod)?
7. Who owns each blocker and by when (named owner + target date)?
8. What modernization opportunities are viable now (replatform/refactor), not later?
9. What security uplift opportunities should be bundled into the wave?
10. What 1-2 AI opportunities are practical in 6-8 weeks with measurable value?

## Simple Answer Format To Capture During Call
- Q1:
- Q2:
- Q3:
- Q4:
- Q5:
- Q6:
- Q7:
- Q8:
- Q9:
- Q10:

## Good Input Example
- "Identity federation agreed but conditional access exceptions unresolved; DNS cutover dependent on third-party provider timeline; quota increase requested but not approved yet."

## What Good Output Looks Like
- Clear readiness status and score
- Blockers with owners and dates
- Explicit dependency sequence
- Nomination pack with assumptions and open decisions

## Common Mistakes to Avoid
- Hiding unknowns in narrative text
- Missing owner for critical blocker
- Mixing assumptions with confirmed facts
- Sending nomination without dependency clarity

## Exit Criteria Before You Share
- At least top 5 actions identified
- Every blocker has owner or "owner missing"
- Open questions are decision-ready
- CSU/Factory can understand context without extra meetings

## 30-Minute Core Interview (Weighted)
Use this after the call notes are captured.

Scoring per question:
- 0 = Unknown / no evidence
- 1 = Partial / at risk
- 2 = Confirmed / evidenced

Weighted readiness score:
- `Weighted Score (%) = sum((response_score / 2) * weight)`
- Target thresholds:
- 80-100 = Ready to Nominate
- 50-79 = Needs Pre-Work
- 0-49 = Not Ready

Quick scoring example:
- If Question 2 has weight 12 and score 1, contribution is 6 points.
- If Question 2 has score 2, contribution is 12 points.

| # | Core Question | Weight | Why It Matters |
|---|---|---:|---|
| 1 | What business outcome and deadline are we committing to in this wave? | 8 | Aligns migration scope and delivery urgency. |
| 2 | Which workloads are in scope for wave 1, and what is explicitly out of scope? | 12 | Prevents scope drift and failed nominations. |
| 3 | What are the top 3 dependencies (identity, network, data) that must land before migration? | 12 | Surfaces sequencing risk early. |
| 4 | Are identity controls ready (MFA, CA, privileged access model)? | 10 | High security and access risk if unclear. |
| 5 | Is landing zone and networking path approved (DNS, connectivity, policy)? | 12 | Common blocker for migration execution. |
| 6 | Are platform quotas, subscriptions, and environments ready (dev/test/uat/prod)? | 8 | Avoids preventable deployment delays. |
| 7 | Who owns each blocker and by when (named owner + target date)? | 12 | Ownership clarity is critical to unblock progress. |
| 8 | What modernization opportunities are viable now (replatform/refactor), not later? | 8 | Captures value beyond lift-and-shift. |
| 9 | What security uplift opportunities should be bundled into the wave? | 8 | Raises resilience and compliance posture. |
| 10 | What 1-2 AI opportunities are practical in 6-8 weeks with measurable value? | 10 | Ensures innovation is scoped to near-term outcomes. |

Total weight = 100

## Conditional Follow-Ups (Only Ask If Needed)
Do not ask deep follow-ups unless the core question scores 0 or 1.

- Trigger A (Identity scored 0-1):
	- Which apps require legacy auth and exception paths?
	- What CA policies block current user journeys?
- Trigger B (LZ/Network scored 0-1):
	- Where are DNS/routing ownership boundaries unclear?
	- What external lead times exist (third-party network/provider)?
- Trigger C (Scope/Dependency scored 0-1):
	- Which upstream systems can delay cutover?
	- What is the minimum viable wave if dependency is delayed?
- Trigger D (Ownership scored 0-1):
	- Which blocker has no accountable owner today?
	- What is the escalation path and decision date?
- Trigger E (AI opportunity scored 0-1):
	- Which repetitive workflow has clear baseline metrics today?
	- What data can safely ground an AI pilot?

## Minimal Data Contract (Required Every Time)
Capture only these fields if time is tight:
- Customer and wave-1 scope
- Target date
- Top 3 blockers
- Blocker owners + dates
- Dependency sequence
- Open decisions

Everything else is optional unless a trigger fires.

## First-Time SE Definition Of Done
You are done for this account when all items below are true:
- You asked all 10 core questions
- You have top 3 blockers and owners
- You have a dependency sequence
- You shared both templates with CSU/Factory
