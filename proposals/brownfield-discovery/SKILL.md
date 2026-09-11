---
name: brownfield-discovery
description: Use when reconstructing an existing application's observed behavior from an approved code snapshot before comparing documentation or validating business intent with its owner.
---

# Brownfield discovery

Draft for owner review. This package is a versioned proposal, not an installed or behaviorally validated skill. Loading it does not authorize a case run.

## Contract and entry gate

Reconstruct what the approved snapshot supports. Keep observations, hypotheses, documented intent, owner-approved intent, and decisions distinct. A successful test supports its exercised path; it does not prove all behavior or business correctness.

Before analysis, require an approved scope, evaluation questions, input manifest, case revision, private feasibility baseline, runtime adapter, storage destinations, and execution profile. Read [the evidence contract](references/evidence-contract.md) and [the validation protocol](references/validation.md). The operational run plan and owner decisions belong in the designated work-management system; do not maintain a competing backlog here.

The first experiment permits one active execution, at most 20 minutes per phase, at most two correction cycles across the run, and no recursive delegation. Do not create workers by default. Changing these limits or widening the approved inputs requires a new decision. Timeouts produce partial evidence, never automatic acceptance.

## 1. Verify inputs and boundaries

Record the exact case, procedure, adapter, and approved-plan revisions. Check access and safe execution against the private feasibility baseline before running case commands. Do not install dependencies, call external services, use production data, or modify case files unless individually covered by that baseline.

Inventory all input channels, including instructions, conversation history, repository documentation, search indexes, tools, logs, caches, and inherited agent context. Keep the owner's reference dossier outside the reconstruction worker's accessible inputs. A separate checkout or an instruction to ignore a file does not establish isolation. If access isolation cannot be verified, label the run **non-blind**, disclose the exposure, and obtain owner acceptance of that evaluation limitation before reconstruction.

If approval, required inputs, safe execution, or enforceable timing is missing, stop with a bounded blocker report. Do not infer consent from silence.

## 2. Reconstruct from code

Use only the approved code, manifests, tests, and permitted generated observations. Consult repository instructions for safety; record any behavioral information they expose. Trace the selected entry point through validation, state changes, outputs, and failure paths. Record file/symbol references at the fixed revision. Distinguish static inspection, test inspection, and executed tests.

Create one evidence record per independently reviewable claim. Record missing coverage, alternatives, and uncertainty. Existing documentation is withheld during this phase; accidental exposure makes the affected run non-blind. Preserve useful negative findings without inventing explanations.

At phase end, freeze the reconstruction artifact with a content hash, timestamp, and input manifest in approved private storage. Subsequent findings must not silently alter this snapshot.

## 3. Compare existing documentation

Only after the reconstruction snapshot is frozen, open approved documentation in a separate comparison phase. Identify document revisions and map assertions to claim IDs. Classify agreements, contradictions, omissions, and unverifiable assertions. Preserve both sources. Documentation describes a claim about behavior or intent; it cannot retroactively become code evidence.

## 4. Validate with the owner

Present the frozen reconstruction, comparison, uncertainties, and evaluation results. The owner determines business intent and accepts, rejects, or requests changes to individual claims. Owner confirmation does not upgrade an unexecuted test to a passing test. Record decisions with approval references and preserve superseded evidence.

Corrections must identify affected claims and consume the shared correction budget. Keep the original reconstruction for comparison. Do not reopen scope or restart a timer to evade limits. Unresolved items remain unresolved when the budget is exhausted.

## Exit and publication

Produce the manifest, evidence records, frozen reconstruction, comparison, owner dispositions, and run summary. Report completeness and stopping reason, measured usage separately from estimated cost, and unavailable telemetry explicitly. Evaluate only the approved scope and reference questions; do not imply whole-application coverage.

Publish only a reviewed, sanitized summary to the approved audience. Keep private evidence and the reference dossier outside public repositories and public planning spaces. Link authorized records to immutable revisions, and verify publication before reporting delivery. Runtime-specific mechanics and model selection belong in [the adapter contract](adapters/runtime-contract.md).
