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

## Verified starting state

- Let's Check was cloned over SSH and its working tree was clean when checked.
- Python 3.13, Git 2.55, Node 24, and Codex CLI 0.153.4 are available.
- SSH and GitHub CLI work in the user's environment. Initial sandbox failures did not establish invalid user credentials.
- Docker and uv were not found on PATH and are not required for the initial approach.
- No laboratory dependencies or Atlassian accounts have been provisioned.

## Pending evidence

- Maintain a discovery travel log and tag every completed milestone. First milestone: project charter and planning baseline.
- Proposed brownfield procedure name: `brownfield-discovery`. It is not implemented or installed yet. Design its instructions in portable SKILL.md format, with runtime-specific adapters documented separately; validate separately on each runtime before claiming compatibility.

- Case stack, startup procedure, test coverage, and safe execution requirements.
- A representative evolution requirement and evaluation reference.
- Which case content is authorized for model execution and public reports.
- Actual telemetry, model availability, and comparative batch budget.

## Superseded

- Private repository: replaced by the explicit public-repository request.
- Synthetic purchasing application: replaced by Let's Check.
- Git-only truth and mandatory diff-only review: replaced by the complete handoff contract.
