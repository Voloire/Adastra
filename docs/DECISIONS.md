# Decision record

## Accepted

1. Project: Adastra. Public GitHub repository, working branch `dev`.
2. Remote Git stores the consolidated plan, decisions, and deliverables. Local files are a working copy; delivery requires a successful push.
3. Let's Check is the real brownfield case, replacing the proposed synthetic purchasing application. Keep its checkout separate and excluded from this public repository.
4. Reconstruct current behavior first, then define an evolution of that same application.
5. Code reveals implemented behavior, not necessarily original intent. Separate facts, hypotheses, defects, and PO decisions.
6. The diff is the review entry point, not an absolute context boundary.
7. The contract includes requirements, revisions, scope, diff, context, evidence, and acceptance rules. No single tool represents all operational truth.
8. Start with local wiki/ticket/Kanban simulations; later validate on dedicated personal Atlassian Free services.
9. Measure total cost, human effort, defect detection, false positives, and rework before claiming improvements.
10. Initial roles: Sol for analysis/review; Luna High for coding; Astra as a later comparison. Verify actual CLI access first.
11. Conversation is in Italian; all external deliverables use standard US English.
12. All Git attribution uses the user's configured identity, without additional coauthors or AI provenance.
13. Publish only the user's GitHub noreply email in Git metadata, never a personal email.
14. Next user-facing step: create dedicated Atlassian Free accounts and connect access. The first substantive experiment is code-based brownfield reconstruction of Let's Check, reviewed by its owner. Keep local simulations as a fallback if account setup blocks progress.

15. Evaluate durable knowledge as phase three, drawing on the LLM Wiki pattern. Define evidence fields before the brownfield run so later synthesis has traceable inputs.
16. Keep observations, inferred intent, PO-approved intent, and decisions distinct. Linting identifies structural faults and possible semantic problems; it does not establish truth.
17. Record factual model/run provenance for delegated choices as requested by the owner, without altering Git authorship or adding generation credits.
18. Publish approved, revision-linked views to Confluence and work-item links to Jira. Initially avoid automatic bidirectional synchronization.

19. Reconcile approved requirements with implementation evidence before proposing documentation updates. Preserve discrepancies and require explicit acceptance; wiki processing is not a prerequisite.
20. Plan read-only project consultation through Slack using authoritative operational sources, approved documents, audience restrictions, and source freshness. No connection is authorized merely by possessing a token.
21. The owner participates in manual review and publication approval. Living documentation requires maintained validation, not an automatic accuracy guarantee.
22. Retain generalized decisions publicly and sensitive operational notes locally outside Git. A private backup remains to be arranged; do not promise complete conversation archival.

23. Development uses Luna 5.6 High; web research uses Terra; planning and complex reasoning use Astra or Sol. Additional workers are not the default; no concurrent duplicate assignments. More-capable model escalation requires prior approval with plan, rationale, and budget.

24. Adopt two permanent branches: `dev` for current exploration and `main` for reviewed milestones. Promote through owner-reviewed pull requests with merge commits preserving history, not squash. Fast-forward `dev` after promotion. Optional short-lived `spike/<topic>` and `feat/<topic>` branches return results to `dev`; no permanent branches per phase, person, or model. Session-end pushes are not automatic promotions. Use annotated milestone tags for the journal and version tags on `main` for consolidated packages. Public branches do not isolate private data. This is an operational policy, not a claim of configured GitHub enforcement.

25. Enable lightweight GitHub protection on `main`, including administrators: require a pull request with zero mandatory approvals, block force pushes and deletion, and require no CI checks yet. Keep `dev` unprotected. No signature, code-owner, or linear-history requirement. This implements the protection layer that was not yet configured in decision 24; tag immutability remains procedural.

26. Use Confluence as the primary operational documentation home and Jira as the source for actionable work and current status. Keep README as a concise repository entry point, and keep the travel log for immutable milestone history rather than day-to-day activity. Git continues to version code, approved deliverables, consolidated decisions, and milestone evidence; material Atlassian decisions require owner-reviewed reconciliation when they change the accepted Git baseline. Jira and GitHub advance coherently: repository-backed work is complete only after verified Git evidence is successfully pushed and linked, while failed publication remains explicitly pending.

27. Use the supported Atlassian connector as the default integration path. Identity, resource discovery, Rovo search, Jira and Confluence reads, JQL search, and a narrowly scoped Jira write were verified on 2026-09-11. The previous connector failure is no longer reproducible, but its root cause is not established. Custom REST adapters require a later approved connector-gap finding.

## Verified starting state

- Let's Check was cloned over SSH and its working tree was clean when checked.
- Python 3.13, Git 2.55, Node 24, and Codex CLI 0.153.4 are available.
- SSH and GitHub CLI work in the user's environment. Initial sandbox failures did not establish invalid user credentials.
- Docker and uv were not found on PATH and are not required for the initial approach.
- No laboratory dependencies have been provisioned. The dedicated Atlassian site, Adastra Confluence space, Jira project, and connector are operational; Free-plan verification and reciprocal project links remain pending in ADA-1.

## Pending evidence

- Maintain a discovery travel log and tag every completed milestone. First milestone: project charter and planning baseline.
- Proposed brownfield procedure name: `brownfield-discovery`. It is not implemented or installed yet. Design its instructions in portable SKILL.md format, with runtime-specific adapters documented separately; validate separately on each runtime before claiming compatibility.

- Case stack, startup procedure, test coverage, and safe execution requirements.
- A representative evolution requirement and evaluation reference.
- Which case content is authorized for model execution and public reports.
- Actual telemetry, model availability, and comparative batch budget.
- Verified Free subscription state and reciprocal Jira-Confluence project links (ADA-1).

## Superseded

- Private repository: replaced by the explicit public-repository request.
- Synthetic purchasing application: replaced by Let's Check.
- Git-only truth and mandatory diff-only review: replaced by the complete handoff contract.
- Local enterprise simulations as the mandatory first environment: replaced by the operational dedicated Atlassian site; local simulations remain a fallback.
