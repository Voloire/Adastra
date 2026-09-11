# Working agreements

## Language and attribution

- Communicate with Franco Geraci in Italian.
- Use standard US English for repository content, commit messages, pull requests, issues, reports, and other external deliverables.
- Use only the user's existing Git identity. Before every commit, verify effective author and committer against the configured identity.
- Never change Git name, email, signing identity, or authorship metadata. Stop if identity is missing or inconsistent.
- Never add AI attribution, provenance statements, or additional coauthor trailers.
- Never publish the user's personal email. The verified Git identity must use the user's GitHub noreply address; stop rather than replacing identity settings if it does not.

## Delivery

- Treat README.md as the current primary documentation entry point. Keep the detailed plan, decisions, and journal consistent with it. After Atlassian setup, use Confluence for explanatory pages and Jira for work items, retaining revision links.

- Work on `dev`.
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
- Use Luna/Terra for collection, Astra/Sol for decisions and review, and Luna with high reasoning effort for coding.
- Report agent count, model tiers, and order-of-magnitude cost when delegating.
- Keep delegated reports within 300 words and final summaries within 800 words unless requested otherwise.
