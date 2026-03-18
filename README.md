# Migration-Acceleration

Migration Acceleration Programme delivers reusable, AI-powered tools and frameworks that help Solution Engineers, CSU teams, and NHS delivery partners remove persistent blockers in cloud migrations.

## Positioning (Important)

This toolkit is not a replacement for CSA, Factory, or delivery services.
It is a pre-sales acceleration layer that improves information quality and handoff readiness.

Primary intent:
- Capture the right customer information early
- Identify gaps quickly
- Bring in the right experts (CSA, Factory, security, networking) at the right time
- Reduce rework caused by incomplete pre-sales discovery

## What This Repository Now Contains

This repo has an execution-ready starter kit for a merged IC63 workflow:
- Module A: Readiness Assessment Agent
- Module B: Factory Intake Generator
- Unified cycle: Prototype -> Feedback -> Review -> Improve -> Repeat

## New SE Start Here (10 Minutes)

If this is your first time using this toolkit, do only this:

0. Read what this framework actually does:
- docs/how-migration-acceleration-works.md
1. Open the beginner guide: `docs/se-instructions-5-minute.md`
2. Ask the customer only the 10 core questions in that guide
3. Fill two templates:
- `templates/loop-readiness-output-template.md`
- `templates/factory-nomination-pack-template.md`
4. Share outputs with CSU/Factory and log 1-minute feedback:
- `templates/feedback-form-template.md`

If you are short on time, use the "Minimal Data Contract" section in the SE guide.

## Which File Should I Use?

- I am new and need a script: `docs/se-instructions-5-minute.md`
- I need to understand what this does: `docs/how-migration-acceleration-works.md`
- I need RACI and when to call in specialists: `docs/raci-and-escalation-matrix.md`
- I need to track the pilot accounts: `docs/pilot-kickoff-and-tracker.md`
- I need strategy/detail for leads: `docs/merged-prototype-spec.md`
- I need to fill readiness output: `templates/loop-readiness-output-template.md`
- I need to fill nomination pack: `templates/factory-nomination-pack-template.md`
- I need to log quick feedback: `templates/feedback-form-template.md`

## Start Here

1. Read the merged implementation spec:
- `docs/merged-prototype-spec.md`
2. Use SE quick-start instructions:
- `docs/se-instructions-5-minute.md`
3. Run prompts in Copilot workflow:
- `prompts/readiness-assessment-agent.prompt.md`
- `prompts/factory-intake-generator.prompt.md`
4. Produce Loop outputs:
- `templates/loop-readiness-output-template.md`
- `templates/factory-nomination-pack-template.md`
5. Capture iteration feedback:
- `templates/feedback-form-template.md`
6. Track delivery work:
- `backlog/devops-backlog.md`

## Suggested Operating Cadence

- Weekly: run prototype on active NHS accounts
- Bi-weekly: review friction patterns and CSU/Factory rework causes
- Every 3-4 weeks: release updated prompts/templates

## Recommended First Pilot

- Pilot with 3 active accounts
- Run "Do Both" mode for each account
- Measure:
	- time to nomination pack
	- nomination rework requested by CSU/Factory
	- repeated blocker categories

## Next Build Options

When you are ready, this repo can be extended with:
- A lightweight CLI/script to convert discovery markdown into YAML + nomination pack draft
- A Power App input form backed by Dataverse
- A Copilot Studio custom agent for guided interviews and file ingestion
