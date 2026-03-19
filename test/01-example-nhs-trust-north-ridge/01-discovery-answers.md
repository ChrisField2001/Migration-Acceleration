# 01 - Discovery Answers (SE Qualification for MCEM Commit)

- Account Name: NHS Trust North Ridge
- Date: 2026-03-19
- SE Owner: Alex Morgan
- Customer PM / Sponsor: Priya Shah (PM), Mark Ellison (CIO Sponsor)
- Opportunity Stage (Uncommitted/Committed): Uncommitted
- Target Commit Date: 2026-04-02

## 1) Business and Decision Context
- Business outcome we are selling: De-risk end-of-support infrastructure and improve service continuity for clinical systems before Q4 budget checkpoint.
- Why now / deadline driver: Current estate has end-of-support risk by Dec 2026 and board requires migration plan confidence in April governance review.
- Decision criteria to move to committed: Named Wave-1 scope, approved risk owners/dates, and agreed 2-week closure plan for unknowns.
- Economic buyer and approval path: CIO as economic buyer, approval via Digital Transformation Board chaired by COO.

## 2) Wave-1 Scope (Presales Level)
- In-scope workloads/capabilities (high level): 12 non-critical app servers, backup management service, and reporting middleware.
- Out-of-scope for Wave-1: EPR core workloads, PACS archive platform, and enterprise identity redesign.
- Key assumptions for sizing and timeline: Existing application compatibility is moderate; no major refactor needed for Wave-1; network and policy approvals complete by end of March.
- Minimum customer inputs required to proceed: Confirmed workload list, named owners for top blockers, and board checkpoint date.

## 3) Readiness Snapshot (RAG + one line)
- Identity/security readiness (MFA/CA/PAM): Amber - baseline exists, privileged access model exceptions unresolved.
- Landing zone/network readiness: Amber - target landing zone pattern agreed, DNS and firewall ownership split not finalized.
- Subscription/quota/environment readiness: Red - subscription model agreed in principle, quota requests not submitted.
- Data/dependency readiness: Amber - key app dependencies listed, cutover sequence still draft.

## 4) Risks to Commit (Top 3)
- Risk 1 + impact + owner + target date: Quota request delay could push commit checkpoint by 1-2 weeks; Owner: Cloud Ops Lead (Helen Ward); Target date: 2026-03-27.
- Risk 2 + impact + owner + target date: DNS and firewall decision latency could block migration sequence sign-off; Owner: Network Manager (Tom Reed); Target date: 2026-03-28.
- Risk 3 + impact + owner + target date: Buyer approval may slip if financial profile is not clear; Owner: Customer PM (Priya Shah); Target date: 2026-03-31.

## 5) Value Expansion Signals (Tie to Business Outcome)
- Modernization opportunities relevant now: Move selected middleware service to managed PaaS in Wave-2 planning.
- Security uplift opportunities: Introduce Defender for Cloud recommendations for baseline hardening in parallel.
- AI opportunities feasible in 6-8 weeks: Pilot service desk triage summarization for migration incident handling.

## 6) Unknowns That Block Commitment
- Unknown: Final owner for cross-team DNS cutover decisions.
- Impact to commit milestone: Commit recommendation remains conditional until owner/date is confirmed.
- Owner: Customer PM (interim)
- Date to resolve: 2026-03-25

## 7) Uncommitted -> Committed Action Plan (Next 2 Weeks)
- Customer actions required: Confirm decision owners, finalize workload inventory, approve commit checkpoint agenda.
- Microsoft actions required: Produce ROM estimate, finalize risk log narrative, run dependency workshop.
- Required commit artifacts (scope note, ROM estimate, plan, risks): Scope note draft v1, ROM estimate draft v1, 2-week closure plan, risk register with owners.
- Commit checkpoint date: 2026-04-02
- Commit exit criteria met? Yes/No: No (pending ownership and quota evidence)
