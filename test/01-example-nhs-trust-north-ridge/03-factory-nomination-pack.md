# 03 - Factory Nomination Pack

## Executive Summary
- Account: NHS Trust North Ridge
- Migration objective: De-risk end-of-support infrastructure and prepare a controlled Wave-1 migration path.
- Scope snapshot: 12 app/reporting servers and backup management capability in Wave-1.
- Target nomination date: 2026-04-03

## Technology Scope
| Area | In Scope | Out of Scope | Notes |
|---|---|---|---|
| Compute | 12 non-critical servers | EPR core compute estate | Wave-1 confidence build |
| Data | Reporting middleware dependencies | PACS archive migration | Dependency mapping still being finalized |
| Identity | Existing control set validation | Enterprise identity redesign | Redesign tracked as future wave |
| Networking | Landing zone connectivity and firewall flow | Full WAN redesign | Ownership needs closure |
| Security | Baseline hardening and risk control checks | Full SOC redesign | Defender uplift candidate |
| Monitoring | Basic migration health telemetry | Enterprise observability refresh | Beyond Wave-1 |

## Delivery Assumptions
1. Quota and subscription approvals complete by 2026-03-27.
2. DNS/firewall ownership finalized by 2026-03-28.
3. Buyer checkpoint on 2026-04-02 confirms stage movement.

## Azure Product Usage
| Product/Service | Current State | Target State | Confidence |
|---|---|---|---|
| Azure landing zone baseline | Partial | Approved pattern for Wave-1 | Medium |
| Microsoft Defender for Cloud | Not standard | Baseline recommendation set | Medium |
| Azure Monitor | Limited | Wave-1 health dashboard | Medium |

## Landing Zone and IaC Needs
- Subscription model: Central billing with dedicated migration subscription.
- Policy baseline: Existing baseline with migration-specific exceptions tracked.
- Networking model: Hub-spoke with restricted ingress/egress policy.
- IaC preferred approach: Existing IaC pipeline with template extension only.
- Environments: Test and pre-prod for Wave-1.

## Risks, Blockers, and Mitigations
| Risk/Blocker | Impact | Owner | Mitigation | Status |
|---|---|---|---|---|
| Quota request delay | Slips checkpoint confidence | Helen Ward | Submit request pack and daily tracking | Open |
| DNS/firewall ownership ambiguity | Blocks sequence sign-off | Tom Reed | Assign governance owner in workshop | Open |
| Buyer financial concern | Stage movement delayed | Priya Shah | Align ROM and value narrative before checkpoint | Open |

## Open Questions and Decision Log
| Question | Decision Owner | Needed By | Status |
|---|---|---|---|
| Who signs off DNS cutover governance? | Mark Ellison | 2026-03-25 | Open |
| Is quota risk acceptable with contingency? | Digital Transformation Board | 2026-03-31 | Open |
| Is Wave-1 exclusion list approved? | Priya Shah | 2026-03-29 | Open |

## Evidence Appendix
- Discovery source: `01-discovery-answers.md`
- Notes: Presales qualification only. No low-level delivery design included.
