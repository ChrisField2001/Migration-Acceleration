# RACI and Escalation Matrix

## Purpose
Clarify who does what at each stage of pre-sales migration acceleration.
Use the escalation matrix to know exactly when and how to bring in specialist teams.

## Roles

| Role | Who They Are |
|---|---|
| SE | Solution Engineer running the customer engagement |
| Customer PM | Customer-side project or programme manager |
| CSA | Cloud Solution Architect |
| Factory | Microsoft delivery factory team |
| Security Specialist | Microsoft or partner security SME |
| Network Specialist | Microsoft or partner networking SME |

RACI Key:
- R = Responsible (does the work)
- A = Accountable (owns the outcome)
- C = Consulted (provides input)
- I = Informed (kept updated)

## Stage RACI

| Stage | SE | Customer PM | CSA | Factory | Security | Network |
|---|---|---|---|---|---|---|
| Run 10-question discovery | R/A | C | I | I | I | I |
| Score readiness and classify status | R/A | I | C | I | I | I |
| Identify blockers and owners | R | A | C | I | C | C |
| Define dependency sequence | R | C | C | I | C | R/C |
| Trigger specialist engagement | R/A | I | C | I | C | C |
| Generate readiness output | R/A | I | C | I | I | I |
| Generate factory nomination pack | R/A | I | C | C | I | I |
| Review nomination pack | C | I | C | R/A | I | I |
| Close pre-work blockers | I | R/A | C | I | R | R |
| Submit feedback | R | I | I | I | I | I |

## Escalation Matrix

Use this table to decide when to bring in a specialist and how urgently.

### Bring in CSA when:

| Trigger | Urgency | Action |
|---|---|---|
| Scope or architecture is unclear after initial discovery | Within 2 business days | SE requests CSA architecture consultation |
| Modernisation path (refactor/replatform) is undecided | Before nomination | SE + CSA joint session with customer |
| Platform readiness is partial and needs technical design input | Within 3 business days | CSA reviews gaps and defines design pre-work |
| Customer is unsure which Azure services apply to their workloads | Before nomination | CSA leads a scoping session |

### Bring in Factory when:

| Trigger | Urgency | Action |
|---|---|---|
| Scope is stable and top blockers have named owners | Same day | SE submits nomination pack for Factory review |
| Delivery assumptions are clear enough for planning | Before nomination | SE shares pack and requests Factory intake review |
| Customer has approved wave-1 scope and timeline | Before nomination | SE formally nominates to Factory |

### Bring in Security Specialist when:

| Trigger | Urgency | Action |
|---|---|---|
| Identity controls (MFA, CA, PAM) are incomplete or in design | Within 2 business days | SE flags identity gap and requests security input |
| Compliance obligations are unclear (NHS DSPT, GDPR, ISO) | Before nomination | SE requests compliance review |
| Security baseline decisions are blocking pre-work | Within 1 business day | Security specialist joins blocker resolution |
| Defender for Cloud or Sentinel are candidates for this wave | Before nomination | Security specialist confirms scope and sizing |

### Bring in Network Specialist when:

| Trigger | Urgency | Action |
|---|---|---|
| DNS or routing ownership is unclear | Within 2 business days | Network specialist maps ownership and resolves gaps |
| Landing zone connectivity design is not approved | Before nomination | Network specialist supports design approval |
| External provider dependencies (third-party network, MPLS) exist | Immediately | SE captures lead times and escalates to unblock |
| IP overlap or firewall/proxy constraints affect migration path | Before nomination | Network specialist validates connectivity model |

## Escalation Contact Template
Use this when triggering specialist engagement:

```
To: [Specialist name or team]
Subject: [Account name] - Migration Acceleration Escalation - [Area]

Account: [Name]
SE: [Name]
Escalation type: [Architecture / Security / Network / Factory intake]
Summary of gap: [2-3 lines]
Blocker impact: [What this is blocking]
Requested action: [What you need from the specialist]
Needed by: [Date]
Attached: Readiness output / Nomination pack draft
```

## Notes on Usage
- Do not wait until a blocker is critical before escalating.
- Use the readiness score as the trigger, not gut feel.
- If score is under 50 across any single domain, escalate that domain specialist immediately.
- Record all specialist engagements in the pilot tracker.
