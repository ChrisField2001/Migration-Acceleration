# Discovery Assessment Summary (Initial Call)

## Input Source
- File: `test/se-instructions-5-minute.md`
- Assessment type: Initial discovery call (early-stage)

## Weighted Scoring
Scoring scale per question:
- 0 = Unknown / no evidence
- 1 = Partial / at risk
- 2 = Confirmed / evidenced

Formula:
- Weighted Score (%) = sum((response_score / 2) * weight)

| Question | Weight | Score | Weighted Contribution |
|---|---:|---:|---:|
| Q1 Business outcome and deadline | 8 | 2 | 8 |
| Q2 Wave-1 scope clarity | 12 | 1 | 6 |
| Q3 Top dependencies | 12 | 1 | 6 |
| Q4 Identity readiness | 10 | 1 | 5 |
| Q5 Landing zone/network readiness | 12 | 1 | 6 |
| Q6 Quota/subscription/environment readiness | 8 | 0 | 0 |
| Q7 Blocker ownership and dates | 12 | 1 | 6 |
| Q8 Modernization opportunities now | 8 | 1 | 4 |
| Q9 Security uplift opportunities | 8 | 1 | 4 |
| Q10 AI opportunities in 6-8 weeks | 10 | 0 | 0 |

Total weighted score: 45/100

## Readiness Status
- Status: Not Ready
- Threshold band:
- 80-100 = Ready to Nominate
- 50-79 = Needs Pre-Work
- 0-49 = Not Ready

## What This Means
This is a normal result for a first discovery call. The output is still useful because it clearly identifies pre-work required before nomination.

## Priority Gaps To Close First
1. Platform readiness not confirmed (subscriptions, quota, environments)
2. Ownership/dates for blockers not explicit
3. Scope and dependencies not detailed enough for nomination quality
4. AI use case intentionally deferred (acceptable), but should be tracked as deferred decision

## Triggered Follow-Ups (Minimum Set)
- LZ/Network:
  - Who owns DNS and routing decisions?
  - What are lead times for network/security approvals?
- Scope/Dependency:
  - Which systems are in scope for wave 1 by name?
  - What is out of scope in this wave?
- Ownership:
  - What are top 3 blockers, each with owner and date?
- Platform readiness:
  - Subscription model and quota request status?
  - Environments needed for wave 1 (dev/test/uat/prod)?
