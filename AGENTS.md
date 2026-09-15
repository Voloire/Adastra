# Working agreements

## Language and attribution

- Communicate with Franco Geraci in Italian.
- Use standard US English for repository content, commit messages, pull requests, issues, reports, and other external deliverables.
- Use only the user's existing Git identity. Before every commit, verify effective author and committer against the configured identity.
- Never change Git name, email, signing identity, or authorship metadata. Stop if identity is missing or inconsistent.
- Never add AI authorship credits, generated-by statements, or additional coauthor trailers. The owner's explicit request for experimental model/run decision provenance permits factual measurement records only, not changes to Git attribution. Keep private evidence out of public records.
- Never publish the user's personal email. The verified Git identity must use the user's GitHub noreply address; stop rather than replacing identity settings if it does not.

## Delivery

- Use Atlassian exclusively for day-to-day work management: Jira for backlog and status, Confluence for operational plans, procedures, and explanatory pages. README.md documents the project and links to Atlassian; do not duplicate operational tracking in Git. Keep versioned deliverables, consolidated decisions, and immutable milestone history consistent, retaining revision links.
- Use concise Mermaid diagrams when they clarify workflows, approval gates, or source relationships. Keep diagram labels in US English and consistent with the written process.

- Work on `dev`.
- Keep `main` for reviewed, reproducible milestones and `dev` for ongoing exploration. Session-end pushes do not automatically promote work to `main`.
- Promote `dev` through a pull request after owner review, preserving commits with a merge commit rather than squash. After promotion, fast-forward `dev` to include the merge commit before continuing; never rewrite published history.
- Use short-lived `spike/<topic>` or `feat/<topic>` branches from `dev` only when isolation is useful; return useful results to `dev`. Record negative findings even when experimental code is not retained. Do not create permanent branches per phase, person, or model.
- Use immutable annotated `step-NNN-short-name` tags for completed journal milestones and `vX.Y.Z` tags on `main` for consolidated package versions. A session does not require a version bump. Branches in this public repository are not privacy boundaries.
- Record each completed discovery milestone in `docs/TRAVEL_LOG.md` and publish an immutable annotated `step-NNN-short-name` tag with its commit. Do not tag unfinished work as complete.
- Plan new implementation work first; execute when requested.
- End sessions by verifying, committing, and pushing relevant authorized changes. Do not create empty commits.
- Report failed pushes explicitly; do not claim local work is published.
- Preserve user changes. No destructive Git operations or force pushes without an explicit request.
- Keep secrets, company transcripts, real operational data, and the brownfield source out of this public repository unless specifically authorized for publication.
- `letscheck/` is a separate ignored checkout. Do not stage it, change its remote, or publish its contents.

## Measurement and delegation

- Separate measured usage, estimated cost, and unavailable data.
- Before delegation, perform 2-3 direct reads, define at most three initial questions with nonoverlapping scopes, and state the budget.
- Use Sol with medium reasoning only for genuinely complex reasoning, planning, coordination or review; do not spend Sol on routine tasks. These rules apply to both laboratory experiments and actual project work.
- Use Luna 5.6 with high reasoning effort for development, feature implementation and other bounded execution; delegate to Luna whenever useful.
- Luna with high reasoning is the default execution model and performs the heavy lifting whenever delegation is safe: routine work, coding, tests, substantial file changes and operational verification. Sol handles only the complex part and does not duplicate Luna's implementation.
- Sub-agents are capped at Luna. Do not dispatch Sol, Astra or another higher-tier sub-agent unless Franco explicitly overrides this agreement.
- Never assign multiple agents to the same task. Multiple delegated needs must be distinct and non-overlapping; keep execution sequential whenever scopes share files, state or decisions.
- Select models explicitly. Do not switch, escalate or silently substitute models when a selected model is unavailable; obtain Franco's explicit approval for any exception.
- Report agent count, model tiers, and order-of-magnitude cost when delegating.
- Keep delegated reports within 300 words and final summaries within 800 words unless requested otherwise.
