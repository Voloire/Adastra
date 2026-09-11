# Evidence contract

Draft schema for review. These are required fields, not a claim that collection or validation is automated. Operational ownership and review state live in Atlassian; private run artifacts remain in the approved private evidence store.

## Run manifest

| Field | Required value |
| --- | --- |
| `run_id`, `parent_run_id` | Stable identifier; parent or explicit `none`. |
| `approval_ref` | Approved scope, questions, limits, audience, and decision revision. Missing approval blocks execution. |
| `case_revision` | Commit SHA plus cleanliness check; any approved uncommitted input requires a separately hashed snapshot. |
| `procedure_revision`, `adapter_revision` | Immutable revision and content hashes of actual loaded instructions. |
| `runtime`, `model`, `reasoning`, `skills` | Observed runtime/version and exposed model metadata; `unavailable` where not exposed. List actual loaded skill revisions, not the installed catalog. |
| `input_manifest` | Allowed roots, files/artifacts and hashes, tools/network scopes, safe commands, excluded inputs, and approved output locations. |
| `feasibility_ref` | Private baseline proving permitted access, setup constraints, test strategy, and safe execution. |
| `blindness` | `verified-blind` or `non-blind`, verification method, exposed information, and acceptance of limitations. Never infer isolation from ignored paths. |
| `phase_records` | Phase ID, start, deadline, finish, elapsed wall time, timer/cancellation mechanism, outcome, and active execution count. |
| `corrections` | Zero to two cycles total; initiating review, affected claim IDs, revision, and result. |
| `usage` | Measured input/output/cache tokens and source, or `unavailable`; elapsed and owner-active time separately. |
| `estimated_cost` | Currency, rate date/source, quantities, formula and estimate limits, or `unavailable`. Subscription cost is not inferred from token list prices. |
| `artifact_manifest` | Private artifact IDs, hashes, timestamps, source revisions, and sanitized publication mapping. |
| `outcome` | `complete`, `partial`, or `blocked`; reason, unresolved questions, and owner disposition. |

## Claim record

| Field | Required value |
| --- | --- |
| `claim_id`, `statement`, `scope` | Stable ID, one falsifiable assertion, inputs and path to which it applies. |
| `claim_type` | `observation`, `hypothesis`, `documented-intent`, `owner-approved-intent`, or `decision`. |
| `review_status` | `unreviewed`, `supported`, `partially-supported`, `not-supported`, `not-verifiable`, or `superseded`. Support is explicitly limited to cited evidence. |
| `case_revision` | Exact inspected commit/snapshot. |
| `file_or_symbol` | Revision-relative path and symbol or lines; `not-applicable` with reason for non-code claims. |
| `observation_method` | `static-code`, `test-inspection`, `test-execution`, `document-comparison`, or `owner-review`; include collection details. |
| `test_evidence` | Test ID/command, environment and input IDs, execution timestamp, outcome and evidence reference; otherwise `not-run` plus reason. Reading a test is not executing it. |
| `uncertainties` | Missing paths, alternative explanations, unavailable dependencies, and limitations; explicit `none-known` where justified. |
| `source_refs` | Stable private artifact or authorized immutable source references; include documentation revision or owner decision when relevant. |
| `review` | Reviewer role, date, rationale, owner disposition (`pending`, `accepted`, `changes-requested`, `rejected`), and decision reference. |
| `relationships` | Supporting/conflicting claim IDs and `supersedes` references; empty list if none. |
| `visibility` | Private classification, permitted audience, and approved sanitized derivative if any. |

Use explicit missing-value reasons. A numeric zero means measured zero, not missing data. Qualitative confidence is optional and cannot replace evidence or review.

## Synthetic example (not case evidence)

```yaml
claim_id: EXAMPLE-C01
statement: "The inspected handler rejects an empty item list before persistence."
scope: "The inspected handler's empty-list branch only."
claim_type: observation
review_status: unreviewed
case_revision: synthetic-fixture-v1
file_or_symbol: example/handler.py:create_order
observation_method: static-code
test_evidence:
  outcome: not-run
  reason: "Example illustrates the schema; no case tests were executed."
uncertainties:
  - "Other entry points and concurrent writes are outside the observation."
source_refs: [synthetic-fixture-v1/example/handler.py]
review:
  owner_disposition: pending
  rationale: "Illustrative record, not reviewed evidence."
relationships: []
visibility: public-synthetic
```

An apparently conflicting document becomes a separate `documented-intent` record. An owner decision creates a separate linked record; it does not overwrite the code observation. A later code revision requires revalidation rather than silently retaining `supported` status.

## Evaluation measures

Freeze the selected reference questions and their reference assertions privately before reconstruction. The owner or an authorized evaluator compares the frozen output against that reference after reconstruction, with a recorded rubric and disagreements.

- Unsupported-claim rate: assertions without adequate cited support / assertions reviewed; report both counts and zero-denominator cases as `not-applicable`.
- Reference coverage: supported in-scope reference assertions recovered / in-scope reference assertions reviewed. This measures the selected reference, not all application behavior.
- Contradictions and omissions: counts plus severity and claim IDs; owner-adjudicated, not automatically defects.
- Rework: correction cycles and changed claims; owner-active review minutes separately from waiting time.
- Cost and effort: measured telemetry and wall time alongside clearly labeled estimates. One run cannot establish comparative savings or model superiority.
