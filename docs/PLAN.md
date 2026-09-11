# Work plan

## 1. Objective and scope

Measure brownfield analysis, PO clarification, specification, backlog decomposition, implementation, review, and knowledge updates using Let's Check.

Adastra contains the laboratory and publishable results. Case source, company transcripts, credentials, and sensitive results stay excluded. Do not automatically publish the case as a submodule. Laboratory implementation has not started.

## 2. Reconnaissance and evaluation reference

The dedicated Atlassian site and connector are operational. Complete the remaining Free-plan and reciprocal-link evidence in ADA-1, then define and obtain owner review of the portable discovery procedure in ADA-3. Only then may the first substantive experiment perform code-based brownfield reconstruction of Let's Check. Use the owner's knowledge for validation after reconstruction, not as answer material supplied to the evaluated session. Local enterprise simulations remain a fallback rather than a prerequisite for this first experiment.

Read case instructions, manifests, entry points, documentation, and test configuration. Record the full baseline commit, cleanliness, dependencies, startup procedure, and executable checks. Do not assume the stack from the earlier synthetic application proposal.

Select a small meaningful scope and an evolution requirement. Produce a feasibility report before implementation. Separate initial code-based reconstruction from comparison with documentation and owner validation. Existing documentation is evidence, not an infallible reference.

Create a private evaluation dossier of confirmed behaviors, tests, and unresolved questions. Exclude it from evaluated sessions. Verify real access isolation: a separate checkout does not prevent reads elsewhere. If isolation is unavailable, label the experiment non-blind and limit conclusions accordingly.

## 3. Local setup

Use the installed Python with a project-local virtual environment. Install Flask, pytest, coverage, and HTTPX, pinning versions after compatibility checks. Use SQLite and simple HTML. No mandatory Docker, GPU, frontend framework, or paid SaaS subscription.

Keep case dependencies separate. Provide PowerShell startup, shutdown, verification, and demo-reset scripts. Bind local services to loopback. Reset only validated laboratory data paths.

Build a minimal local portal:
- Versioned wiki pages for context, brownfield results, requirements, specifications, and decisions.
- Tickets containing acceptance criteria, dependencies, and links to handoffs.
- A Kanban view of ticket state: Backlog, Needs Clarification, Ready, In Progress, In Review, Done.
- An experiment dashboard with evidence and comparisons.

The board must not duplicate ticket state. A Python coordinator exposes page, ticket, transition, handoff, and event operations. Store state in SQLite and append-only events in JSONL. Do not duplicate full Atlassian APIs.

## 4. Multi-agent workflow

1. Sol analyzes the case in a fresh session and produces components, observed rules, evidence, and questions.
2. Franco acts as PO. Record clarification answers and freeze them for comparable experiments.
3. Sol proposes an approved specification, impact analysis, and testable stories. Keep the descriptive existing-system backlog separate from future work.
4. Luna High implements one story at a time in an isolated checkout.
5. Automated checks precede an independent Sol review. Introduce Astra only in a later controlled comparison.
6. Human approval precedes integration. Propose knowledge updates referencing the integrated version.

A handoff contains approved requirement/specification revisions, base and candidate commits, diff, authorized scope, test environment and results, dependencies, and open questions.

Review starts from the change and can retrieve additional context with a recorded reason. Outcomes: acceptable, changes required, or insufficient information. Authors cannot approve their own changes or unilaterally weaken gates. New candidate code invalidates evidence that no longer applies.

Local proposal records initially simulate a PR packet; they are not hosted PRs. Git identifies code, tickets track work, tests provide evidence, and acceptance rules govern transitions.

## 5. Instrumentation and budget

Execution policy: Luna 5.6 High for development, Terra for web research, and Astra or Sol for planning and complex reasoning. Do not launch additional workers by default or duplicate concurrent assignments. Obtain explicit approval with plan, rationale, and budget before any escalation to a more capable model, including spikes. This policy also governs implementation of the laboratory itself.

Use separate CLI sessions per role and capture structured events. Run one calibration before batches to verify authentication, actual access to requested models, structured outputs, and usage fields. Visible user tasks are not a substitute for subagents without a specific request.

Record model/settings, input/output versions, duration, observable sources, tool calls, retries, delegations, tests, findings, and human minutes. Observed reads do not represent the full internal context.

Separate measured tokens, billed cost, and estimates. Missing data stays unavailable. Subscription consumption does not automatically imply a per-run API price. Include handoff preparation, corrections, and knowledge maintenance.

Defaults: one active execution, 20 minutes per phase, at most two correction cycles, and no recursive delegation in the first experiment. Enforce time limits in the coordinator. Do not claim hard token limits if usage arrives only after completion.

Present a total comparative-batch budget after calibration and before the batch starts. No automatic credit purchases or paid upgrades.

## 6. Comparative experiments

