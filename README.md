# Migration-Acceleration

Migration Acceleration Programme delivers reusable, AI-powered tools and frameworks that help Solution Engineers, CSU teams, and NHS delivery partners remove persistent blockers in cloud migrations.

## Positioning (Important)

This toolkit is not a replacement for CSA, Factory, or delivery services.
It is a pre-sales acceleration layer that improves information quality and handoff readiness.

Primary intent:
- Qualify opportunities with enough confidence to move from Uncommitted to Committed in MCEM
- Capture only the data required for commit decisions and quality handoff
- Identify risks and unknowns early with clear owner/date accountability
- Bring in the right experts (CSA, Factory, security, networking) at the right time
- Reduce rework caused by incomplete pre-sales discovery

## What This Repository Now Contains

This repo has an execution-ready starter kit for a merged IC63 workflow:
- Module A: Readiness Assessment Agent
- Module B: Factory Intake Generator
- Unified cycle: Prototype -> Feedback -> Review -> Improve -> Repeat

## Start Here - Understand The Flow First

Before opening any template or guide, read this one page to understand what you are doing and why:
- `docs/01-how-migration-acceleration-works.md`

It explains the 6-stage flow in plain English and tells you which file to use at each stage.

## New SE Start Here (10 Minutes)

If this is your first time using this toolkit, do only this:

0. Read what this framework actually does:
- `docs/01-how-migration-acceleration-works.md`
1. Open the SE runbook:
- `docs/02-se-instructions.md`
2. Capture only commit-critical discovery inputs from the customer
3. Fill account discovery and two output templates:
- `accounts/00-account-template/01-discovery-answers.md`
- `templates/01-loop-readiness-output-template.md`
- `templates/02-factory-nomination-pack-template.md`
4. Share outputs with CSU/Factory and log 1-minute feedback:
- `templates/03-feedback-form-template.md`

If you are short on time, use the "Minimal Data Contract" section in the SE guide.

## Which File Should I Use?

| I need to... | File |
|---|---|
| Understand the flow | `docs/01-how-migration-acceleration-works.md` |
| Run a customer discovery call | `docs/02-se-instructions.md` |
| Know when to bring in specialists | `docs/03-raci-and-escalation-matrix.md` |
| Track pilot accounts | `docs/04-pilot-kickoff-and-tracker.md` |
| Read the detailed spec (leads/IC63) | `docs/05-merged-prototype-spec.md` |
| Capture commit-focused discovery answers | `accounts/00-account-template/01-discovery-answers.md` |
| Fill readiness output | `templates/01-loop-readiness-output-template.md` |
| Fill nomination pack | `templates/02-factory-nomination-pack-template.md` |
| Log quick feedback | `templates/03-feedback-form-template.md` |
| Run AI readiness prompt | `prompts/01-readiness-assessment-agent.prompt.md` |
| Run AI intake generator prompt | `prompts/02-factory-intake-generator.prompt.md` |
| Track delivery backlog | `backlog/devops-backlog.md` |

## Suggested Operating Cadence

- Weekly: run prototype on active NHS accounts
- Bi-weekly: review friction patterns and CSU/Factory rework causes
- Every 3-4 weeks: release updated prompts/templates

## Account Folder Starter

Use this copy-ready folder for each new customer account:
- `accounts/00-account-template/`

It contains all engagement files in order (`01` to `05`) so SEs can run the same workflow every time.

## Recommended First Pilot

- Pilot with 3 active accounts
- Run commit-focused discovery plus "Do Both" mode for each account
- Measure:
	- conversion from Uncommitted to Committed
	- time to nomination pack
	- nomination rework requested by CSU/Factory
	- repeated blocker categories

## Next Build Options

When you are ready, this repo can be extended with:
- A lightweight CLI/script to convert discovery markdown into YAML + nomination pack draft
- A Power App input form backed by Dataverse
- A Copilot Studio custom agent for guided interviews and file ingestion
