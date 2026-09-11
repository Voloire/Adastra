# Discovery travel log

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
