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

The immediate next step is a dedicated Jira and Confluence Cloud Free site, separate from company services, followed by connector authorization and the first brownfield experiment. Minimal local wiki, ticket, and Kanban simulations remain a fallback if account setup blocks progress.

[Atlassian Free plans](https://www.atlassian.com/software/free) provide the account entry point. No paid trial is needed for the initial experiment.

## Documentation home

This README is the current primary documentation entry point. The linked plan, decisions, and travel log preserve supporting detail and history. Once the dedicated Atlassian site is connected, publish explanatory documentation to Confluence and actionable work items to Jira, linking each milestone to its Git revision. Do not create competing, unversioned copies of the approved specification.

## Skills and evaluation roadmap

The following is a proposed selection, not a claim that these workflows have already run on the case.

| Phase | Skill or procedure | Assessment and current status |
| --- | --- | --- |
| 1: Brownfield | `brownfield-discovery` | Proposed project-specific skill; not implemented or installed. Reconstruct observed behavior with code evidence, record uncertainty, and separate current behavior from business intent. No dedicated existing brownfield skill has been selected in this environment. |
| 2: Requirements clarification | `brainstorming` from Superpowers | Existing skill available locally and inspected. Helps clarify intent and design with the PO; it is not a reverse-engineering or Jira publishing tool. |
| 2: Technical task planning | `writing-plans` from Superpowers | Existing skill available locally and inspected. Decomposes an approved specification into implementation tasks; it does not by itself provide a complete business backlog with epics, stories, and Jira synchronization. |
| 2: Business backlog decomposition | `backlog-decomposition` | Proposed project-specific procedure, not yet implemented. Build on clarified requirements and technical planning, adding story boundaries, acceptance criteria, dependencies, coverage checks, and publication mapping. |

Phase 2 starts after the brownfield baseline is reviewed by the application owner. Assess decomposition by requirement coverage, independently testable stories, missing dependencies, invented scope, and human correction time. A longer backlog is not inherently a better backlog.

### Claude Code compatibility

Superpowers documents support for Claude Code and Codex. Claude Code supports the Agent Skills `SKILL.md` format. This establishes a supported packaging route, not identical behavior across runtimes or a verified run of the locally installed skill revisions.

For the two proposed project skills, keep the core procedure in standard Markdown/frontmatter and isolate tool names, connector operations, shell commands, and model routing in runtime adapters. Before calling a skill compatible, test discovery, invocation, tool permissions, output structure, and evidence quality in both environments using the same inputs. Record the skill revision, model, runtime, and result in the travel log.

Claude Code support does not automatically establish support in every Claude web or hosted cloud environment. Those environments have their own skill-loading and tool-access rules and require a separate check if selected.

References: [Superpowers](https://github.com/obra/superpowers), [Claude Code skills](https://code.claude.com/docs/en/skills).
