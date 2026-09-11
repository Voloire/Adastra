# Adastra

A measurement-first laboratory for multi-agent software development.

## Project objectives

Adastra turns the idea of “Git as the contract” into an explicit, testable workflow. Git identifies the exact code being proposed and accepted. The complete contract also includes approved requirements, specification revisions, constraints, relevant context, test evidence, and acceptance authority.

The project will:
- Reconstruct the observed behavior of an existing application through brownfield analysis.
- Distinguish implemented behavior from intended business requirements.
- Turn a PO's business request into an approved specification and testable backlog.
- Implement changes through isolated roles and versioned handoffs.
- Review changes starting from the diff, retrieving additional context when necessary.
- Measure total cost, human effort, defects, false positives, and rework.
- Compare the proposed process against an ordinary review baseline.

The hypothesis is that structured handoffs and targeted context retrieval improve the cost-quality tradeoff. Savings and reliability are outcomes to measure, not promises.

## Current status

Planning is documented. Laboratory implementation and functional brownfield analysis have not started. Let's Check is the selected real case; its separate local checkout is excluded from this public repository.

- [Work plan](docs/PLAN.md)
- [Decision record](docs/DECISIONS.md)
- [Discovery travel log](docs/TRAVEL_LOG.md)
- [Working agreements](AGENTS.md)

## Workflow

The working branch is `dev`. Each work session ends with verification, a commit of relevant authorized changes, and a push. Local-only work is not a completed delivery. No empty commits are required.

## Enterprise tools

Start with minimal local wiki, ticket, and Kanban simulations, then validate the workflow with dedicated Jira and Confluence Cloud Free accounts, separate from company services.

[Atlassian Free plans](https://www.atlassian.com/software/free) provide the account entry point. No paid trial is needed for the initial experiment.