First complete one functional end-to-end walkthrough. Then prepare six frozen candidate changes: three correct and three with known defects in experimental copies. Run each twice under each method, for 24 reviews.

A: documented ordinary review. B: structured handoff and progressive context retrieval. Keep model, candidates, tools, and resource limits equal; alternate ordering and isolate session memory. Both methods may inspect the repository.

Evaluate against the separate reference dossier. Measure:
- Brownfield accuracy, omissions, and unsupported claims.
- Requirement coverage, missing dependencies, unrequested scope, and testability.
- Regressions, defects found/missed, false positives, and decision correctness.
- Rework, elapsed time, human effort, and measured usage.
- Knowledge-update accuracy and stale information.

Exploratory success criteria: no known critical defect missed, no observed decline in important-defect detection, and at least 20% reduction in human effort or variable cost without increasing the other. Report per-case results and negative outcomes. This small sample does not establish general safety or enterprise-wide savings.

Only after a favorable review experiment compare model allocations across the full implementation/review/correction lifecycle.

## 7. Real enterprise tools

Use the operational dedicated personal Jira and Confluence Cloud site as the selected initial enterprise environment, separate from company accounts; local simulations are a fallback. Verify the actual subscription state in ADA-1 before describing it as Free. No paid trial is required for the planned experiment.

Identity, site discovery, Jira and Confluence reads, Rovo search, JQL search, and a narrowly scoped Jira write were verified through the supported connector on 2026-09-11. Use only demo or explicitly authorized content. Subscription limits and Atlassian permissions/audit/automation limits mean laboratory telemetry remains independent.

Use the supported connector for pages, work items, searches, and transitions. Add narrow custom REST adapters only if a later approved experiment identifies a connector gap; keep any credentials outside Git. Project accepted changes into ticket state with idempotent retries. Record synchronization failures and reconcile them without duplicating records or losing integration evidence.

For repository-backed work, transition Jira in step with GitHub evidence: verify the candidate, commit and push the relevant revision, link the commit or pull request, then apply the agreed Jira completion rule. Reconcile requirement or decision changes originating in Jira or Confluence back into the accepted Git baseline. A failed push or publication leaves the corresponding work visibly pending.

OpenProject Community is a viable wiki/board alternative but is not selected for the initial installation because it adds local infrastructure.

## 8. Verification and delivery

Maintain `docs/TRAVEL_LOG.md` as the immutable Git milestone history, not as a duplicate operational task register. Each completed milestone records purpose, inputs, method/skill version, findings, evidence, limitations, and next step, and receives an immutable annotated `step-NNN-short-name` Git tag. Publish the tag together with its commit. Use Confluence for current explanatory documentation and Jira for actionable work and status.

Before brownfield execution, define the proposed `brownfield-discovery` procedure as a portable SKILL.md package. It is not currently implemented. Keep provider-specific tool names out of core instructions. Document installation and runtime adapters separately. Claude Code supports SKILL.md-based skills, but successful execution and comparable results require separate validation. See https://code.claude.com/docs/en/agent-sdk/skills.

Test demo restoration, session separation, dossier isolation, failed gates, stale approvals, duplicate ticket claims, retries, synchronization failures, and unavailable models.

Deliver setup instructions, local simulations, protocol, instrumentation, brownfield feasibility findings, comparison results, and the real Atlassian walkthrough once the account exists. Do not modify case functionality before reconnaissance and approved requirement definition.

## 9. Knowledge reconciliation and consultation roadmap

The README defines the accepted planning direction for evidence records, knowledge maintenance, reconciliation, and a read-only Slack interface. Define record fields before discovery. After implementation, compare frozen PO requirements with candidate evidence, resolve discrepancies with the owner and technical reviewer, and commit the accepted report before owner-approved Confluence publication. Wiki synthesis is downstream and optional.

Evaluate source-backed onboarding answers and seeded stale/contradictory records. Measure retrieval correctness, unsupported statements, stale-data detection, false positives, and human maintenance effort. Slack project-state answers must consult authorized operational sources and identify freshness rather than rely solely on wiki snapshots. Validate access, organizational consent, and existing service configuration before integration; do not collect secrets during planning.

Keep sensitive integration details in ignored local notes. Complete a public-content review before each push. Private backup, implementation design, and integration authorization remain separate pending steps.

## References

- [Atlassian Free plans](https://www.atlassian.com/software/free)
- [Atlassian licensing and trials](https://www.atlassian.com/licensing/cloud)
- [OpenProject wiki](https://www.openproject.org/docs/user-guide/wiki/)
- [OpenProject requirements](https://www.openproject.org/docs/installation-and-operations/system-requirements/)
- [Non-interactive execution](https://developers.openai.com/codex/noninteractive/)
- [Flask installation](https://flask.palletsprojects.com/en/stable/installation/)

Recheck service limits, pricing, and access when activating integrations.
