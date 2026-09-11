# Discovery travel log

## Step 009 — Free environment and reciprocal navigation

Tag: `step-009-atlassian-free-environment`

Verified the dedicated Adastra environment through Brave on 2026-09-11. Initial inspection found Jira and Confluence on Premium 30-day trials, not Free. The owner completed both downgrades; subscription detail pages and the billing subscription list subsequently showed Free for both products, with one user each. The payment-methods page explicitly reported that the billing account had no payment methods. No credentials or payment details were entered, and no paid subscription was purchased.

Connected the Adastra Confluence space to Jira's Docs view and added the `Adastra documentation` shortcut to the [Jira board](https://voloirex.atlassian.net/jira/software/projects/ADA/boards/1). Added the reciprocal `Adastra Kanban board` shortcut to the [Confluence documentation home](https://voloirex.atlassian.net/wiki/spaces/ADA/overview). Read-back confirmed both shortcuts and the connected space. Confluence records the environment evidence and the owner-approved operating model: Jira and Confluence exclusively manage daily work; README documents the project, while Git preserves versioned deliverables, consolidated decisions, and immutable milestones. Only approved public planning content and navigation links were published.

Verification limits: the billing console continued to display a payment-details warning even though both product plans showed Free and the account had no payment methods. The cause is unconfirmed; the displayed plan state does not establish future billing behavior. No Atlassian plugin or connector was invoked in this session, and the earlier connector tests are not a post-downgrade validation. Official [Atlassian MCP documentation](https://www.atlassian.com/platform/rovo-mcp) states that Cloud Free customers have access with a site limit of 500 calls per hour. [Rovo credit documentation](https://support.atlassian.com/rovo/docs/rovo-usage-limits/) distinguishes free single-product reads and writes from enriched, credit-consuming context calls. This is documentary eligibility evidence, not a successful connection test on this machine.

[Confluence page 196947, version 6](https://voloirex.atlassian.net/wiki/spaces/ADA/history/196947/Adastra) records the environment evidence and operating model. [ADA-1](https://voloirex.atlassian.net/browse/ADA-1) retains the operational completion record and published Git revision. Subsequent sequencing and procedure approval belong in Atlassian; no brownfield experiment was run in this milestone.

## Step 008 — Atlassian connector validation

Tag: `step-008-atlassian-connector`

Validated the supported connector against the dedicated `voloirex` Atlassian site in a fresh conversation. Current-user identity and accessible resources resolved successfully. Cross-product Rovo search returned the Adastra space, page, and Jira work item; direct reads of Confluence page `196947` and Jira issue ADA-2 succeeded; validated JQL returned the ADA project work items; and Atlassian Projects search completed successfully. A narrowly scoped Jira comment recorded the recovery evidence and proved write access, after which ADA-2 was transitioned to Done and read back in that state.

The earlier generic `INVALID_ARGUMENT` failure is no longer reproducible. No reconnect, API token, scope expansion, or credential handling was required, but the root cause remains unconfirmed; this milestone records observed recovery rather than attributing an unverified fix. The connector's declared access includes Jira, Confluence, Projects, Goals, and Loom, but this milestone does not claim exhaustive write coverage. No Atlassian Projects were present in the search result.

Confluence is now the primary operational documentation home and Jira the source for task state. Git retains consolidated, owner-reviewed baselines and immutable milestone history without duplicating live operational records. Complete the Free-plan and reciprocal-link evidence in ADA-1, then obtain owner review of the portable brownfield procedure in ADA-3 before executing the first experiment.

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
