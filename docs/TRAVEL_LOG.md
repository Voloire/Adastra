# Discovery travel log

## Step 007 — Lightweight main protection

Tag: `step-007-main-protection`

Applied the owner-approved GitHub branch protection to `main`: require pull requests with zero mandatory approvals, prevent force pushes and deletion, and enforce the policy for administrators too. No status checks, signatures, code-owner reviews, or linear history are required. Read-back verification confirmed the settings and that `dev` remains unprotected. No destructive push was used to test enforcement. Tag immutability remains an operational convention.

This configuration and documentation milestone does not merge `dev` into `main` or publish a new package version.

## Step 006 — Approved branching strategy

Tag: `step-006-branching-strategy`

The owner approved two permanent branches, optional short-lived experiment and feature branches, and owner-reviewed pull requests from `dev` to `main` with preserved commit history. The README now includes the workflow diagram; working agreements define session closure, promotion, and tag semantics. After a promotion, bring the merge commit back into `dev` by fast-forward before continuing.

This milestone records the approved workflow on `dev`; it does not promote a new package version to `main`. No GitHub protection settings, default-branch changes, application implementation, or brownfield analysis are included. Verification is limited to documentation consistency, Git whitespace checks, attribution, and publication alignment.

## Step 005 — First versioned planning baseline

Milestone tag: `step-005-planning-release`

Version tag: `v0.1.0`

The owner requested publication on `main` in addition to `dev`. Remote inspection found no existing `main` branch, so the first main baseline is created from the committed development history; no artificial merge commit is required. Keep `dev` for ongoing work and retain the existing default-branch setting.

This version contains the project charter, plan, decisions, and discovery journal only. No application release, brownfield execution, or integration is implied. Verification covers tracked-file scope, Git whitespace checks, configured attribution, and remote branch/tag alignment. Private notes and the separate brownfield checkout remain excluded.

## Step 004 — Session handoff and execution controls

Tag: `step-004-session-handoff`

Recorded the owner's model routing, sequential delegation constraints, and mandatory approval before model escalation. Added dedicated Atlassian Free signup instructions to the README. No additional workers were launched, accounts created, or integrations connected. Next session begins with the owner's experimental site and a review of the brownfield plan; sensitive local notes still require an authorized private backup.

## Step 003 — Knowledge provenance design

Tag: `step-003-knowledge-provenance`

Reviewed the original Karpathy LLM Wiki gist and added a phase-three design to the README. The gist is a conceptual pattern, not an installed skill. Adastra's proposed extension distinguishes evidence types, approval status, revision validity, structural checks, semantic review, and controlled publication.

The owner requested traceability of intent, decisions, affected code, and delegated model choices. Technical experiment provenance is separate from Git authorship. Brownfield conclusions cannot establish original intent without additional evidence or owner confirmation.

This milestone completes documentation only. No wiki, lint checks, Atlassian publication, or brownfield execution has been implemented. Next: establish the first experiment's evidence fields, permissions, and reference questions before collecting case findings; evaluate knowledge maintenance once earlier phases provide inputs.

Additional requirements captured in this milestone: owner-led manual review, reconciliation before documentation publication, read-only project-state consultation, and evidence-backed onboarding. Sensitive integration details are retained in an ignored local note rather than this public record. No credentials were collected. Private backup remains pending.

## Step 002 — Skill roadmap and documentation home

Tag: `step-002-skill-roadmap`

The README is now the primary documentation entry point. It distinguishes proposed `brownfield-discovery` and `backlog-decomposition` procedures from existing `brainstorming` and `writing-plans` skills. The existing local instructions and upstream Superpowers/Claude Code documentation were inspected; no case analysis or cross-runtime execution was performed.

Business backlog decomposition is phase two. Technical task planning alone does not establish complete story decomposition or Jira integration. Compatibility is split into packaging support and actual runtime validation. Future explanatory pages belong in Confluence; work items belong in Jira, with Git revision links.

Next: dedicated Atlassian account and connector access, then define and validate the brownfield procedure before the first case run.

## Step 001 — Project charter and planning baseline

Tag: `step-001-project-charter`

### Purpose

Translate the versioned-handoff idea into an explicit measurement plan and establish a durable project record.

### Inputs and method

Requirements clarified with the project owner, read-only environment checks, and official product documentation. No brownfield analysis skill has been executed yet.

### Decisions and findings

- Adastra is a public planning and laboratory repository using `dev`.
- Let's Check is the selected brownfield case; its separate checkout stays excluded.
- Git identifies changes; requirements, constraints, context, evidence, and acceptance authority complete the contract.
- Compare total effort and defect detection, not only reviewer token consumption.
- Start with minimal local enterprise simulations and validate later on dedicated Atlassian Free services.
- Use Italian for conversations and US English for external deliverables.

### Evidence and limits

SSH cloning succeeded and the case working tree was clean. Python, Git, Node, and the CLI are available. The work plan and decision record contain the current scope and sources. No laboratory dependency installation, model experiment, or functional case analysis has occurred. Model access and telemetry require calibration.

### Next milestone

Read case instructions and manifests, establish an executable baseline, and define the brownfield procedure and evaluation boundaries. Do not treat current code as proof of original business intent.
