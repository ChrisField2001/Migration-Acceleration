# Loop Template - Readiness Assessment Output

## How To Use This Template (2 Minutes)
Fill required fields first, then optional fields if known.

Required now:
- Engagement: Account, Date, SE Owner
- Readiness Score: Score and Status
- Top Blockers: at least 3 with owner and due date
- Dependency Sequence: at least 3 steps

Optional for later refinement:
- Full Domain Ratings notes
- Additional actions beyond top 5

## Engagement
- Account: TBD (customer name not captured in initial answers)
- Date: 2026-03-18
- SE Owner: TBD
- Migration Objective: De-risk end of support for existing hardware by Dec 2026
- Target Nomination Date: TBD

## Readiness Score
- Score (0-100): 45
- Status: Not Ready

## Domain Ratings
| Domain | Score (0/1/2) | Notes |
|---|---:|---|
| Identity and access | 1 | Being designed |
| Landing zone | 1 | Being designed |
| Networking and connectivity | 1 | Dependency identified; not approved |
| Subscription and quota | 0 | Not ready/unknown |
| Security baseline | 1 | Potential Defender for Cloud + Sentinel; not committed |
| Monitoring and operations | 1 | Not yet detailed |
| UAT and testing | 1 | Test servers planned |
| Ownership and RACI | 1 | PM identified; blocker-level owners/dates missing |
| Sequencing dependencies | 1 | LZ -> network -> security identified at high level |

## Top Blockers
| Blocker | Owner | Due Date | Impact | Status |
|---|---|---|---|---|
| Landing zone design approval pending | Project Manager (named) + Platform Architect (TBD) | TBD | Migration planning cannot baseline target platform | Open |
| Networking and security design not approved | Project Manager (named) + Network Lead (TBD) | TBD | Workloads cannot connect or pass security gate | Open |
| Subscriptions/quotas/environments not confirmed | Project Manager (named) + Cloud Ops Owner (TBD) | TBD | Test wave cannot be deployed predictably | Open |

## Dependency Sequence
1. Finalize and approve landing zone design baseline.
2. Approve networking/security architecture (DNS, connectivity, policy).
3. Confirm subscriptions, quotas, and environment setup for wave-1 testing.

## Recommended Next Actions (Top 5)
1. Run a 60-minute technical checkpoint to name blocker owners and due dates.
2. Produce wave-1 scope list (workload names) plus explicit out-of-scope list.
3. Raise quota/subscription requests and confirm environment plan.
4. Define readiness exit criteria for moving from test servers to nomination.
5. Confirm whether Defender for Cloud + Sentinel are in wave-1 or phase-2.

## Customer Decisions Required
1. Which workloads are in wave-1 by name, and which are deferred?
2. Who is the accountable owner for each of the top 3 blockers?
3. Are security uplift items in wave-1 scope or post-migration scope?

## Share Log
- Shared with (CSU/Factory/Partner): Pending
- Date shared: Pending
- Requested follow-up: Technical dependency and ownership workshop
