# Runtime adapter contract

Adapter requirements accepted as part of the ADA-3 design on 2026-09-11. This document does not establish installed compatibility, current product capabilities, or automated enforcement. Validate each selected runtime before using it with the case. The portable core must not depend on a particular CLI, connector, shell, or model name.

## Common adapter responsibilities

1. Record runtime/version and the actual loaded core, references, and skill hashes. Demonstrate invocation with a synthetic fixture before case access. Merely having a SKILL.md file is insufficient.
2. Translate the approved input manifest into real filesystem, tool, network, and session-context restrictions. Test excluded-data access with a harmless canary in a synthetic environment. Record the verification evidence; do not expose the real dossier to test a boundary.
3. Provide one active execution, an observable phase clock, a deadline, and reliable cancellation/checkpoint behavior. A prompt alone is not a hard timeout. If cancellation cannot be demonstrated, stop the timed experiment until a suitable supervisor is available.
4. Track two correction cycles across the entire run, with no recursive delegation or automatic retries after exhaustion. External tool latency counts toward the active phase. Human review waiting time is outside active execution and recorded separately.
5. Collect only available telemetry. Never infer hidden tokens, model identity, or cost from a subscription name. Respect existing identity, attribution, credentials, publication, and model-escalation policies.
6. Write artifacts only to approved private destinations. Separate reconstruction from document comparison and from the publishing session. Verify saved hashes, output structure, and publication receipts.

## Codex profile to validate

- Load the proposal explicitly in a fresh, scoped session using the runtime's supported skill mechanism after approval. Do not install from this proposal directory as a side effect of planning.
- Identify inherited instructions and conversation/tool context. The present planning session has prior project knowledge and must not be reused as a supposedly blind reconstruction session.
- Map allowed roots and execution permissions to the actual configured sandbox. Repository ignore rules and workspace selection alone do not prove read isolation.
- Demonstrate cancellation and output capture under the selected runtime; tool timeouts may not terminate a persistent child process. Record evidence that active work actually stops.
- Follow the project's model policy: Luna 5.6 High for development; Terra for web research; Astra or Sol for planning/complex reasoning. The selected analysis model and budget require the approved run profile. No silent substitution or escalation.

## Claude Code profile to validate

- Independently verify supported skill discovery and invocation in the exact installed runtime/version. Do not assume parity with Codex or with hosted Claude environments.
- Inspect inherited instruction files, permission settings, accessible roots, tools, and prior session context. Repeat canary isolation and cancellation checks; do not reuse Codex results as proof.
- Run the same approved synthetic fixture and compare required evidence fields and behavior against the same rubric. Record model metadata and unavailable measurements honestly.
- Use a separately approved model mapping and budget. No Claude run, installation, or model substitution is authorized by this draft.

## Atlassian publication profile

Atlassian is an output and work-management surface, not an input to the blind reconstruction worker. Publish from a separate authorized session after reviewing the audience and sanitizing evidence.

For this environment, use the existing authenticated Brave session. The owner has explicitly excluded the Atlassian plugin on this machine. Do not attempt connector access, collect API tokens, or create a custom REST integration for this task.

Jira owns scope, acceptance criteria, status, blockers, and approval references. Confluence owns the operational plan, skill catalog, evaluation protocol, and owner decisions. The public repository stores the portable proposal and later accepted versions; README provides navigation. Link Confluence revisions and Git commits explicitly. Do not copy the private dossier, case snippets, internal names, credentials, or raw execution logs to public planning records.

Before reporting publication, reopen the page/ticket and check its text, links, and resulting state. Record the published page revision or version-history link and exact Git revision in Jira. Failed publication remains pending. A browser fallback is a supported working choice, not evidence of connector incompatibility.
