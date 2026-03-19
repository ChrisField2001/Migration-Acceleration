# IC63 Migration Acceleration - Merged Prototype Spec

## Audience
This document is for initiative owners, leads, and reviewers.
If you are an SE running a customer call, start here instead:
- `docs/02-se-instructions.md`

## 1) Purpose
This prototype combines two initiatives into one repeatable operating flow:
- Module A: Readiness Assessment Agent
- Module B: Factory Intake Generator

Positioning principles:
- This is a pre-sales acceleration framework.
- This does not replace CSA, Factory, or delivery services.
- This improves information quality, identifies gaps early, and routes work to the right specialist teams.

Primary outcomes:
- Improve confidence to move opportunities from Uncommitted to Committed
- Reduce recurring migration blockers
- Improve nomination quality to CSU/Factory
- Increase reuse across NHS accounts
- Enable consistent execution by 10-15 SEs

## 2) Scope and Non-Goals
In scope (v1):
- Structured readiness interview
- Blocker and ownership capture
- Commit confidence recommendation and status
- Discovery-to-intake transformation
- Standardized output templates for Loop and handoff

Out of scope (v1):
- Full delivery planning automation
- Low-level design generation
- Automated environment provisioning

## 3) End-to-End User Journey
1. SE opens single entry point (agent/app/form).
2. SE selects one option:
- Run Readiness Assessment
- Generate Factory Intake from Discovery
- Do Both (recommended)
3. System collects inputs and generates standardized outputs.
4. SE shares outputs with CSU/Factory/partner.
5. SE submits quick feedback (1 minute).
6. Team reviews recurring friction and updates prompts/templates.

## 4) Module A - Readiness Assessment Agent

### Inputs
- Customer/account name
- Migration objective and deadline
- Current environment constraints
- Known blockers and dependencies

### Question Domains
- Identity and access readiness
- Landing zone readiness
- Networking and connectivity (ER, DNS, firewall)
- Subscription and quota readiness
- Security baseline (Defender, policy, CA)
- Monitoring and operations readiness
- UAT/test readiness
- Ownership and RACI clarity
- Sequencing and critical dependencies

### Output
- Commit confidence summary with recommendation:
- Move to Committed, or
- Stay Uncommitted with closure plan
- Blocker list with owner and target date
- Dependency map (what must happen before nomination)
- Recommended next actions (top 5)
- Loop-ready summary

### Qualification Logic v1
- Use RAG and ownership quality as primary signal for commitment decision.
- Do not require implementation-level design to recommend commitment.
- Require owner/date accountability for critical blockers.
- Use a dated 2-week closure plan for any unresolved commit blockers.

## 5) Module B - Factory Intake Generator

### Inputs
- SE discovery notes (structured or unstructured)
- Optional architecture notes
- Optional assumptions and constraints

### Extraction Targets
- Business outcome and migration scope
- In-scope workloads and data dependencies
- Azure services expected in target state
- Landing zone and IaC assumptions
- Security/compliance requirements
- Delivery constraints and milestone dates
- Open decisions and unknowns

### Output (Factory Nomination Pack)
- Executive summary
- Technology scope
- Delivery assumptions
- Azure product usage
- LZ/IaC needs
- Risks and blockers
- Open questions and decision log
- Evidence appendix (source notes snippets)

## 6) Shared Data Model (YAML)
Use this shared schema in both modules to increase reuse:

```yaml
engagement:
  account_name: ""
  region: ""
  migration_wave: ""
  owner_se: ""
  date: "YYYY-MM-DD"

readiness:
  score: 0
  status: "Not Ready | Needs Pre-Work | Ready to Nominate"
  blockers: []
  dependencies: []

factory_intake:
  scope: []
  azure_services: []
  assumptions: []
  lz_iac_needs: []
  open_questions: []
```

## 7) Pilot Cadence (First 7 Weeks)
- Weeks 1-3: Prototype v1 build and first usage
- Weeks 2-4: Structured feedback capture
- Weeks 4-5: Review against success measures
- Weeks 5-7: Improve high-value items and release v2
- Then: Repeat every 3-4 weeks

## 8) Success Metrics
- Time to first nomination pack (target: reduce by 30%)
- Rework requests from CSU/Factory (target: reduce by 25%)
- Reused assets per account (target: increase every cycle)
- Readiness blocker visibility before nomination (target: increase)
- SE satisfaction score (target: 4/5+)

## 9) Tooling Options
- Copilot for M365: guided Q&A, summaries, Loop generation
- Copilot Studio: custom IC63 migration agent with file ingestion
- GitHub Copilot in VS Code: prompt workflows and transformations
- Power Platform: forms, orchestration, tracking backend

## 10) Definition of Done for v1
- Both modules usable by at least 3 SEs on live accounts
- Outputs accepted by CSU/Factory for at least 2 pilot nominations
- Feedback loop in place and actively used
- v2 backlog approved and prioritized
