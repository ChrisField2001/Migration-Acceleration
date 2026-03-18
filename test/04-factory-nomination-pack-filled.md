# Loop Template - Factory Nomination Pack

## How To Use This Template (3 Minutes)
Fill required fields first so CSU/Factory can act quickly.

Required now:
- Executive Summary: Account, Objective, Scope Snapshot, Date
- Technology Scope: in scope and out of scope
- Risks/Blockers: at least 3 with owner
- Open Questions: owner and needed-by date

Optional for later refinement:
- Detailed evidence appendix
- Expanded Azure product mapping

## Executive Summary
- Account: TBD (not captured in initial call)
- Migration Objective: De-risk end of support for existing on-prem/private cloud hardware by Dec 2026
- Scope Snapshot: Small set of servers for test migration wave focused on performance, stability, and supportability validation
- Target Nomination Date: TBD

## Technology Scope
| Area | In Scope | Out of Scope | Notes |
|---|---|---|---|
| Compute | Small number of test servers | Full estate cutover | Test wave only |
| Data | Minimal data needed for performance/supportability validation | Full data migration | Data dependency detail not captured yet |
| Identity | Identity design activities | Finalized identity controls | MFA/CA/PAM status is design-stage |
| Networking | Network design for migration path | Full production network transition | Depends on LZ/network approval |
| Security | Baseline security architecture discussion | Full security operating model rollout | Defender for Cloud + Sentinel possible |
| Monitoring | Initial supportability checks | Full observability platform rollout | To be defined in next checkpoint |

## Delivery Assumptions
1. Wave-1 is a controlled test migration, not full production migration.
2. Landing zone, networking, and security designs will be approved before nomination.
3. Subscription/quota readiness can be completed in pre-work period.

## Azure Product Usage
| Product/Service | Current State | Target State | Confidence |
|---|---|---|---|
| Azure Landing Zone capabilities | Not finalized | Baseline design approved for wave-1 | Low |
| Microsoft Defender for Cloud | Potential | Candidate for security uplift | Medium |
| Microsoft Sentinel | Potential | Candidate for security uplift | Medium |

## Landing Zone and IaC Needs
- Subscription model: TBD
- Policy baseline: TBD
- Networking model: TBD
- IaC preferred approach: TBD
- Environments (Dev/Test/UAT/Prod): Test first; broader environment plan TBD

## Risks, Blockers, and Mitigations
| Risk/Blocker | Impact | Owner | Mitigation | Status |
|---|---|---|---|---|
| Landing zone design not yet approved | Blocks architecture and migration sequencing | Project Manager + Platform Architect (TBD) | Run design approval checkpoint and baseline sign-off | Open |
| Networking/security path not approved | Blocks connectivity and policy validation | Project Manager + Network/Security Leads (TBD) | Agree DNS/connectivity/policy ownership and due dates | Open |
| Platform readiness (subscriptions/quotas/envs) not ready | Delays test wave execution | Project Manager + Cloud Ops Owner (TBD) | Submit quota/subscription requests and confirm environment plan | Open |

## Open Questions and Decision Log
| Question | Decision Owner | Needed By | Status |
|---|---|---|---|
| Which workloads are explicitly in wave-1 and out of scope? | Project Manager + Customer Technical Lead | 2026-03-25 | Open |
| Who owns each blocker and what are committed target dates? | Project Manager | 2026-03-25 | Open |
| Are Defender for Cloud and Sentinel included in wave-1 or later phase? | Security Lead | 2026-03-25 | Open |

## Evidence Appendix
- Discovery source 1: Initial SE discovery Q1-Q10 answers
- Discovery source 2: N/A
- Key extracted notes:
  - End-of-support hardware deadline in Dec 2026
  - Test-server wave planned to validate migration feasibility
  - Dependencies called out as landing zone, networking, security
  - Identity and network currently being designed
  - AI opportunities deferred at this stage
