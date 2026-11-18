# ScoreGate Contracts Engineering Audit Backlog

This local backlog contains 100 expanded issue drafts. Final validation notes are recorded below. Navigation numbers are outside the publishable issue bodies; priority is the only classification in each body. Proposed existing GitHub labels appear only in the metadata table.

Review baseline: `main` at `71799a3` in `hartz0/scoregate-contracts`, including preserved local cleanup edits. The refreshed exclusion inventory contains 259 published issues and 70 pull requests (329 records, #1–#329). Inherited candidate titles were investigation leads only and have been removed from the deliverable.

## Draft metadata

| Navigation | Title | Proposed GitHub labels |
|---|---|---|
| 1 | Make schema drift checks read-only | `bug`, `tooling` |
| 2 | Make generated JSON Schema documents validate their root type | `bug`, `tooling` |
| 3 | Measure fixed byte fields in base64 characters in generated schemas | `bug`, `tooling` |
| 4 | Collect Any imports when generating Python annotations | `bug`, `tooling` |
| 5 | Preserve union grouping in TypeScript array element types | `bug`, `tooling` |
| 6 | Preserve result tags in generated Python models | `bug`, `tooling` |
| 7 | Build release reproducibility samples in independent build directories | `bug`, `tooling` |
| 8 | Check out repository history before generating release notes | `bug`, `tooling` |
| 9 | Use Cargo unit-test targets in mutation testing configuration | `bug`, `testing`, `tooling` |
| 10 | Reject invalid base references in error stability checks | `bug`, `tooling` |
| 11 | Enumerate on-chain-only records during reconciliation | `bug`, `tooling` |
| 12 | Parse documented WASM budgets without silently substituting defaults | `bug`, `tooling` |
| 13 | Reject repeated initialization in both mock consumers | `bug`, `security` |
| 14 | Bind resumed traceability checkpoints to the complete input | `bug`, `tooling` |
| 15 | Validate checkpoint structure before using nested values | `bug`, `tooling` |
| 16 | Report empty traceability input as lacking evidence | `bug`, `tooling` |
| 17 | Validate traceability test identifiers before counting coverage | `bug`, `tooling` |
| 18 | Distinguish traceability references from executed tests | `documentation`, `tooling` |
| 19 | Treat missing observations as replay determinism differences | `bug`, `tooling` |
| 20 | Sort replay state differences for reproducible reports | `bug`, `tooling` |
| 21 | Bound event-export RPC calls and total collection size | `bug`, `tooling` |
| 22 | Make snapshot export replace output only after successful completion | `bug`, `tooling` |
| 23 | Repair fenced command blocks in the WASM size guide | `documentation` |
| 24 | Authenticate Stellar address checksums during manifest validation | `bug`, `tooling` |
| 25 | Expose a test environment without blanket authorization | `testing`, `enhancement` |
| 26 | Avoid overflow in the example AMM fee calculation | `bug`, `documentation` |
| 27 | Correct the AMM example claim that cross-contract calls cannot trap | `documentation`, `enhancement` |
| 28 | Implement the advertised cluster membership query | `feature`, `testing` |
| 29 | Calculate score age from the score observation timestamp | `bug` |
| 30 | Allow an idle registered oracle to recover on a subsequent consultation | `bug` |
| 31 | Hash score identities and complete records in state checksums | `bug`, `security` |
| 32 | Bound historical proposal cleanup independently of total proposal IDs | `performance`, `enhancement` |
| 33 | Apply score-domain bounds to bulk signer tier updates | `bug` |
| 34 | Report remaining capacity correctly in flat cooldown mode | `bug` |
| 35 | Make interface metadata enumerate every supported capability | `bug`, `enhancement` |
| 36 | Restrict reviewer approvals to existing bounded proposal targets | `bug`, `security` |
| 37 | Define conservative aggregate arbitration for equal timestamps | `bug` |
| 38 | Reject malformed or repeated replay headers | `bug`, `tooling` |
| 39 | Capture contract events rather than synthetic submission messages in replay evidence | `bug`, `tooling` |
| 40 | Validate numeric trade data before deriving replay scores | `bug`, `tooling` |
| 41 | Give replay input errors a path and line number | `enhancement`, `tooling` |
| 42 | Register the oracle adapter example as a Cargo build target | `testing`, `documentation` |
| 43 | Enforce tuple cardinality in generated JSON schemas | `bug`, `tooling` |
| 44 | Preserve map key and value types across generated bindings | `bug`, `tooling` |
| 45 | Resolve referenced user-defined types during schema generation | `bug`, `tooling` |
| 46 | Enforce XDR integer ranges in runtime schema validators | `bug`, `tooling` |
| 47 | Align Python model handling of unknown fields with JSON Schema | `enhancement`, `tooling` |
| 48 | Validate recovery export records beyond their JSON shape | `bug`, `tooling` |
| 49 | Compare recovery roots as canonical digest bytes | `bug`, `tooling` |
| 50 | Bind recovery snapshots to their network and contract | `bug`, `tooling` |
| 51 | Separate action time from report generation time in recovery reports | `enhancement`, `tooling` |
| 52 | Keep fuzzer mutations within the operation bound | `bug`, `tooling` |
| 53 | Preserve the failure category when shrinking fuzzer counterexamples | `bug`, `tooling` |
| 54 | Handle zero denominators in WASM attribution reports | `bug`, `tooling` |
| 55 | Include newly introduced modules in WASM growth diagnostics | `bug`, `tooling` |
| 56 | Validate qualified symbol ownership in the refinement checker | `bug`, `tooling` |
| 57 | Count actual tuple elements in event arity checks | `bug`, `tooling` |
| 58 | Upload production acceptance evidence when CI checks fail | `bug`, `tooling` |
| 59 | Run schema drift verification in pull request CI | `bug`, `tooling` |
| 60 | Provide authentic release provenance instead of calling a checksum a signature | `enhancement`, `tooling` |
| 61 | Bind optimized release artifacts to the reproducibility result | `bug`, `tooling` |
| 62 | Make release checksum manifests portable after download | `bug`, `tooling` |
| 63 | Pass release notes as data instead of interpolating them into shell source | `bug`, `tooling` |
| 64 | Attach the generated dependency inventory to releases | `enhancement`, `tooling` |
| 65 | Generate release download instructions for the actual repository | `documentation`, `tooling` |
| 66 | Lock dependency resolution in the deployment build | `bug`, `tooling` |
| 67 | Resolve deployment identities before creating the contract | `bug`, `tooling` |
| 68 | Compare deployed configuration with intended values before reporting success | `bug`, `tooling` |
| 69 | Anchor deployment build paths to the repository root | `enhancement`, `tooling` |
| 70 | Make canary dry runs fully offline and non-mutating | `bug`, `tooling` |
| 71 | Require a successful score round trip before declaring canary success | `bug`, `tooling` |
| 72 | Restore the original pause state after operational rehearsal | `bug`, `tooling` |
| 73 | Compare baseline and final state during canary reconciliation | `bug`, `tooling` |
| 74 | Reject incomplete reconciliation records instead of inventing values | `bug`, `tooling` |
| 75 | Reject duplicate logical keys in reconciliation input | `bug`, `tooling` |
| 76 | Process the final reconciliation record without requiring a newline | `bug`, `tooling` |
| 77 | Build reconciliation reports without repeatedly copying the whole array | `performance`, `tooling` |
| 78 | Exclude stale WASM files from production acceptance evidence | `bug`, `tooling` |
| 79 | Honor explicit WASM paths in the size-report command | `enhancement`, `tooling` |
| 80 | Collect SBOM outputs from a bounded generation location | `bug`, `tooling` |
| 81 | Register documentation synchronization tests with Cargo | `testing`, `documentation` |
| 82 | Keep replacement governance proposals executable in the formal model | `bug`, `testing` |
| 83 | Model observable gate decisions in the embargo safety property | `testing`, `enhancement` |
| 84 | Check upgrade approval snapshot safety in the formal model | `testing`, `enhancement` |
| 85 | Compile and test the replay analysis modules through the library | `bug`, `tooling` |
| 86 | Expose the documented configuration drift command in the replay CLI | `bug`, `tooling` |
| 87 | Reject incomplete configuration manifests before declaring no drift | `bug`, `tooling` |
| 88 | Make error coverage checks verify executable per-variant tests | `testing`, `tooling` |
| 89 | Configure Criterion harnesses for every benchmark suite | `testing`, `tooling` |
| 90 | Measure the enabled noise path in the private aggregate benchmark | `testing`, `performance` |
| 91 | Populate model statistics summary fields on each accepted submission | `bug` |
| 92 | Connect pair volatility updates to accepted score finalization | `bug` |
| 93 | Validate static correlation coefficients before storing them | `bug` |
| 94 | Preserve hysteresis validity when the risk threshold changes | `bug` |
| 95 | Separate immediate cooldown updates from timelocked governance proposals | `enhancement` |
| 96 | Scope contributor WASM build commands to deployable crates | `documentation` |
| 97 | Repair broken local links in operational documentation | `documentation` |
| 98 | Generate syntactically valid Python for empty contract structs | `bug`, `tooling` |
| 99 | Offer a strict exit status for recovery snapshot divergence | `enhancement`, `tooling` |
| 100 | Enforce the capability and resource assertions in SDK conformance fixtures | `testing`, `enhancement` |

## Draft 1

### Title

Make schema drift checks read-only

### Priority

Medium

### Summary

Schema check mode modifies the artifacts it is supposed to inspect, hiding drift from subsequent runs.

### Problem / Evidence

`tools/schema-gen/src/main.rs` — `main / write_if_changed`. The write_type closure invokes write_if_changed for all twelve artifacts before main examines check && any_changed. write_if_changed writes both missing and changed files. Thus --check repairs the evidence of drift before returning an error, contrary to its help text.

### Expected Behavior

Check mode detects drift without creating directories or changing artifacts.

### Proposed Solution

Separate rendering/comparison from writes; permit writes only in regeneration mode.

### Acceptance Criteria

- [ ] A stale or missing artifact produces a nonzero check result and leaves the directory byte-for-byte unchanged; normal regeneration still writes all artifacts.

### Validation / Test Plan

Run the CLI against a temporary output tree with stale, missing, and matching files; compare file hashes and directory entries before and after each check.

## Draft 2

### Title

Make generated JSON Schema documents validate their root type

### Priority

Medium

### Summary

Generated schema documents leave all validation constraints inside an unreferenced definition, so invalid root instances can pass.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `struct_to_json_schema`. The generated document contains the object constraints only under $defs and has no root $ref or root object constraints. A validator invoked on the document therefore has no object requirements to enforce. The same risk_score.schema.json $id is also emitted for every struct.

### Expected Behavior

Each schema validates instances of its named type and has a distinct identity.

### Proposed Solution

Emit a root reference to the generated definition and derive the schema ID from the target artifact name. Keep field shapes unchanged.

### Acceptance Criteria

- [ ] An empty object and a scalar fail RiskScore validation; a complete valid object passes; four generated documents have distinct IDs.

### Validation / Test Plan

Use a draft-07 validator on valid and invalid instances for each generated root; verify referenced definitions resolve without external network access.

## Draft 3

### Title

Measure fixed byte fields in base64 characters in generated schemas

### Priority

Medium

### Summary

Fixed-byte schemas measure raw bytes as encoded string characters and reject valid base64 values.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `bytes_schema`. bytes_schema(n) sets minLength and maxLength to n, although contentEncoding is base64. For BytesN<32>, canonical padded base64 has 44 characters, so the current length restriction rejects a valid encoded value.

### Expected Behavior

Fixed-size byte schema constraints match the documented wire encoding.

### Proposed Solution

Define padding rules explicitly and generate constraints for encoded length and decoded byte size; do not treat raw byte count as character count.

### Acceptance Criteria

- [ ] A valid 32-byte base64 value passes; 31- and 33-byte values fail decoded-size validation; variable Bytes remains supported.

### Validation / Test Plan

Add vectors at raw lengths 1, 2, 3, 31, 32, and 33 and validate canonical and malformed encodings.

## Draft 4

### Title

Collect Any imports when generating Python annotations

### Priority

Low

### Summary

Generated Python annotations can refer to Any without importing it, preventing supported model shapes from loading.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `py_type / struct_to_python`. The Val arm returns Any without adding it to needs. The Map arm records Dict but returns Dict[str, Any] without recording Any. struct_to_python emits typing imports only from needs, producing unresolved annotations for these supported type branches.

### Expected Behavior

Every generated annotation resolves when the Python model is loaded.

### Proposed Solution

Record Any whenever emitted, including nested values; retain deterministic deduplicated imports.

### Acceptance Criteria

- [ ] Synthetic Val and Map fields produce an Any import exactly once; generated models import successfully.

### Validation / Test Plan

Generate models for Val, Map, and nested Option/Vec combinations and load them under Pydantic v2 in an isolated Python process.

## Draft 5

### Title

Preserve union grouping in TypeScript array element types

### Priority

Medium

### Summary

Vector rendering loses union precedence and changes the meaning of nested TypeScript types.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `ts_type`. The Vec arm appends [] directly to the recursively rendered element. Vec<Option<U32>> becomes number | null[], which means a number or an array of null rather than an array whose elements are numbers or null.

### Expected Behavior

Nested type composition retains the XDR container structure.

### Proposed Solution

Use Array<T> or precedence-aware parenthesization for vector elements.

### Acceptance Criteria

- [ ] Vec<Option<U32>> accepts [1, null] and rejects scalar 1; nested vectors and result unions retain their structure.

### Validation / Test Plan

Generate synthetic XDR fixtures and compile positive and negative assignment samples with tsc --noEmit; keep existing integer precision behavior.

## Draft 6

### Title

Preserve result tags in generated Python models

### Priority

Medium

### Summary

Python result unions lose the distinction between success and error when their payload types overlap.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `py_type`. The Result arm renders Union[ok_type, err_type], whereas json_schema_type and ts_type retain explicit ok and err object tags. When both branches use the same primitive, Python cannot represent which branch was returned.

### Expected Behavior

Python bindings preserve the same success/error distinction as the other generated formats.

### Proposed Solution

Generate tagged result models or a compatible discriminated representation, including nested results. Document the serialized representation.

### Acceptance Criteria

- [ ] Result<U32,U32> round-trips success and error as distinct values; nested result fields preserve their tags.

### Validation / Test Plan

Generate synthetic result fields, deserialize both branches, serialize them again, and compare with corresponding JSON Schema and TypeScript representations.

## Draft 7

### Title

Build release reproducibility samples in independent build directories

### Priority

Medium

### Summary

The release reproducibility check can compare a cached build output with itself instead of two independent compilations.

### Problem / Evidence

`.github/workflows/release.yml` — `reproducibility-check`. Both build runs occur as steps in the same job and invoke the same cargo build command against the same target directory. No step removes or isolates target between builds, despite comments describing independent containers. The second hash can therefore cover a reused artifact.

### Expected Behavior

Both compared WASM files come from independent compilations of the same commit.

### Proposed Solution

Use separate jobs or fresh CARGO_TARGET_DIR directories with identical pinned inputs; compare the resulting artifacts.

### Acceptance Criteria

- [ ] Neither compilation can read the other compilation output; both hashes are derived from fresh builds and compared before publication.

### Validation / Test Plan

Inspect job dependencies and logs for two real rustc compilations; test that substituting a differing artifact makes comparison fail.

## Draft 8

### Title

Check out repository history before generating release notes

### Priority

High

### Summary

The release publication job cannot read changelog files or Git history because it never checks out the repository.

### Problem / Evidence

`.github/workflows/release.yml` — `publish-release`. publish-release downloads build artifacts but has no checkout step. Its release-note shell reads CHANGELOG.md and falls back to git tag and git log. Those commands require repository files and history that a fresh job does not receive from the preceding jobs.

### Expected Behavior

The publication job can read the tagged changelog and enumerate prior release history.

### Proposed Solution

Check out the exact release tag with the history required for the fallback; initialize the notes variable and handle a first release explicitly.

### Acceptance Criteria

- [ ] Changelog extraction and history fallback both work in a clean runner; generated notes correspond to the tagged source.

### Validation / Test Plan

Exercise note-generation commands in clean temporary checkouts with a changelog section, an empty section, and no earlier contract tag; do not create a remote release.

## Draft 9

### Title

Use Cargo unit-test targets in mutation testing configuration

### Priority

Medium

### Summary

Mutation shard configuration names unit-test modules as integration-test targets, preventing the intended baseline tests from running.

### Problem / Evidence

`.cargo/mutants.toml` — `additional_cargo_args`. The configuration passes --test test_zk_range_proof, --test test_verkle, and other names corresponding to modules in contracts/scoregate-score/src. The crate does not declare integration-test targets with those names. Cargo --test selects integration targets rather than unit-test modules.

### Expected Behavior

Mutation campaigns execute the intended unit tests instead of failing target selection.

### Proposed Solution

Select the library test target and use supported module filters or shard-specific selection; align the workflow and mutation-test script with that selection.

### Acceptance Criteria

- [ ] Every configured shard completes its unmutated baseline test selection; no configured --test argument names a nonexistent Cargo target.

### Validation / Test Plan

Compare cargo metadata target names with the configuration and run each shard baseline after contract compilation is restored.

## Draft 10

### Title

Reject invalid base references in error stability checks

### Priority

Medium

### Summary

An invalid Git reference makes the ABI stability checker skip comparison and return success.

### Problem / Evidence

`tools/check_error_discriminants.sh` — `extract_discriminants`. extract_discriminants suppresses every git show or extraction failure with || true. A nonexistent base ref produces empty base_pairs and exits zero through the skip branch. Running bash tools/check_error_discriminants.sh scoregate-nonexistent-ref HEAD reproduced that successful skip.

### Expected Behavior

Unavailable comparison history fails explicitly instead of passing an ABI check.

### Proposed Solution

Validate commit refs before extraction and distinguish an absent historical file from an invalid ref or malformed extraction. Keep the separately tracked multi-contract expansion out of scope.

### Acceptance Criteria

- [ ] An invalid base or head ref exits nonzero; a valid comparison still enforces existing discriminants; intentional historical file absence has an explicit policy.

### Validation / Test Plan

Test invalid refs, shallow history, a missing historical file, a renamed discriminant, an appended alias, and identical refs.

## Draft 11

### Title

Enumerate on-chain-only records during reconciliation

### Priority

Medium

### Summary

Reconciliation never discovers records absent from the pipeline input, leaving its on-chain-only count permanently zero.

### Problem / Evidence

`scripts/reconcile.sh` — `reconciliation loop`. ONCHAIN_ONLY is initialized to zero and included in the output totals, but the reconciliation loop visits only rows from PIPELINE and never increments ONCHAIN_ONLY. Scores existing exclusively on chain cannot enter the report.

### Expected Behavior

The report detects records present on either side of the comparison.

### Proposed Solution

Obtain a paginated on-chain inventory or require an explicit complete export, then reconcile the union of wallet/pair keys. Bound work and distinguish incomplete inventories.

### Acceptance Criteria

- [ ] An on-chain key absent from the pipeline appears once with onchain_only status and increments the total; common and pipeline-only keys retain their classifications.

### Validation / Test Plan

Stub CLI responses for multiple pages, including a chain-only key, an empty pipeline, and an interrupted page fetch; assert counts and fail on incomplete inventory.

## Draft 12

### Title

Parse documented WASM budgets without silently substituting defaults

### Priority

Medium

### Summary

The size-budget parser cannot read the documented baseline and silently substitutes a larger allowance.

### Problem / Evidence

`scripts/check-wasm-size.sh` — `per-contract budget extraction`. The grep pipeline requires the crate name and a numeric bytes value on the same line. docs/wasm-size-budget.md puts scoregate-score on Target Contract and 599,000 bytes on a separate Total Binary Size line. The parser therefore misses that documented budget and substitutes 1048576.

### Expected Behavior

The enforced size ceiling matches an explicit budget for each contract.

### Proposed Solution

Store budgets in a structured source shared by documentation and the check, or parse an unambiguous table. Treat a missing budget as an error rather than silently weakening it.

### Acceptance Criteria

- [ ] The score contract uses its documented budget; each other checked contract has an explicit budget; malformed or absent values fail clearly.

### Validation / Test Plan

Use stub WASM files or a size-reader fixture to exercise below, exactly at, and above the tolerance ceiling; test missing and malformed budget records.

## Draft 13

### Title

Reject repeated initialization in both mock consumers

### Priority

High

### Summary

An authenticated unrelated account can reinitialize either mock consumer and replace an established administrator and oracle configuration.

### Problem / Evidence

`contracts/mock-amm/src/lib.rs` and `contracts/mock-lending/src/lib.rs` — `MockAmm::initialize / MockLending::initialize`. Both entry points authenticate the supplied admin, then overwrite DataKey::Admin and the oracle configuration without checking whether an administrator is already stored. An unrelated authenticated account can invoke initialization again and replace an established fixture configuration.

### Expected Behavior

A second initialization from either the original or a different administrator fails and preserves all configuration; first initialization still succeeds.

### Proposed Solution

Check initialization state before accepting configuration. Return an existing compatible error or append a documented alias without changing existing discriminants.

### Acceptance Criteria

- [ ] A second initialization from either the original or a different administrator fails and preserves all configuration; first initialization still succeeds.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Use real authorization entries for two distinct accounts and assert stored admin, oracle, threshold, and failure policy remain unchanged after each rejected call.

## Draft 14

### Title

Bind resumed traceability checkpoints to the complete input

### Priority

Medium

### Summary

Resuming a checkpoint after input edits can reuse stale coverage decisions for unchanged issue identifiers.

### Problem / Evidence

`tools/replay/traceability_report.py` — `load_checkpoint / main`. Resume compares only the issue_id prefix. If invariant IDs or test_ids change under those same issue IDs, processed_items from the old checkpoint are reused, including their verified flags, instead of recomputing coverage from the current input.

### Expected Behavior

Editing an invariant or removing a test reference invalidates a checkpoint even when issue IDs are unchanged; an unchanged input resumes to the same coverage as a clean run.

### Proposed Solution

Include a deterministic fingerprint of normalized input and checkpoint format version, and reject or recompute stale checkpoints.

### Acceptance Criteria

- [ ] Editing an invariant or removing a test reference invalidates a checkpoint even when issue IDs are unchanged; an unchanged input resumes to the same coverage as a clean run.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Generate a checkpoint, alter test_ids under an existing issue, and compare resumed and fresh runs; also test reordered semantically identical input.

## Draft 15

### Title

Validate checkpoint structure before using nested values

### Priority

Medium

### Summary

Nested malformed checkpoint data can escape validation and crash the report generator instead of producing its documented error status.

### Problem / Evidence

`tools/replay/traceability_report.py` — `load_checkpoint`. Only last_index being an int and processed_items being a list are checked. main then calls item.get and inv.get and adds arbitrary test_ids to a set. Non-object entries, non-object invariants, and unhashable IDs can raise uncaught exceptions instead of EXIT_CHECKPOINT_ERROR. Negative indices and bool indices also pass the current integer test.

### Expected Behavior

Malformed nested objects and invalid indices produce exit code 4 with a useful message and leave output files untouched.

### Proposed Solution

Validate the complete checkpoint schema and index bounds before reading nested values.

### Acceptance Criteria

- [ ] Malformed nested objects and invalid indices produce exit code 4 with a useful message and leave output files untouched.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Exercise null/list processed items, malformed invariant collections, object test IDs, negative and boolean indices, and a well-formed checkpoint.

## Draft 16

### Title

Report empty traceability input as lacking evidence

### Priority

Medium

### Summary

A traceability input containing no invariants passes strict mode without supplying any coverage evidence.

### Problem / Evidence

`tools/replay/traceability_report.py` — `build_report`. status is PASSED whenever total_invariants equals covered_invariants. With zero invariants both are zero, so an empty list or issues with empty invariant lists pass strict mode while reporting 0% coverage.

### Expected Behavior

Empty input and zero-invariant issues cannot produce a successful strict coverage gate; nonempty fully covered input still passes.

### Proposed Solution

Define an explicit no-evidence state and make strict mode reject it.

### Acceptance Criteria

- [ ] Empty input and zero-invariant issues cannot produce a successful strict coverage gate; nonempty fully covered input still passes.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Run strict mode on [], an issue with no invariants, one uncovered invariant, and one covered invariant; verify statuses and exit codes.

## Draft 17

### Title

Validate traceability test identifiers before counting coverage

### Priority

Medium

### Summary

Blank and boolean test identifiers count as evidence even though they are not meaningful test references.

### Problem / Evidence

`tools/replay/traceability_report.py` — `validate_issue / main`. test IDs accept isinstance(value, (str, int)), which admits booleans and empty strings. main marks an invariant verified solely when the list is nonempty, so [false] or [""] supplies apparent coverage.

### Expected Behavior

Invalid identifiers fail input validation and cannot increase coverage; equivalent duplicate identifiers count once.

### Proposed Solution

Require nonblank string identifiers or explicitly supported integer identifiers, rejecting booleans; normalize and deduplicate consistently.

### Acceptance Criteria

- [ ] Invalid identifiers fail input validation and cannot increase coverage; equivalent duplicate identifiers count once.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test empty/whitespace strings, booleans, integers, repeated IDs, and valid named IDs; check exit code 2 for malformed inputs.

## Draft 18

### Title

Distinguish traceability references from executed tests

### Priority

Low

### Summary

Mapping-only traceability output claims tests were executed even though the tool neither runs tests nor ingests their results.

### Problem / Evidence

`tools/replay/traceability_report.py` — `generate_human_readable / main`. Human output says Total Tests Executed and VERIFIED, but the program only counts user-provided test_ids and does not run tests or ingest test results. This makes a mapping report look like evidence that tests passed.

### Expected Behavior

A mapping-only report does not claim execution or passing tests; JSON and human output describe the same evidence level.

### Proposed Solution

Use referenced/linked terminology, or add explicit result ingestion before making execution claims. Document the meaning of the coverage metric.

### Acceptance Criteria

- [ ] A mapping-only report does not claim execution or passing tests; JSON and human output describe the same evidence level.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Generate a report referencing a nonexistent test ID and confirm the output describes a reference, not a successful execution.

## Draft 19

### Title

Treat missing observations as replay determinism differences

### Priority

Medium

### Summary

One-sided state, events, and measurements can appear in difference details while the overall determinism verdict remains true.

### Problem / Evidence

`tools/replay/src/determinism.rs` — `compare_results`. Missing state keys and unmatched trailing events populate detail vectors but add a divergence only when both sides are Some. is_deterministic uses divergences.is_empty(). Optional resource metrics are likewise compared only when both exist. A one-sided observation can therefore be listed as different while the overall result says deterministic.

### Expected Behavior

Adding or removing a key, event, or measured metric cannot leave is_deterministic true; identical results remain true.

### Proposed Solution

Classify one-sided state, event, and metric observations explicitly and derive status consistently from all difference categories.

### Acceptance Criteria

- [ ] Adding or removing a key, event, or measured metric cannot leave is_deterministic true; identical results remain true.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test each one-sided category in both argument orders, including one extra final event and Some(0) versus None.

## Draft 20

### Title

Sort replay state differences for reproducible reports

### Priority

Low

### Summary

Hash-set iteration gives otherwise identical determinism reports unstable diagnostic ordering.

### Problem / Evidence

`tools/replay/src/determinism.rs` — `compare_results`. State keys are collected in a HashSet and iterated directly into state_differences and divergences. Hash iteration order is not stable, so serializing identical comparisons can produce differently ordered diagnostic arrays.

### Expected Behavior

Identical comparisons produce byte-identical diagnostic ordering regardless of state map insertion order.

### Proposed Solution

Use ordered key iteration or explicitly sort difference records before returning the report.

### Acceptance Criteria

- [ ] Identical comparisons produce byte-identical diagnostic ordering regardless of state map insertion order.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Construct equivalent maps in different orders with several changed keys; compare serialized reports over repeated processes.

## Draft 21

### Title

Bound event-export RPC calls and total collection size

### Priority

Medium

### Summary

An unbounded RPC request or ledger export can stall the exporter indefinitely or exhaust its memory.

### Problem / Evidence

`scripts/fetch_testnet_snapshot.py` — `fetch_events`. urlopen is called without a timeout, and every page is appended to an in-memory events list without a page, record, or byte ceiling. A slow endpoint can stall indefinitely, while a large ledger range can exhaust local memory.

### Expected Behavior

A stalled request terminates with an actionable error; configured limits are enforced and incomplete exports are distinguishable from successful complete exports.

### Proposed Solution

Add configurable request deadlines and bounded pagination or stream records to a temporary output; report truncation explicitly rather than presenting partial data as complete.

### Acceptance Criteria

- [ ] A stalled request terminates with an actionable error; configured limits are enforced and incomplete exports are distinguishable from successful complete exports.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Use a local HTTP fixture that stalls, returns many pages, repeats a cursor, and returns an error after partial progress; assert bounded runtime and output handling.

## Draft 22

### Title

Make snapshot export replace output only after successful completion

### Priority

Medium

### Summary

A failed snapshot conversion can destroy a previously valid export and leave a partial file at its final path.

### Problem / Evidence

`scripts/fetch_testnet_snapshot.py` — `main`. The output file is opened with mode w before records are converted and written. A conversion or write failure after that point destroys the previous export and leaves a partial file at the requested final path.

### Expected Behavior

An existing valid export survives conversion or write failure; successful export replaces it completely.

### Proposed Solution

Write to a temporary sibling file and atomically replace the final output only after successful conversion and close. Clean temporary files on errors.

### Acceptance Criteria

- [ ] An existing valid export survives conversion or write failure; successful export replaces it completely.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Inject a conversion exception and a simulated write failure after one record, compare the old output hash, and verify successful replacement.

## Draft 23

### Title

Repair fenced command blocks in the WASM size guide

### Priority

Low

### Summary

Malformed Markdown fences hide section boundaries and mix prose into copyable shell commands.

### Problem / Evidence

`docs/wasm-size-budget.md` — Local Reproduction Steps. The installation block ends with a backtick fence carrying the text yaml, which is not a valid closing fence. The automated reporting block has no closing fence before Manual Analysis Commands, and the final shell block repeats the malformed closing marker. The rendered guide can absorb headings and narrative into code blocks.

### Expected Behavior

Each shell example renders as its own complete code block, and subsequent headings and prose render outside it.

### Proposed Solution

Repair the fence boundaries and add a lightweight Markdown structure check for documentation command blocks. Preserve the commands and budget policy unless separately reviewed.

### Acceptance Criteria

- [ ] Installation, automated analysis, and manual analysis each have correctly closed shell blocks.
- [ ] All section headings render as headings, and copying a command block includes no surrounding prose.

### Validation / Test Plan

Render the page with a CommonMark-compatible parser and inspect its heading/code-block nodes; run the documentation lint and manually inspect the three copyable examples.

## Draft 24

### Title

Authenticate Stellar address checksums during manifest validation

### Priority

Medium

### Summary

Address validation checks shape but not the checksum, allowing invalid account identifiers to survive preflight.

### Problem / Evidence

`deploy/validate_manifest.sh` — `manifest_is_valid_stellar_address`. The validator only checks the G prefix, length, and base32 alphabet. It accepts syntactically plausible strings with an invalid StrKey checksum, despite calling them valid Stellar public keys. Such input survives local preflight and fails later in CLI or contract processing.

### Expected Behavior

A checksum-mutated otherwise well-formed key is rejected; valid account keys pass and unsupported address types receive clear diagnostics.

### Proposed Solution

Decode the StrKey and validate its version and checksum with an existing supported library or CLI preflight, without submitting transactions.

### Acceptance Criteria

- [ ] A checksum-mutated otherwise well-formed key is rejected; valid account keys pass and unsupported address types receive clear diagnostics.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Use known valid account keys, mutate a checksum character, and test invalid version, alphabet, and length cases. Keep network calls unnecessary.

## Draft 25

### Title

Expose a test environment without blanket authorization

### Priority

Low

### Summary

The shared test environment helper always bypasses authorization, making strict authorization setup unavailable through its API.

### Problem / Evidence

`contracts/scoregate-test-support/src/lib.rs` — `test_env`. The common test_env helper always calls mock_all_auths and the unlimited-budget helper builds on it. Callers adopting the shared helper cannot express the distinction between authorization-sensitive setup and intentionally mocked positive-path setup through its API.

### Expected Behavior

A caller can obtain a configured test Env without blanket mocks; an unsigned administrative call in a focused regression test fails.

### Proposed Solution

Add an explicitly named environment constructor with normal authorization enabled and clearly name/document helpers that blanket-mock authorization. Migrate appropriate authorization tests to the strict constructor.

### Acceptance Criteria

- [ ] A caller can obtain a configured test Env without blanket mocks; an unsigned administrative call in a focused regression test fails.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Add a small contract-backed authorization test showing unsigned rejection and explicitly authorized success; preserve existing positive fixtures.

## Draft 26

### Title

Avoid overflow in the example AMM fee calculation

### Priority

Low

### Summary

The example fee calculation overflows for large valid u64 inputs even though its final result fits.

### Problem / Evidence

`examples/amm_gate_example.rs` — `SimpleAMM::compute_swap_output`. The formula amount_in * 997 / 1000 multiplies in u64. Amounts above u64::MAX / 997 overflow even though the final quotient is representable. Release overflow checks are enabled in Cargo.toml, so the example traps for those inputs.

### Expected Behavior

The calculation succeeds for the full u64 input domain and preserves floor rounding and the existing 1,000,000 example.

### Proposed Solution

Perform the intermediate multiplication in u128 and convert the bounded quotient back to u64.

### Acceptance Criteria

- [ ] The calculation succeeds for the full u64 input domain and preserves floor rounding and the existing 1,000,000 example.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test zero, one, u64::MAX / 997, the next value, and u64::MAX against a u128 reference.

## Draft 27

### Title

Correct the AMM example claim that cross-contract calls cannot trap

### Priority

Low

### Summary

AMM examples promise cross-contract calls cannot fail, encouraging integrations that do not handle unavailable dependencies.

### Problem / Evidence

`examples/amm_gate.rs` and `examples/amm_gate_example.rs` — `module documentation / swap`. The examples assert the gate cannot fail and omit try wrappers on that basis. A boolean contract return type does not prevent a call to an absent or incompatible contract from failing; SimpleAMM also accepts the oracle address as an argument. Integrators are told to copy an overly strong guarantee.

### Expected Behavior

Documentation no longer promises that arbitrary cross-contract calls cannot trap; the example handles missing and incompatible dependencies through its documented error path.

### Proposed Solution

Describe the distinction between a fail-closed gate result and invocation failure, and demonstrate an explicit consumer policy using the generated try client.

### Acceptance Criteria

- [ ] Documentation no longer promises that arbitrary cross-contract calls cannot trap; the example handles missing and incompatible dependencies through its documented error path.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Invoke the example with a valid registry, an unregistered address, and an incompatible stub contract; verify documented consumer outcomes.

## Draft 28

### Title

Implement the advertised cluster membership query

### Priority

Medium

### Summary

The public cluster membership query returns ScoreNotFound for every input instead of enumerating existing members.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `get_cluster_members`. The function constructs an empty Vec, computes unused cluster bounds, and always returns ScoreNotFound. Its documentation promises a scan returning up to 200 wallets. Existing scored wallets therefore cannot be discovered through this API.

### Expected Behavior

A scored wallet is returned for its assigned cluster; wrong-pair and wrong-cluster wallets are excluded; invalid cluster IDs cannot overflow arithmetic.

### Proposed Solution

Implement bounded membership enumeration with defined boundary semantics and a pagination strategy if needed. Align assignment and membership with the same cluster definition.

### Acceptance Criteria

- [ ] A scored wallet is returned for its assigned cluster; wrong-pair and wrong-cluster wallets are excluded; invalid cluster IDs cannot overflow arithmetic.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test scores 0, 9, 10, 99, and 100; empty clusters, deleted scores, invalid IDs, and more than 200 members.

## Draft 29

### Title

Calculate score age from the score observation timestamp

### Priority

Medium

### Summary

Resetting rate-limit state changes reported score age even though the underlying observation has not changed.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `get_score_age`. get_score_age reads LastSubmitTime, which is rate-limit state, rather than RiskScore.timestamp. Administrative rate-limit resets can remove this state while leaving the score intact, causing age to become zero for an existing observation.

### Expected Behavior

Resetting cooldown state does not change a live score age; age advances with ledger time and never underflows for future timestamps.

### Proposed Solution

Define age as elapsed ledger time since the stored observation and use the score timestamp; preserve a documented missing-score return convention.

### Acceptance Criteria

- [ ] Resetting cooldown state does not change a live score age; age advances with ledger time and never underflows for future timestamps.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Submit a score, advance time, override the rate limit, and query age before and after; cover no-score and future-timestamp cases.

## Draft 30

### Title

Allow an idle registered oracle to recover on a subsequent consultation

### Priority

Medium

### Summary

An idle oracle cannot become fresh through consultation once its cached consultation timestamp triggers the stale branch.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `get_effective_score`. When oracle_last_updated is nonzero and older than the configured threshold, the method returns the fallback floor without invoking the oracle. Only the successful invocation branch updates oracle_last_updated. Once consultation age crosses the threshold, this read path cannot refresh itself even if the oracle has fresh data.

### Expected Behavior

After an idle interval, a fresh oracle response restores the confidence adjustment; unavailable or stale data retains the documented fallback.

### Proposed Solution

Distinguish oracle data freshness from local consultation age and attempt a bounded, trapped refresh before deciding to fall back.

### Acceptance Criteria

- [ ] After an idle interval, a fresh oracle response restores the confidence adjustment; unavailable or stale data retains the documented fallback.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Use a controllable oracle stub, advance beyond the threshold, update its data, and query again; test an invocation error and genuinely stale data.

## Draft 31

### Title

Hash score identities and complete records in state checksums

### Priority

High

### Summary

State checksums omit record identities and several persisted fields, so materially different states can share a checksum.

### Problem / Evidence

`contracts/scoregate-score/src/storage.rs` — `compute_score_root`. The preimage contains only score, timestamp, and model_version for each indexed record. Wallet, asset_pair, confidence, component scores, flags, and commitment are omitted. Moving the same numeric observation to a different key or changing omitted fields can leave the root unchanged.

### Expected Behavior

Changing any persisted record field or its key changes the root; equivalent states inserted or touched in different orders produce the same root; count reflects live records.

### Proposed Solution

Define a versioned canonical encoding of each complete keyed score record and hash it in a stable key order. Document snapshot compatibility and migration.

### Acceptance Criteria

- [ ] Changing any persisted record field or its key changes the root; equivalent states inserted or touched in different orders produce the same root; count reflects live records.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Create paired states differing in each omitted field and identity, plus equivalent states with different insertion orders; verify root and count expectations.

## Draft 32

### Title

Bound historical proposal cleanup independently of total proposal IDs

### Priority

Medium

### Summary

Historical proposal cleanup probes every lifetime proposal ID, including removed records, without a per-call scan budget.

### Problem / Evidence

`contracts/scoregate-score/src/storage.rs` — `cleanup_expired_parameter_proposals`. Cleanup iterates 1..ParameterProposalNextId, probing every historical ID even when most records have been removed. Per-call cost therefore grows with lifetime proposal volume rather than remaining records or a maintenance budget. This is a different loop from the pending-vector pruning addressed in the published pruning issue.

### Expected Behavior

A call examines no more than the configured budget; repeated calls eventually remove eligible records; missing IDs cannot cause lifetime-sized work in one call.

### Proposed Solution

Use a resumable cursor and explicit scan budget, or traverse a bounded retained index, updating indices consistently when records are removed.

### Acceptance Criteria

- [ ] A call examines no more than the configured budget; repeated calls eventually remove eligible records; missing IDs cannot cause lifetime-sized work in one call.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Seed a large next ID with sparse live records and verify bounded work and cursor progress across repeated cleanup calls.

## Draft 33

### Title

Apply score-domain bounds to bulk signer tier updates

### Priority

Medium

### Summary

Bulk signer-tier updates admit bounds that the single-entry setter correctly rejects.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `bulk_set_signer_tier`. The bulk setter only rejects min_score > max_score. The single setter rejects either bound above 100. An entry such as (registered_signer, 101, 200) is accepted through the bulk API, producing a configuration outside the documented score domain.

### Expected Behavior

Both entry points reject bounds above 100 and inverted intervals; valid inclusive intervals remain supported; invalid batches leave no partial configuration.

### Proposed Solution

Share tier validation between single and bulk setters, retaining the batch bound and authorization checks.

### Acceptance Criteria

- [ ] Both entry points reject bounds above 100 and inverted intervals; valid inclusive intervals remain supported; invalid batches leave no partial configuration.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test 0..100, 100..100, 101..200, inverted bounds, and an invalid final batch element, checking rollback.

## Draft 34

### Title

Report remaining capacity correctly in flat cooldown mode

### Priority

Medium

### Summary

The remaining-token getter reports capacity during a flat-mode cooldown even when another submission would be rejected.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `get_remaining_tokens`. The getter returns capacity whenever get_token_bucket returns None. Flat cooldown mode uses LastSubmitTime instead of a token bucket, so after a submission it can report one available token while a new submission is still rate-limited.

### Expected Behavior

The getter reports zero during an active flat cooldown and one when it expires; burst-mode refill reporting remains consistent with enforcement.

### Proposed Solution

Branch on rate-limit mode and derive availability from the same effective cooldown and state used by enforcement. Clarify the never-submitted convention.

### Acceptance Criteria

- [ ] The getter reports zero during an active flat cooldown and one when it expires; burst-mode refill reporting remains consistent with enforcement.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Query before submission, immediately after, just before expiry, and at expiry in both flat and burst modes.

## Draft 35

### Title

Make interface metadata enumerate every supported capability

### Priority

Low

### Summary

Runtime capability metadata omits interfaces that direct supports_interface probes accept.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `get_interface_metadata / supports_interface`. Metadata builds a separate hardcoded capability list lacking symbols handled by supports_interface, including hpag, var, histogram, rgate, and dprv. Clients discovering features through metadata receive a different result from direct probes. The published documentation issue concerns rustdoc rather than this runtime list.

### Expected Behavior

Every metadata capability is accepted by supports_interface and every supported public capability appears once in metadata.

### Proposed Solution

Use a shared capability registry to generate both runtime discovery surfaces.

### Acceptance Criteria

- [ ] Every metadata capability is accepted by supports_interface and every supported public capability appears once in metadata.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Assert set equality between the documented registry, metadata result, and individual capability probes, including unknown symbols.

## Draft 36

### Title

Restrict reviewer approvals to existing bounded proposal targets

### Priority

Medium

### Summary

Reviewer approvals can allocate storage for arbitrary targets unrelated to an active proposal.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — `approve_proposal_review`. An authorized reviewer can supply any Symbol as target. The method writes a new approvals record without checking an active proposal or bounding the number of target keys. Repeated arbitrary targets create persistent instance-state growth unrelated to governance work.

### Expected Behavior

Unknown and completed targets cannot allocate approval state; active targets remain approvable and completed records are reclaimed.

### Proposed Solution

Resolve targets to active proposal identities and reject unknown targets before writing; bound and retire stored approvals with proposal lifecycle.

### Acceptance Criteria

- [ ] Unknown and completed targets cannot allocate approval state; active targets remain approvable and completed records are reclaimed.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Submit many unique nonexistent targets and assert storage remains unchanged; exercise proposal create, approve, execute/cancel, and cleanup.

## Draft 37

### Title

Define conservative aggregate arbitration for equal timestamps

### Priority

Medium

### Summary

Equal-timestamp aggregate arbitration depends on shard registration order and can choose the lower-risk result.

### Problem / Evidence

`contracts/scoregate-aggregator/src/lib.rs` — `get_aggregate_score`. Selection replaces the current best only when last_updated is greater. Equal-timestamp aggregates retain whichever registered shard is visited first, even if another reports higher risk. get_score already applies a higher-score tie-break for equal timestamps.

### Expected Behavior

Reordering shards with equal observation timestamps does not lower the selected aggregate risk; fresher observations still take precedence.

### Proposed Solution

Specify and implement deterministic conservative tie-breaking for aggregate observations, including ties in all primary fields.

### Acceptance Criteria

- [ ] Reordering shards with equal observation timestamps does not lower the selected aggregate risk; fresher observations still take precedence.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Register stub shards in both orders with equal timestamps and different aggregate scores; test equal scores and a fresher lower score.

## Draft 38

### Title

Reject malformed or repeated replay headers

### Priority

Medium

### Summary

Replay header detection accepts repeated headers and can mistake malformed header-like objects for data.

### Problem / Evidence

`tools/replay/src/main.rs` — `process_snapshot`. Header recognition depends on count == 0, where count increments only for data records. Multiple valid headers before the first record are accepted. A header-like object that fails ReplayFileHeader deserialization can fall through into SnapshotEntry parsing, which ignores unknown fields.

### Expected Behavior

At most one header is accepted at the start; malformed schema_version values cannot be silently treated as data; legacy headerless input remains supported.

### Proposed Solution

Track whether the first nonblank record has been consumed and distinguish explicit header objects from data records before deserializing.

### Acceptance Criteria

- [ ] At most one header is accepted at the start; malformed schema_version values cannot be silently treated as data; legacy headerless input remains supported.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test duplicate headers, headers after data, string/negative schema versions, a mixed header/data object, and a valid headerless fixture.

## Draft 39

### Title

Capture contract events rather than synthetic submission messages in replay evidence

### Priority

Medium

### Summary

Replay event hashes cover synthetic progress messages instead of the contract events needed to detect emission regressions.

### Problem / Evidence

`tools/replay/src/main.rs` — `process_snapshot / EventEvidence`. process_snapshot appends a batch_submission message for each processed input without reading Env events. The events_hash therefore authenticates generated prose rather than actual contract event topics and payloads, and cannot reveal an event emission regression.

### Expected Behavior

A contract event topic/payload change changes the event hash; an invocation emitting no event contributes no fabricated contract event.

### Proposed Solution

Capture ordered contract event deltas with contract identity, topics, and payloads; keep tool progress messages separately identified. Version the evidence format.

### Acceptance Criteria

- [ ] A contract event topic/payload change changes the event hash; an invocation emitting no event contributes no fabricated contract event.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Replay success and rejection fixtures, compare captured events with Env event output, and verify deterministic hashes across identical runs.

## Draft 40

### Title

Validate numeric trade data before deriving replay scores

### Priority

Medium

### Summary

Malformed or overflowing price data can be silently converted into an apparently valid replay score.

### Problem / Evidence

`tools/replay/src/main.rs` — `parse_price_average`. The average silently skips nonnumeric price fields, accepts negative values, and accumulates finite f64 values without checking for overflow to infinity. The caller then casts and clamps the result, converting malformed data into apparently valid risk scores.

### Expected Behavior

Malformed price records cannot silently contribute a default or clamped score; supported finite input yields the documented average.

### Proposed Solution

Define accepted price values, reject malformed or nonfinite intermediate results with record context, and use an overflow-resistant average.

### Acceptance Criteria

- [ ] Malformed price records cannot silently contribute a default or clamped score; supported finite input yields the documented average.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Test missing prices, strings, negatives, empty trades, repeated very large finite prices, and ordinary positive values; verify useful record diagnostics.

## Draft 41

### Title

Give replay input errors a path and line number

### Priority

Low

### Summary

Replay parse errors omit the source path and physical line number needed to locate a bad record.

### Problem / Evidence

`tools/replay/src/main.rs` — `process_snapshot / process_failure_scenario`. NDJSON parse failures use generic contexts parsing ndjson line and parsing failure entry. Neither loop enumerates lines for diagnostics, so an operator cannot locate a corrupt record in a large export from the error message.

### Expected Behavior

A malformed record after blank lines reports its physical line and input path; successful output remains unchanged.

### Proposed Solution

Enumerate physical lines and add source path and line number to parse, schema, and field-validation errors.

### Acceptance Criteria

- [ ] A malformed record after blank lines reports its physical line and input path; successful output remains unchanged.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Feed a temporary file with blank lines and an invalid later record; assert exact location information in the error.

## Draft 42

### Title

Register the oracle adapter example as a Cargo build target

### Priority

Low

### Summary

The oracle adapter example is outside the declared Cargo example targets, leaving its build and tests unchecked.

### Problem / Evidence

`examples/oracle_adapter.rs` and `contracts/scoregate-score/Cargo.toml` — `ExamplePriceFeedOracle / example target list`. The oracle adapter exists at the workspace root examples directory, but the virtual workspace does not build root examples and the score crate explicitly registers only three other examples. The adapter can drift without appearing in cargo build --examples.

### Expected Behavior

Cargo metadata lists the adapter target and the documented example build command compiles it.

### Proposed Solution

Register the adapter as an appropriate library example and include it in the existing example build check.

### Acceptance Criteria

- [ ] Cargo metadata lists the adapter target and the documented example build command compiles it.
- [ ] Add regression coverage for the specified failure and success cases.

### Validation / Test Plan

Run cargo metadata and, after baseline compile repairs, build the adapter and all registered examples.

## Draft 43

### Title

Enforce tuple cardinality in generated JSON schemas

### Priority

Medium

### Summary

Tuple schemas currently accept arrays that cannot represent the declared contract tuple.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `json_schema_type`, Tuple arm. The fragment supplies positional `items` but no `minItems`, `maxItems`, or `additionalItems` restriction. A two-element tuple therefore admits an empty array or extra elements under the declared draft-07 dialect.

### Expected Behavior

A tuple instance has exactly the number of elements in its XDR specification, with each position validated.

### Proposed Solution

Emit exact cardinality constraints alongside positional item schemas, including an explicit representation for the empty tuple.

### Acceptance Criteria

- [ ] Empty and oversized arrays fail for nonempty tuples.
- [ ] Exactly sized valid arrays pass. Nested tuples retain independent length checks.

### Validation / Test Plan

Generate zero-, one-, and two-element tuple fixtures and validate missing, extra, and wrong-type elements with a draft-07 validator.

## Draft 44

### Title

Preserve map key and value types across generated bindings

### Priority

Medium

### Summary

Map rendering discards information that client validation needs to preserve contract values.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — Map arms in `json_schema_type`, `ts_type`, and `py_type`. JSON and TypeScript always use string object keys regardless of `key_type`; Python always emits `Dict[str, Any]`, discarding `value_type` as well. A map with integer or composite keys cannot be faithfully represented by these declarations.

### Expected Behavior

Supported maps retain both key and value types through serialization; unsupported key encodings fail generation explicitly.

### Proposed Solution

Define one map wire representation, such as typed key/value entry arrays where object keys are insufficient, and render it consistently in all three languages. Recursively render Python value types.

### Acceptance Criteria

- [ ] Map<U32,Bool> and a map with composite keys round-trip without key coercion.
- [ ] Invalid value types are rejected. Document any representation change.

### Validation / Test Plan

Use synthetic map specs with string, integer, and tuple keys and nested values; compare JSON validation and Python/TypeScript round trips. This is separate from fixing missing typing imports.

## Draft 45

### Title

Resolve referenced user-defined types during schema generation

### Priority

Medium

### Summary

Generated files can contain names and references whose definitions are never emitted.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — Udt branches return a local `$defs` reference or a bare language type name. `struct_to_json_schema`, `struct_to_typescript`, and `struct_to_python` receive only one struct and never collect dependent definitions. The public conversion API therefore renders a nested UDT without a resolvable dependency.

### Expected Behavior

Every referenced type resolves within the generated artifact set, or generation reports the unsupported dependency.

### Proposed Solution

Build a dependency graph from the contract spec, emit/import reachable definitions, and detect missing or recursive references deliberately.

### Acceptance Criteria

- [ ] A struct containing another struct produces resolvable JSON references and importable Python/TypeScript definitions.
- [ ] Missing dependencies produce actionable errors.

### Validation / Test Plan

Generate fixtures with a nested struct, shared dependency, enum dependency, and recursive reference; validate reference resolution and compile/load emitted bindings.

## Draft 46

### Title

Enforce XDR integer ranges in runtime schema validators

### Priority

Medium

### Summary

Generated runtime validators accept integers outside the source contract field widths.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `json_schema_type` emits only a zero minimum for unsigned integers and no width limits; `py_type` maps every integer to unconstrained `int` unless a field happens to have a score-domain name. For example a U32 non-score field admits 4294967296, and Python admits negative U64 values.

### Expected Behavior

Integer fields accept exactly the representable XDR range, additionally narrowed by any semantic score constraints.

### Proposed Solution

Derive signed and unsigned width bounds from ScSpecTypeDef and apply them recursively in JSON Schema and Pydantic constraints. Preserve the existing TypeScript bigint precision policy.

### Acceptance Criteria

- [ ] Boundary values pass and values one below/above each width fail.
- [ ] Unsigned fields reject negatives.
- [ ] Score fields remain bounded to 0–100.

### Validation / Test Plan

Test U32, I32, U64, I64, U128, and U256 boundaries using arbitrary-precision validation. Keep this independent of the published TypeScript number precision fix.

## Draft 47

### Title

Align Python model handling of unknown fields with JSON Schema

### Priority

Low

### Summary

Python and JSON consumers disagree about whether an unexpected field is valid.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — `struct_to_json_schema` sets `additionalProperties: false`, while `struct_to_python` generates a plain BaseModel with no extra-field policy. Default Pydantic behavior can discard a misspelled or future field instead of rejecting it, obscuring schema drift.

### Expected Behavior

The two runtime representations apply the same documented unknown-field policy.

### Proposed Solution

Generate a Pydantic v2 configuration forbidding extras, or explicitly revise and document both formats together if permissive compatibility is intended.

### Acceptance Criteria

- [ ] A valid record passes both validators.
- [ ] Adding an unknown field yields the same rejection in both. Required and optional field behavior remains documented.

### Validation / Test Plan

Load a generated model and validate a valid record plus one with a misspelled extra field; compare against the corresponding rooted JSON schema.

## Draft 48

### Title

Validate recovery export records beyond their JSON shape

### Priority

Medium

### Summary

A well-typed JSON backup may still contain impossible scores or duplicate logical records.

### Problem / Evidence

`tools/recovery/src/main.rs` — `cmd_export` and `cmd_verify` deserialize `Vec<ExportableScoreEntry>` but do not check score/confidence/component bounds or uniqueness of `(wallet, asset_pair)`. The entry-count check can pass for two copies of one record while another record is absent.

### Expected Behavior

Export and verification reject semantically invalid records before presenting the backup as usable.

### Proposed Solution

Share record validation for score-domain bounds, valid identifiers, and duplicate logical keys. Report the offending index and key. Retain the existing count comparison.

### Acceptance Criteria

- [ ] Out-of-domain values and duplicate keys fail even when the total count matches.
- [ ] Distinct valid entries pass without alteration.

### Validation / Test Plan

Use a two-record export with a duplicated key and matching snapshot count, plus boundary values 0, 100, and 101. Confirm no output is replaced for invalid input.

## Draft 49

### Title

Compare recovery roots as canonical digest bytes

### Priority

Low

### Summary

Equivalent hexadecimal roots can be reported as different state.

### Problem / Evidence

`tools/recovery/src/main.rs` — `cmd_verify` allows both uppercase and lowercase hex through `is_ascii_hexdigit`, but `cmd_reconcile` compares the raw strings. Uppercase and lowercase encodings of the same digest therefore produce a false divergence.

### Expected Behavior

Valid encodings of the same 32-byte digest compare equal; different digest bytes remain different.

### Proposed Solution

Decode validated roots to fixed-size byte arrays before comparison and use one canonical hex encoding in reports. Do not weaken root validation.

### Acceptance Criteria

- [ ] Case-only differences yield matching roots.
- [ ] One changed nibble yields a divergence.
- [ ] Invalid encodings receive a controlled diagnostic.

### Validation / Test Plan

Compare snapshots containing lower-, upper-, and mixed-case copies of the same roots, then alter a single byte and verify only the relevant root differs.

## Draft 50

### Title

Bind recovery snapshots to their network and contract

### Priority

Medium

### Summary

Recovery files lack provenance needed to establish which deployment their state describes.

### Problem / Evidence

`tools/recovery/src/main.rs` — `StateSnapshot` stores roots, count, ledger sequence, and timestamp, but no contract ID or network identity. `cmd_reconcile` accepts two snapshots with identical roots regardless of their origin, so an operator can accidentally reconcile different deployments.

### Expected Behavior

Reconciliation identifies incompatible origins and never treats matching roots alone as proof that the intended deployment was checked.

### Proposed Solution

Add versioned network and contract identity to new snapshots, validate identity on comparison, and define an explicit legacy-file policy.

### Acceptance Criteria

- [ ] Same-origin snapshots compare normally.
- [ ] A different contract or network is reported as an origin mismatch.
- [ ] Legacy files are visibly unbound rather than silently trusted.

### Validation / Test Plan

Create identical-root fixtures for two contracts and two networks and test all combinations, including a legacy snapshot with no identity fields.

## Draft 51

### Title

Separate action time from report generation time in recovery reports

### Priority

Low

### Summary

A report generated after an incident records the current time as though it were the time of the recovery action.

### Problem / Evidence

`tools/recovery/src/main.rs` — `cmd_report` sets `action_timestamp` to `chrono_now()`, while the CLI accepts only action type and description. Operators cannot accurately record an action performed earlier.

### Expected Behavior

Reports distinguish when the action happened from when evidence was assembled.

### Proposed Solution

Accept an explicit action timestamp with format validation and add a generated-at timestamp. If action time is omitted, represent it as unknown rather than inferring it.

### Acceptance Criteria

- [ ] A supplied historical action time is preserved.
- [ ] Generated-at reflects report creation.
- [ ] Invalid timestamps fail clearly and omitted action times are unambiguous.

### Validation / Test Plan

Generate a report for a fixed past action under a controlled clock and inspect both timestamps; test malformed and omitted inputs.

## Draft 52

### Title

Keep fuzzer mutations within the operation bound

### Priority

Medium

### Summary

The fuzzer can generate invalid campaigns and mistake its own bound violation for a contract counterexample.

### Problem / Evidence

`tools/invocation-fuzzer/src/lib.rs` — `mutate`. At MAX_OPERATIONS, insertion and duplication guards fail, but the final wildcard arm still pushes a new operation. `replay_campaign` then rejects the oversized campaign before contract execution.

### Expected Behavior

Every mutation of a valid campaign remains within MAX_OPERATIONS.

### Proposed Solution

Use a replacement, deletion, or no-op fallback when the campaign is full; retain insertion only when capacity exists.

### Acceptance Criteria

- [ ] All mutation branches preserve the bound for empty, nearly full, and full parents.
- [ ] Generated campaigns do not fail solely because the mutator exceeded its own limit.

### Validation / Test Plan

Exercise deterministic seeds across every branch with a MAX_OPERATIONS parent and validate the child before replay; confirm campaigns can still grow from empty input.

## Draft 53

### Title

Preserve the failure category when shrinking fuzzer counterexamples

### Priority

Medium

### Summary

Minimization can replace a meaningful contract failure with an unrelated harness error.

### Problem / Evidence

`tools/invocation-fuzzer/src/lib.rs` — `run_fuzz` passes `replay_campaign(candidate).is_err()` to `shrink_campaign`. Any error satisfies the predicate, even if deleting or simplifying operations changes a determinism failure into input validation or another invariant failure.

### Expected Behavior

The saved minimized fixture reproduces the original failure class and relevant invariant.

### Proposed Solution

Introduce a structured failure fingerprint and require candidate shrink steps to preserve it; include the original and minimized fingerprints in diagnostics.

### Acceptance Criteria

- [ ] A candidate that fails for a different reason is not accepted.
- [ ] The final saved fixture reproduces the initial fingerprint on repeated replay.

### Validation / Test Plan

Test a shrink predicate with two distinguishable failures and verify irrelevant operations are removed while the original invariant remains violated.

## Draft 54

### Title

Handle zero denominators in WASM attribution reports

### Priority

Low

### Summary

Empty baselines and zero-size entries can generate nonfinite percentages in serializable reports.

### Problem / Evidence

`tools/replay/src/wasm_analysis.rs` — `add_module` and `add_feature` divide by `total_size`; `compare_binaries` divides module growth by the previous module size without a zero guard. Zero-sized inputs can therefore produce NaN or infinity instead of usable numeric evidence.

### Expected Behavior

Reports have an explicit, JSON-safe representation for percentages that cannot be computed from a zero baseline.

### Proposed Solution

Define zero-baseline semantics, using an optional percentage or an explicit new-allocation state, and apply them consistently to attribution and comparison.

### Acceptance Criteria

- [ ] Zero-to-zero and zero-to-positive cases serialize without nonfinite numbers.
- [ ] Ordinary nonzero percentages are unchanged.

### Validation / Test Plan

Add focused unit tests for zero total size, zero prior module size, and normal growth; wire the module into the library test target before executing them.

## Draft 55

### Title

Include newly introduced modules in WASM growth diagnostics

### Priority

Low

### Summary

Growth reports can omit the component responsible for a binary increase.

### Problem / Evidence

`tools/replay/src/wasm_analysis.rs` — `compare_binaries` adds regressions only inside `if let Some(prev_size) = module_map.get(...)`. A module appearing for the first time is absent from the regressions list, even when its bytes are material.

### Expected Behavior

Newly introduced modules appear in growth diagnostics with their full added size.

### Proposed Solution

Compare the union of module names and explicitly classify added and removed modules. Define review handling for additions without inventing an infinite percentage.

### Acceptance Criteria

- [ ] A newly added module is reported with zero previous bytes.
- [ ] Unchanged modules are omitted.
- [ ] Removal is not classified as growth.

### Validation / Test Plan

Compare a baseline containing A with a current artifact containing unchanged A and new B, then reverse the comparison and inspect attribution.

## Draft 56

### Title

Validate qualified symbol ownership in the refinement checker

### Priority

Medium

### Summary

The refinement checker can approve a reference to the wrong enum, module, or struct.

### Problem / Evidence

`tools/check_refinement_mapping.py` — `build_rust_index` records a global name-to-role set; `extract_candidates` discards enum/field owners, and `resolve` accepts any globally present symbol without enforcing its role. A real field name attached to the wrong struct can pass.

### Expected Behavior

A qualified reference resolves to the named owner and the expected symbol kind.

### Proposed Solution

Index qualified declarations and resolve owner/member pairs together. Restrict function, constant, field, and variant checks to their recorded roles.

### Acceptance Criteria

- [ ] A valid qualified reference passes.
- [ ] Moving its member to a wrong existing owner fails even when both names exist elsewhere.

### Validation / Test Plan

Create mapping fixtures with a real field under the wrong struct, a variant under the wrong enum, and a constant used as a function; assert all are rejected.

## Draft 57

### Title

Count actual tuple elements in event arity checks

### Priority

Medium

### Summary

Legal four-topic events can be rejected because formatting adds a trailing comma.

### Problem / Evidence

`tools/check_event_schema.sh` — embedded Python topic parser counts top-level commas and then adds one whenever any content exists. A four-element tuple ending in a comma is counted as five; the same parser ignores variable-bound topic arguments entirely.

### Expected Behavior

Arity validation counts real topic expressions and reports unsupported forms instead of silently skipping them.

### Proposed Solution

Parse tuple elements with trailing separators handled correctly and resolve supported local topic bindings, or use Rust syntax parsing with explicit diagnostics for unsupported expressions.

### Acceptance Criteria

- [ ] Four topics pass with or without a trailing comma.
- [ ] Five topics fail in direct and locally bound tuples.
- [ ] Strings/comments do not change the count.

### Validation / Test Plan

Extend `tests/check_event_schema.test.sh` with equivalent formatting variants and a five-topic local variable. This fixes arity analysis rather than expanding the already-published contract-file coverage.

## Draft 58

### Title

Upload production acceptance evidence when CI checks fail

### Priority

Medium

### Summary

The CI job loses the report precisely when it is needed to diagnose a failed readiness run.

### Problem / Evidence

`.github/workflows/ci.yml` — `production-acceptance` runs the script and then uploads the report without an `if: always()` condition. `scripts/production-acceptance.sh` deliberately writes a failure report and exits nonzero, causing the subsequent upload step to be skipped.

### Expected Behavior

A failed acceptance run retains its report and associated step logs while the job remains failed.

### Proposed Solution

Run evidence upload on failure as well as success and include the generated log directory with the report. Use explicit handling when no report was created.

### Acceptance Criteria

- [ ] A deliberately failing check yields a failed job and a downloadable report with all available referenced logs.
- [ ] Success retains the same evidence.

### Validation / Test Plan

Inspect workflow conditions and exercise the job in a local workflow harness with a failing command and a generated report; no remote workflow dispatch is required.

## Draft 59

### Title

Run schema drift verification in pull request CI

### Priority

Medium

### Summary

The schema generator has a check mode, but the repository does not automatically enforce it for source changes.

### Problem / Evidence

`.github/workflows/ci.yml` contains build, test, policy, and formal-model jobs but no invocation of `schema-gen --check`. `tools/schema-gen/src/main.rs` implements that command, while `schemas/` contains committed client artifacts. Source-only edits can therefore merge without detecting stale generated bindings.

### Expected Behavior

PR validation fails when committed schema artifacts differ from generator output.

### Proposed Solution

Add a locked schema verification job after making check mode read-only, and document the regeneration command. Check all supported output artifacts.

### Acceptance Criteria

- [ ] Changing a contract field without regenerating artifacts fails CI.
- [ ] Regeneration restores the check.
- [ ] Verification does not modify tracked files.

### Validation / Test Plan

Use a temporary checkout to alter a source spec or generated artifact, run the job command, and inspect exit status and git diff. This adds enforcement, separate from fixing the CLI write behavior.

## Draft 60

### Title

Provide authentic release provenance instead of calling a checksum a signature

### Priority

Medium

### Summary

The release pipeline labels an integrity checksum as a signature, although it provides no identity authentication.

### Problem / Evidence

`.github/workflows/release.yml` — the sign step only runs `sha256sum`; `.github/workflows/ci.yml` uses the same wording. Neither invokes a signing key or creates an attestation. A replaced artifact and replaced checksum remain mutually consistent.

### Expected Behavior

Release consumers can verify authenticated build provenance, and documentation accurately distinguishes checksums from signatures.

### Proposed Solution

Add a verifiable provenance attestation or detached signature tied to the release artifact and repository identity; retain SHA-256 for integrity and correct the current terminology.

### Acceptance Criteria

- [ ] The release includes verifiable provenance tied to its artifact digest.
- [ ] Verification rejects a substituted artifact.
- [ ] Instructions identify the trusted issuer or key.

### Validation / Test Plan

Validate the signing/attestation workflow against a local test artifact and a tampered copy, without publishing a release. Review permissions required by the selected mechanism.

## Draft 61

### Title

Bind optimized release artifacts to the reproducibility result

### Priority

Medium

### Summary

The published optimized binary is not compared with the raw binary checked by the reproducibility job.

### Problem / Evidence

`.github/workflows/release.yml` — `build-and-sign` independently builds and optimizes a raw WASM. `reproducibility-check` compares two other raw builds, and `publish-release` only prints their verified hash alongside the optimized artifact. No comparison binds the optimizer input to that verified hash.

### Expected Behavior

The exact raw input used for the deployable optimized artifact matches the reproducibility result.

### Proposed Solution

Pass the raw artifact digest from build-and-sign into the comparison, or optimize the verified artifact downstream. Verify the downloaded publish artifact against its manifest before release creation.

### Acceptance Criteria

- [ ] A differing raw optimizer input blocks publication even if the two reproducibility samples agree.
- [ ] The final downloaded optimized artifact passes a digest check.

### Validation / Test Plan

Model the job artifact flow with small fixture files; substitute the optimizer input and then the downloaded optimized output and assert both mismatches block the final publication command.

## Draft 62

### Title

Make release checksum manifests portable after download

### Priority

Low

### Summary

The checksum sidecar references a build-directory path that does not exist beside downloaded release files.

### Problem / Evidence

`.github/workflows/release.yml` — the manifest is generated by `sha256sum "$OPT_WASM"`, where OPT_WASM includes `target/wasm32-unknown-unknown/release/`. The published artifact is downloaded as a bare filename, so a standard checksum verification from the download directory cannot resolve the recorded path.

### Expected Behavior

Downloading the WASM and sidecar into one directory is sufficient to run `sha256sum --check`.

### Proposed Solution

Generate the release manifest from the artifact directory using a basename and document verification from that directory.

### Acceptance Criteria

- [ ] The sidecar contains the release filename without repository build paths.
- [ ] Verification succeeds after download and fails after a one-byte mutation.

### Validation / Test Plan

Copy a fixture WASM and generated manifest into a fresh temporary directory and run checksum verification before and after modifying the fixture.

## Draft 63

### Title

Pass release notes as data instead of interpolating them into shell source

### Priority

Medium

### Summary

Changelog and commit text can break or execute within the release shell script.

### Problem / Evidence

`.github/workflows/release.yml` — `NOTES="${{ steps.release-notes.outputs.notes }}"` inserts an expression directly into shell source. The preceding sed escape handles quotes/newlines but leaves shell substitutions such as dollar-parentheses and backticks active. It also converts real newlines into literal escape text.

### Expected Behavior

Release prose is preserved literally and never interpreted as shell syntax.

### Proposed Solution

Write notes to a file and carry that file between steps, or use a structured environment variable with safe output transport. Pass the final body through `--notes-file` without source interpolation.

### Acceptance Criteria

- [ ] Backticks, dollar signs, quotes, and multiple paragraphs survive unchanged.
- [ ] Embedded command-looking text has no side effects.

### Validation / Test Plan

Run the note assembly commands locally with sentinel command-substitution text and assert no sentinel file is created and the body matches the input bytes.

## Draft 64

### Title

Attach the generated dependency inventory to releases

### Priority

Low

### Summary

Release consumers cannot retrieve the SBOM through the release assets even though CI already generates one.

### Problem / Evidence

`.github/workflows/release.yml` ends with a commented SBOM placeholder, while `.github/workflows/ci.yml` calls `tools/generate_sbom.sh` and uploads its output as a separate CI artifact. Tag publication attaches only WASM and a checksum.

### Expected Behavior

Each release carries a dependency inventory generated from the same tagged source and lockfile as its binary.

### Proposed Solution

Integrate the existing generator into the tag workflow, validate its output, and attach it with the release assets and provenance.

### Acceptance Criteria

- [ ] A release preparation run produces a valid SBOM from the tag.
- [ ] Missing or failed generation prevents claiming a complete release inventory.
- [ ] The asset list includes the SBOM.

### Validation / Test Plan

Inspect a local release staging directory and verify the SBOM package graph and lockfile provenance; use a stub gh command to assert the upload arguments without remote writes.

## Draft 65

### Title

Generate release download instructions for the actual repository

### Priority

Low

### Summary

Generated verification instructions point at another repository name.

### Problem / Evidence

`.github/workflows/release.yml` — the release-body heredoc hardcodes `https://github.com/Ledger-Lenz/scoregate-contract/releases/download/`. This checkout is hartz0/scoregate-contracts, so its generated instructions do not point at the release being created.

### Expected Behavior

Verification commands reference the repository and tag of the current release run.

### Proposed Solution

Build release URLs from the workflow server and repository context, with shell-safe transport, and remove hardcoded repository identity from the generated body.

### Acceptance Criteria

- [ ] The generated URL contains the current repository and tag.
- [ ] A fork produces its own URL.
- [ ] Artifact filenames match attached assets.

### Validation / Test Plan

Render the body locally for hartz0/scoregate-contracts and a second fixture repository and verify the resulting URL components.

## Draft 66

### Title

Lock dependency resolution in the deployment build

### Priority

Medium

### Summary

Deployment can resolve a different dependency graph from the reviewed lockfile.

### Problem / Evidence

`deploy.sh` — the build command invokes `cargo build --target wasm32-unknown-unknown --release -p scoregate-score` without `--locked`, whereas the release workflow and canary deployment use locked builds. A stale lockfile can be rewritten during a deployment build.

### Expected Behavior

Deployment builds fail on lockfile drift before optimization or transaction submission.

### Proposed Solution

Use `--locked` for the deployment build and provide a clear diagnostic directing dependency changes back through review.

### Acceptance Criteria

- [ ] The printed and executed build command is locked.
- [ ] A manifest/lockfile mismatch aborts before any deploy invocation and leaves Cargo.lock unchanged.

### Validation / Test Plan

Check dry-run output and use stub cargo/CLI binaries to simulate lockfile rejection; assert no optimizer or network mutation command is called afterward.

## Draft 67

### Title

Resolve deployment identities before creating the contract

### Priority

Medium

### Summary

An invalid admin identity is discovered only after deployment, and failure is replaced by a literal placeholder.

### Problem / Evidence

`deploy.sh` — `keys address` runs after `contract deploy` and falls back to `<ADMIN_ADDRESS>` on failure. Initialization then attempts to use that placeholder. The service address is checked only for nonemptiness before the deployment sequence.

### Expected Behavior

Invalid local signing identity or service address prevents deployment before any transaction is submitted.

### Proposed Solution

Resolve and validate the administrator and service inputs during preflight; remove the real-run placeholder fallback. Keep placeholders limited to printed dry-run plans.

### Acceptance Criteria

- [ ] Identity resolution failure stops before build/deploy mutation.
- [ ] Malformed service addresses are rejected.
- [ ] Valid inputs are reused consistently for initialization and verification.

### Validation / Test Plan

Use CLI stubs recording calls for missing identity, malformed service address, and success; verify that failing preflight never invokes contract deploy.

## Draft 68

### Title

Compare deployed configuration with intended values before reporting success

### Priority

Medium

### Summary

A successful read is currently treated as successful deployment verification even if it returns the wrong administrator.

### Problem / Evidence

`deploy.sh` — the verification block obtains STORED_ADMIN and CONTRACT_VERSION and logs them, but never compares the admin with ADMIN_ADDRESS or the version with an expected value. It does not read back the configured service address.

### Expected Behavior

Deployment succeeds only after parsed on-chain administrator, service, and version match the intended configuration.

### Proposed Solution

Parse the CLI response format explicitly, compare each required field, and return a failure containing the contract ID and mismatched field.

### Acceptance Criteria

- [ ] Wrong admin, wrong service, malformed response, or unexpected version fails verification.
- [ ] Exact matches reach the completion summary.

### Validation / Test Plan

Extend deployment CLI stubs to return valid-but-wrong values and correctly encoded matches; assert the exit status and that mismatches never print deployment complete.

## Draft 69

### Title

Anchor deployment build paths to the repository root

### Priority

Low

### Summary

Invoking deployment scripts by absolute path from another directory changes where Cargo and artifact lookup operate.

### Problem / Evidence

`deploy.sh` computes SCRIPT_DIR for manifests but leaves WASM paths relative and does not change working directory. `scripts/canary-deploy.sh` uses absolute artifact paths yet also invokes Cargo in the caller directory. Outside the checkout these commands fail or build a different workspace.

### Expected Behavior

The scripts build the intended repository regardless of the caller working directory.

### Proposed Solution

Change into the resolved repository root before Cargo/artifact operations or pass explicit manifest and target paths consistently.

### Acceptance Criteria

- [ ] Invocation from the repository, a subdirectory, and an unrelated temporary directory selects the same Cargo manifest and WASM output.

### Validation / Test Plan

Run dry/stubbed deployments from all three directories and inspect captured command working directories and paths, without network calls.

## Draft 70

### Title

Make canary dry runs fully offline and non-mutating

### Priority

Medium

### Summary

Canary dry-run mode still depends on built artifacts and invokes live verification commands.

### Problem / Evidence

`scripts/canary-deploy.sh` skips the build through `run`, but executes sha256sum on the optimized WASM unconditionally, writes the contract ID file, and calls get_admin, get_version, submit_score, and get_score directly through soroban. A clean offline dry run therefore fails or reaches real RPC calls.

### Expected Behavior

Dry run prints the complete plan without requiring a WASM, sending RPC requests, or replacing saved canary identity.

### Proposed Solution

Route every external action through an explicit dry-run branch and use in-memory placeholders for dependent values. Keep durable report/identity writes out of dry run.

### Acceptance Criteria

- [ ] With no CLI or target artifacts, dry run completes and prints verification commands.
- [ ] An existing canary ID file remains byte-identical.
- [ ] No RPC subprocess runs.

### Validation / Test Plan

Run in a temporary clean copy with a CLI sentinel that fails if executed, then compare filesystem state before and after.

## Draft 71

### Title

Require a successful score round trip before declaring canary success

### Priority

Medium

### Summary

The canary deployment can finish successfully after its core submission and retrieval checks fail.

### Problem / Evidence

`scripts/canary-deploy.sh` converts submit failure to CANARY_SUBMIT_FAILED, logs a warning, converts get_score failure to SCORE_NOT_FOUND, and still prints the completion summary. Submission also uses the admin identity rather than accepting a dedicated service signing identity.

### Expected Behavior

A canary verdict distinguishes deployment-only success from a verified submit/read round trip, and required round-trip failures produce nonzero status.

### Proposed Solution

Accept the appropriate service identity for the smoke write, require successful submission and parsed score comparison, and make intentionally skipped checks explicit rather than successful.

### Acceptance Criteria

- [ ] Failed submission, missing score, or wrong returned score blocks a successful canary verdict.
- [ ] A valid authenticated round trip succeeds.

### Validation / Test Plan

Use a stub CLI for submission rejection, retrieval failure, wrong score, and success; assert status and report wording in each case.

## Draft 72

### Title

Restore the original pause state after operational rehearsal

### Priority

Medium

### Summary

The rehearsal always unpauses the contract, even when it started paused, and has no interrupt cleanup for a newly applied pause.

### Problem / Evidence

`scripts/testnet-canary-rehearsal.sh` invokes pause followed by unpause without reading the original is_paused value or installing a state-restoration trap. A rehearsal on an already paused deployment can unintentionally enable submissions; interruption can leave a previously active deployment paused.

### Expected Behavior

Reversible drills preserve the original operational state and report any failed restoration.

### Proposed Solution

Capture the initial pause state, track successful mutations, and restore only changes made by the drill on normal and interrupted exit. Report restoration failure prominently.

### Acceptance Criteria

- [ ] Initially paused deployments remain paused.
- [ ] Initially active deployments are restored after success and interruption.
- [ ] Restoration failures return nonzero.

### Validation / Test Plan

Use a stateful local CLI stub and interrupt between pause and unpause; test both initial states and a failed restoration command.

## Draft 73

### Title

Compare baseline and final state during canary reconciliation

### Priority

Medium

### Summary

The rehearsal writes hashes of logs without checking that the underlying configuration was restored.

### Problem / Evidence

`scripts/testnet-canary-rehearsal.sh` reads admin and service at baseline, reads only service at reconciliation, then hashes the three log files. There is no equality comparison and no final admin query, so changed configuration can still accompany a completed report.

### Expected Behavior

Reconciliation verifies the chosen baseline fields and reports a mismatch as a failed drill.

### Proposed Solution

Read the same fields before and after, parse values independently of CLI log noise, compare them, and retain digests as evidence rather than as the decision itself.

### Acceptance Criteria

- [ ] A changed admin or service fails the final result.
- [ ] Equal parsed values pass despite harmless log formatting changes.
- [ ] Missing observations fail explicitly.

### Validation / Test Plan

Feed stateful CLI responses with changed admin, changed service, equal state, and malformed output; verify report status and retained before/after values.

## Draft 74

### Title

Reject incomplete reconciliation records instead of inventing values

### Priority

Medium

### Summary

Reconciliation can silently skip malformed identities or compare fabricated default score data.

### Problem / Evidence

`scripts/reconcile.sh` defaults missing pipeline score to 50 and confidence/timestamp to zero, skips records lacking wallet or pair, and defaults missing on-chain fields to zero. A malformed but parseable object can therefore become a normal discrepancy or disappear from the report.

### Expected Behavior

Every input record and successful on-chain response meets an explicit schema before comparison.

### Proposed Solution

Validate required fields, numeric domains, and CLI numeric options up front; report path/line or query context for malformed data rather than applying defaults.

### Acceptance Criteria

- [ ] Missing identity/score fields and nonnumeric values fail with location context.
- [ ] Valid zero values are preserved.
- [ ] No record is silently omitted.

### Validation / Test Plan

Run against local NDJSON fixtures and a stub CLI returning empty objects, nulls, strings, and valid complete records; assert no success report for invalid data.

## Draft 75

### Title

Reject duplicate logical keys in reconciliation input

### Priority

Medium

### Summary

Repeated pipeline records inflate counts and can produce conflicting decisions for one score.

### Problem / Evidence

`scripts/reconcile.sh` builds PIPELINE_KEYS and per-key temporary files, but the comparison loop rereads every original line and never checks whether a key was already processed. Both identical and conflicting duplicates become independent report entries.

### Expected Behavior

Each wallet/pair has one unambiguous pipeline observation for a reconciliation run.

### Proposed Solution

Reject duplicates with both source locations, or define and document a deterministic latest-observation policy before issuing queries. Use the resulting unique index for comparison.

### Acceptance Criteria

- [ ] Duplicates cannot inflate total_entries.
- [ ] Conflicting observations are never silently chosen.
- [ ] Valid distinct keys each trigger one query.

### Validation / Test Plan

Provide identical and conflicting duplicate records in both orders and inspect query counts, diagnostics, and report cardinality.

## Draft 76

### Title

Process the final reconciliation record without requiring a newline

### Priority

Low

### Summary

A valid last NDJSON record is omitted when its file has no trailing newline.

### Problem / Evidence

`scripts/reconcile.sh` uses `while IFS= read -r line; do` in both input passes. Bash read returns failure at EOF when it has collected an unterminated final line, so neither loop processes that record.

### Expected Behavior

Files containing the same records produce the same comparison whether or not the final line has a newline.

### Proposed Solution

Use an EOF-safe read condition in both loops, preserving blank-line handling and malformed-record diagnostics.

### Acceptance Criteria

- [ ] One-record and multi-record files without final newlines retain their last record.
- [ ] Newline-terminated equivalents produce equal entries and counts.

### Validation / Test Plan

Run pairs of byte-identical fixtures differing only by the last newline against a deterministic CLI stub and compare reports after normalizing generated_at.

## Draft 77

### Title

Build reconciliation reports without repeatedly copying the whole array

### Priority

Low

### Summary

Large reconciliations spend growing local CPU and memory on report assembly.

### Problem / Evidence

`scripts/reconcile.sh` initializes ENTRIES_JSON to an array and invokes jq with `. + [$e]` for every record. Each iteration reparses and copies all prior entries, giving quadratic serialization work and eventually large command arguments.

### Expected Behavior

Report assembly scales approximately linearly with the number of input records.

### Proposed Solution

Spool individual validated entries to a temporary NDJSON file and assemble the final report once, or use a streaming implementation with bounded intermediate memory.

### Acceptance Criteria

- [ ] Output semantics and order remain stable.
- [ ] No per-record subprocess receives the accumulated report.
- [ ] Large fixtures complete within a documented local resource budget.

### Validation / Test Plan

Use a zero-latency CLI stub with 100, 1000, and 5000 unique records, compare resulting JSON, and measure assembly time and peak memory.

## Draft 78

### Title

Exclude stale WASM files from production acceptance evidence

### Priority

Medium

### Summary

A failed release build can still contribute an old binary hash to the current readiness report.

### Problem / Evidence

`scripts/production-acceptance.sh` continues after run_step failures and records WASM evidence whenever the fixed target path exists. It does not tie that file to the successful build step or clear/isolate old output. The overall status fails, but the artifact section can misleadingly describe an earlier build.

### Expected Behavior

Artifact evidence is included only for a successfully produced artifact from the current acceptance run.

### Proposed Solution

Build into an isolated run directory or track successful output provenance and mark artifacts unavailable after a failed build. Record the source revision and dirty-tree status with the artifact.

### Acceptance Criteria

- [ ] A preexisting WASM plus a failed build produces no current-artifact hash claim.
- [ ] A successful fresh build records the correct digest and provenance.

### Validation / Test Plan

Use a fake cargo command and a sentinel old WASM to simulate build failure, then successful replacement; inspect the artifact section in both reports.

## Draft 79

### Title

Honor explicit WASM paths in the size-report command

### Priority

Low

### Summary

An explicit missing input path triggers a build that cannot create that requested file.

### Problem / Evidence

`scripts/wasm-size-report.sh` accepts `--wasm`, but for every missing path runs the default scoregate-score build. A typo or external artifact path causes unnecessary compilation and still leaves the requested input absent.

### Expected Behavior

An explicit nonexistent input fails immediately with its path; only the documented default may trigger an automatic build.

### Proposed Solution

Track whether --wasm was supplied, validate explicit input first, and verify the default build actually created its expected output before analysis.

### Acceptance Criteria

- [ ] An invalid explicit path never invokes Cargo.
- [ ] Default missing output may build once.
- [ ] An existing custom file is analyzed directly.

### Validation / Test Plan

Use Cargo and twiggy stubs to record calls for missing explicit, existing explicit, and missing default paths.

## Draft 80

### Title

Collect SBOM outputs from a bounded generation location

### Priority

Medium

### Summary

SBOM collection can include stale or unrelated dependency inventories from the checkout.

### Problem / Evidence

`tools/generate_sbom.sh` searches the entire repository for `*.cdx.json` outside target after generation, then copies files by basename into target/sbom. Old files can satisfy the expected filename check, and colliding basenames can overwrite each other.

### Expected Behavior

Collected SBOMs are precisely the outputs of the current invocation for known workspace packages.

### Proposed Solution

Generate into a clean staging location or enumerate expected package output paths from Cargo metadata; reject collisions and missing fresh outputs.

### Acceptance Criteria

- [ ] A stale expected-name file cannot make failed generation appear complete.
- [ ] Unrelated SBOMs are excluded.
- [ ] Each workspace output has a unique destination.

### Validation / Test Plan

Stub the generator in a temporary checkout containing stale and duplicate-basename SBOMs and verify only fresh expected outputs are collected.

## Draft 81

### Title

Register documentation synchronization tests with Cargo

### Priority

Low

### Summary

The existing documentation drift tests are outside any active Cargo test target.

### Problem / Evidence

`Cargo.toml` is a virtual workspace with no root package. `tests/doc_sync_check.rs` sits under the workspace root and is not declared by a member manifest, so normal workspace tests do not discover its version and documentation checks.

### Expected Behavior

The documentation checks execute in the standard test or CI path and resolve repository paths reliably.

### Proposed Solution

Move or explicitly register the test in a suitable member crate, or expose it as a standalone CI check. Resolve file paths relative to the repository rather than an assumed process directory.

### Acceptance Criteria

- [ ] Test listing includes the drift checks.
- [ ] Changing a documented contract version makes the check fail.
- [ ] Normal source/document agreement passes.

### Validation / Test Plan

Use cargo metadata and test listing to confirm discovery, then run a temporary mismatch fixture and restore it.

## Draft 82

### Title

Keep replacement governance proposals executable in the formal model

### Priority

Medium

### Summary

The model marks the new proposal as already replaced, preventing the intended replacement lifecycle from being explored.

### Problem / Evidence

`spec/ScoreGate.tla` — `ReplaceGov` assigns both gov_proposal_id and gov_replaced_by to new_id. `GovProposalOpen` requires gov_replaced_by = 0, so the new proposal is immediately closed and ExecuteGov cannot act on it after its delay.

### Expected Behavior

The superseded proposal is permanently ineligible while its replacement can become executable after its own timelock.

### Proposed Solution

Represent old-proposal terminal state separately from the active proposal, reset replacement status for the new identity, and retain a history sufficient to state the old-proposal invariant.

### Acceptance Criteria

- [ ] A trace can replace a proposal and execute the replacement after the delay.
- [ ] The old identity never executes.
- [ ] Early replacement execution is rejected.

### Validation / Test Plan

Add a bounded TLC reachability witness for successful replacement execution and run existing veto, expiry, and no-early-execution properties.

## Draft 83

### Title

Model observable gate decisions in the embargo safety property

### Priority

Medium

### Summary

The formal embargo property does not currently constrain a gate decision.

### Problem / Evidence

`spec/ScoreGate.tla` — `EmbargoGateSoundness` compares EmbargoActive with another expression over embargo_expiry. For the modeled expiry domain the expressions restate the same condition; neither references a gate output. `spec/ScoreGate.cfg` nevertheless lists it as an invariant, so a gate that ignores embargoes cannot be detected by that check.

### Expected Behavior

The model proves that an active embargo forces the documented rejection decision, including expiry boundaries.

### Proposed Solution

Add a gate predicate or query observation tied to modeled state and assert embargo implies rejection. Keep expiry validity as a separate type/state constraint.

### Acceptance Criteria

- [ ] A deliberately mutated gate that ignores embargoes yields a TLC counterexample.
- [ ] Indefinite, active timed, expired, and lifted embargoes exercise distinct cases.

### Validation / Test Plan

Run the bounded model normally and with the embargo guard removed from the modeled gate; inspect the counterexample to ensure the property is not vacuous.

## Draft 84

### Title

Check upgrade approval snapshot safety in the formal model

### Priority

Medium

### Summary

Upgrade approval state is explored without any configured property checking its safety.

### Problem / Evidence

`spec/ScoreGate.tla` declares upg_approvals, upg_signer_snap, and upg_live_signers and includes AddUpgradeApproval, MutateAdminSet, and ClearUpgradeApprovals in Next. `spec/ScoreGate.cfg` lists no upgrade-approval invariant or property, leaving signer-set binding unverified despite the added state space.

### Expected Behavior

Model checking detects approval retention across incompatible signer-set changes and approvals outside the captured signer set.

### Proposed Solution

Add approval subset, snapshot consistency, and reset-after-mutation properties, register them in the TLC configuration, and explain their refinement to Rust behavior.

### Acceptance Criteria

- [ ] The normal model satisfies the properties.
- [ ] Removing approval clearing from MutateAdminSet produces a counterexample.
- [ ] Empty approval state is handled explicitly.

### Validation / Test Plan

Run TLC on the existing small signer domain and a mutation that retains old approvals; record state counts and the expected failing trace.

## Draft 85

### Title

Compile and test the replay analysis modules through the library

### Priority

Medium

### Summary

Analysis source files and their unit tests are disconnected from the crate module graph.

### Problem / Evidence

`tools/replay/src/lib.rs` declares configuration comparison helpers but no determinism or wasm_analysis module; `tools/replay/src/main.rs` declares schema only. Consequently `tools/replay/src/determinism.rs` and `tools/replay/src/wasm_analysis.rs` are not compiled by normal replay tests. The latter also contains orphaned statements after test_static_memory_offset and a severity comparison without ordering traits.

### Expected Behavior

The analysis APIs and tests participate in ordinary crate builds, exposing source errors and regressions.

### Proposed Solution

Register the modules, repair the revealed syntax/trait errors, and add a test-list check for representative analysis tests.

### Acceptance Criteria

- [ ] Cargo test listing includes determinism and WASM analysis tests.
- [ ] Both modules compile.
- [ ] Malformed source in either file fails the standard build.

### Validation / Test Plan

Inspect the module graph now; after baseline contract blockers are fixed, run `cargo test -p replay --lib` and verify representative tests execute. Algorithm-specific corrections remain separate.

## Draft 86

### Title

Expose the documented configuration drift command in the replay CLI

### Priority

Medium

### Summary

The documented operator command has a library implementation but no CLI dispatch.

### Problem / Evidence

`docs/config-drift.md` instructs operators to run `config-drift approved.json observed.json`. `tools/replay/src/lib.rs` provides compare_config_manifests, but the main function in `tools/replay/src/main.rs` handles replay and failure-inject behavior without dispatching config-drift. The documented invocation cannot produce the promised drift report.

### Expected Behavior

The documented command loads the two manifests, emits the deterministic report, and exits according to the documented drift policy.

### Proposed Solution

Add explicit subcommand parsing and connect the existing comparison library; provide help and reject missing or extra arguments.

### Acceptance Criteria

- [ ] The documented invocation compares the supplied paths.
- [ ] Malformed JSON fails with path context.
- [ ] An unknown subcommand is not silently treated as a replay path.

### Validation / Test Plan

Use temporary matching and differing manifest files, missing files, malformed JSON, and extra arguments in CLI tests; assert output and exit status.

## Draft 87

### Title

Reject incomplete configuration manifests before declaring no drift

### Priority

Medium

### Summary

Two empty or identically incomplete manifests can be reported as a successful configuration match.

### Problem / Evidence

`tools/replay/src/lib.rs` — compare_config_manifests treats `(None, None)` as no difference for every CONFIG_DRIFT_MANIFEST_FIELDS member; parse_manifest_json only requires an object. Thus `{}` compared with `{}` yields status ok without checking any approved configuration.

### Expected Behavior

A no-drift result requires complete, valid observations for every mandatory configuration field.

### Proposed Solution

Validate completeness and field types before comparison, or introduce an explicit partial-comparison mode whose result cannot be mistaken for full verification.

### Acceptance Criteria

- [ ] Empty objects and matching incomplete objects do not produce full-verification success.
- [ ] Complete matching objects pass.
- [ ] Null template values are not accepted as observed configuration.

### Validation / Test Plan

Test empty, missing-field, wrong-type, null-template, complete equal, and complete differing manifests directly through the library and CLI.

## Draft 88

### Title

Make error coverage checks verify executable per-variant tests

### Priority

Medium

### Summary

The build-time coverage message can claim complete coverage based solely on matching text counts.

### Problem / Evidence

`contracts/scoregate-score/build.rs` counts enum lines and functions prefixed test_error_ in `contracts/scoregate-score/src/error_coverage.rs`, then prints a checkmark when totals match. `contracts/scoregate-score/src/lib.rs` does not declare error_coverage as a test module. Equal counts do not establish unique variant coverage or test execution.

### Expected Behavior

The guard verifies one intentional assertion per supported error variant in a compiled test target.

### Proposed Solution

Wire the coverage module into tests, repair stale calls, and compare explicit covered variant identities rather than raw counts. Keep the build script lightweight and avoid claiming tests ran during a build.

### Acceptance Criteria

- [ ] Replacing one variant assertion with a duplicate cannot preserve coverage success.
- [ ] Test listing includes the suite.
- [ ] Each variant mapping is checked.

### Validation / Test Plan

Inspect discovery through Cargo metadata/test listing after build repair; temporarily duplicate a covered variant and add an uncovered variant to confirm the guard fails.

## Draft 89

### Title

Configure Criterion harnesses for every benchmark suite

### Priority

Low

### Summary

Several Criterion benchmarks are auto-discovered with Cargo’s default test harness instead of their Criterion entry point.

### Problem / Evidence

`contracts/scoregate-score/Cargo.toml` declares harness=false for twelve benches but omits entry_point_budgets, get_score_histogram, get_interpolated_score, and query_risk_gate_relative. Their corresponding files under `contracts/scoregate-score/benches/` use criterion_main!, requiring the custom harness configuration.

### Expected Behavior

Each documented benchmark command executes its Criterion benchmark functions.

### Proposed Solution

Add explicit bench entries with harness=false for the four suites and keep the benchmark inventory aligned with source files.

### Acceptance Criteria

- [ ] All four suites explicitly disable the default Cargo test harness.
- [ ] Invoking each suite lists/runs its named Criterion groups rather than reporting an empty libtest suite.

### Validation / Test Plan

Compare manifest declarations with every criterion_main source, then run the four bench targets with a minimal measurement profile once compilation is restored.

## Draft 90

### Title

Measure the enabled noise path in the private aggregate benchmark

### Priority

Low

### Summary

The private-aggregate benchmark claims to measure noise computation but only exercises its disabled branch.

### Problem / Evidence

`contracts/scoregate-score/benches/get_private_aggregate_score.rs` initializes the contract and submits pairs without configuring epsilon. `contracts/scoregate-score/src/storage.rs` — get_dp_epsilon defaults to zero; `contracts/scoregate-score/src/lib.rs` computes noise only when epsilon_bps > 0. The timed closure also recreates all fixture state on every iteration.

### Expected Behavior

The benchmark separately measures aggregate queries with noise disabled and enabled, with setup cost clearly excluded or separately named.

### Proposed Solution

Prepare explicit epsilon configurations outside the measured query using Criterion batching, and label the compared paths accurately.

### Acceptance Criteria

- [ ] Both noise branches are exercised.
- [ ] Each measured query starts from equivalent state.
- [ ] Reported query timing excludes contract registration and score submission.

### Validation / Test Plan

Add setup assertions for epsilon and pair count, run both benchmark cases, and inspect budget/timing deltas against a separately measured setup baseline.

## Draft 91

### Title

Populate model statistics summary fields on each accepted submission

### Priority

Medium

### Summary

The model statistics API exposes zero summaries even after accumulating observations.

### Problem / Evidence

`contracts/scoregate-score/src/types.rs` documents ModelVersionStats as including counter and summary forms. `contracts/scoregate-score/src/storage.rs` — update_model_stats increments submission_count and score_sum but leaves total_submissions and average_score at their initial zero values before storing the struct.

### Expected Behavior

All published fields describe the same accumulated observations and have documented rounding semantics.

### Proposed Solution

Update summary fields from the canonical counters or compute them at read time; handle existing stored records consistently without changing field layout unnecessarily.

### Acceptance Criteria

- [ ] Two accepted scores 20 and 40 yield count 2 and average 30 in both representations.
- [ ] Rejected submissions do not advance statistics.
- [ ] Existing records produce consistent summaries.

### Validation / Test Plan

Test first and repeated submissions, multiple model versions, rejection, and a preexisting record whose summary fields are zero.

## Draft 92

### Title

Connect pair volatility updates to accepted score finalization

### Priority

Medium

### Summary

The pair volatility getter has no production data source because its update helper is never called.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` defines update_pair_volatility, which writes PairVolatilityState, but contains no invocation of that helper. `contracts/scoregate-score/src/storage.rs` provides the matching getter/setter. Normal score ingestion therefore cannot accumulate the series needed by the volatility endpoint.

### Expected Behavior

Every finalized accepted observation updates pair volatility exactly once; rejected or still-pending observations do not.

### Proposed Solution

Integrate the Welford update in the shared finalization path, specify its units and window reset semantics, and ensure all accepted ingestion routes use that path.

### Acceptance Criteria

- [ ] A nonconstant accepted series yields nonzero volatility.
- [ ] Single observations and rejected submissions do not create spurious variance.
- [ ] Window expiry resets the series as documented.

### Validation / Test Plan

Exercise single, batch, consensus, and pending-commit ingestion with a known series and compare stored mean/variance with an integer reference. Inspect call sites to prevent double updates.

## Draft 93

### Title

Validate static correlation coefficients before storing them

### Priority

Medium

### Summary

The correlation setter accepts values outside the documented mathematical domain.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — set_pair_correlation documents a scaled range of -10000 to 10000 but authenticates and stores any i32 without a range check. `get_portfolio_var` consumes that value as a correlation coefficient, so invalid configuration distorts covariance calculations.

### Expected Behavior

Only inclusive scaled correlations in [-10000, 10000] can enter storage.

### Proposed Solution

Validate the range before mutation and use a documented error while preserving existing discriminants. Share validation with any alternate configuration path.

### Acceptance Criteria

- [ ] Both endpoints of the domain and zero pass.
- [ ] -10001, 10001, i32::MIN, and i32::MAX fail without changing prior correlation state.

### Validation / Test Plan

Run boundary tests on a configured pair and inspect unchanged state after rejection. Keep pair-order symmetry and multisig authorization out of this issue, as those have published coverage.

## Draft 94

### Title

Preserve hysteresis validity when the risk threshold changes

### Priority

Medium

### Summary

A valid hysteresis margin can become invalid when a later threshold update is applied.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — set_hysteresis_margin requires margin < risk_threshold, but set_risk_threshold and the risk_thr branch of apply_param_change do not preserve that relation. update_risk_band uses `risk_threshold.saturating_sub(margin)` and clears a band only for score < exit_threshold. A zero exit threshold cannot be crossed by a nonnegative score.

### Expected Behavior

Every threshold-changing path preserves an attainable band-exit condition or explicitly resets the affected band policy.

### Proposed Solution

Validate the joint threshold/margin configuration at proposal and execution time, including policy bundles; reject or explicitly coordinate conflicting updates.

### Acceptance Criteria

- [ ] Lowering a threshold to or below an active margin cannot silently trap wallets in the high-risk band.
- [ ] Valid updates retain existing hysteresis behavior.

### Validation / Test Plan

Configure a nonzero margin, enter the band, then propose/apply a lower threshold; test a margin change between proposal and execution and valid recovery through a low score.

## Draft 95

### Title

Separate immediate cooldown updates from timelocked governance proposals

### Priority

Medium

### Summary

The cooldown API mixes an immediate compatibility update with a pending timelock proposal, leaving operators with two conflicting indications of when the change takes effect.

### Problem / Evidence

`contracts/scoregate-score/src/lib.rs` — set_cooldown stores a ParamChangeProposal with apply_after and emits param_change_proposed, then immediately calls storage::set_cooldown_secs and emits cooldown_updated. This immediate behavior was deliberately retained for backward compatibility in PR #299. The resulting proposal does not defer the effective change and can later reapply a value that is already active.

### Expected Behavior

Operators can distinguish immediate legacy configuration from a genuinely delayed proposal; a timelocked path leaves the effective value unchanged until execution.

### Proposed Solution

Define and document a compatibility migration: retain an explicitly identified immediate legacy path if required, and provide a proposal-only path whose effective write occurs at execution. Do not silently change existing client timing. Ensure pending state and events describe the selected path accurately.

### Acceptance Criteria

- [ ] Immediate legacy calls do not masquerade as deferred changes in pending state or documentation.
- [ ] The delayed path preserves the old cooldown until apply_after and successful execution.
- [ ] Migration documentation and tests state the timing guarantees for existing and new clients.

### Validation / Test Plan

Test both compatibility and delayed paths with a nonzero delay, observing get_cooldown, pending state, events, and submission timing before and after execution. Verify rejected/cancelled proposals do not change effective state.

## Draft 96

### Title

Scope contributor WASM build commands to deployable crates

### Priority

Low

### Summary

The contributor guide asks Cargo to build the entire workspace for a target that includes host-only tools.

### Problem / Evidence

`CONTRIBUTING.md` gives `cargo build --target wasm32-unknown-unknown --release` without a package selector. `Cargo.toml` includes replay, recovery, schema-gen, invocation-fuzzer, and composability members alongside contracts. The CI WASM command instead selects scoregate-score explicitly.

### Expected Behavior

Following the documented release-build command builds the intended deployable contract rather than host-only workspace tools.

### Proposed Solution

Use explicit contract package selection and --locked in the guide; separate native workspace checks from contract WASM checks and identify additional deployable packages deliberately.

### Acceptance Criteria

- [ ] The documented command matches the reviewed CI contract build.
- [ ] Native tool tests remain documented separately.
- [ ] No instruction implies all workspace members are deployable WASM.

### Validation / Test Plan

Compare commands with Cargo metadata and CI, then run the documented build after source blockers are resolved. No production deployment is needed.

## Draft 97

### Title

Repair broken local links in operational documentation

### Priority

Low

### Summary

Several documentation links cannot resolve to their intended local source or policy.

### Problem / Evidence

`docs/commit-reveal-flow.md` links to ../../contracts/scoregate-score/src/lib.rs, which escapes the repository root from docs. `docs/audit-chain.md` links to tools/replay/src/main.rs relative to docs. `docs/operator-alerts.md` points to absent operator-faq.md, and `docs/deprecation-policy.md` points to absent abi-compatibility-notes.md.

### Expected Behavior

Local documentation links resolve to existing maintained files or deliberately identified external references.

### Proposed Solution

Correct relative paths, replace obsolete references with the maintained documents, and add a lightweight local-link check with explicit handling of anchors and external URLs.

### Acceptance Criteria

- [ ] All four reported links resolve.
- [ ] The checker detects a newly broken relative file link and does not request external network access.

### Validation / Test Plan

Run a repository-relative Markdown link scan and manually inspect each replacement target for relevance; render the affected pages to confirm navigation.

## Draft 98

### Title

Generate syntactically valid Python for empty contract structs

### Priority

Low

### Summary

The public Python renderer emits a class with no body for an empty struct specification.

### Problem / Evidence

`tools/schema-gen/src/lib.rs` — struct_to_python appends `class NAME(BaseModel):` and then extends field_lines. When the field list is empty there is no indented statement, so importing or compiling the generated file fails with an expected-indented-block error.

### Expected Behavior

Every supported struct shape, including an empty field list, produces valid Python source.

### Proposed Solution

Emit an explicit pass statement or model configuration body for empty structs and preserve the normal field path for nonempty structs.

### Acceptance Criteria

- [ ] An empty synthetic struct generates a compileable model.
- [ ] A nonempty struct retains its fields.
- [ ] No unintended placeholder field appears in serialization.

### Validation / Test Plan

Generate empty and one-field XDR struct fixtures, run Python compile/import checks, and verify the empty model serializes as an empty object.

## Draft 99

### Title

Offer a strict exit status for recovery snapshot divergence

### Priority

Low

### Summary

Automation cannot use reconciliation exit status to enforce equality.

### Problem / Evidence

`tools/recovery/src/main.rs` — cmd_reconcile computes all_match and prints a divergence warning but returns Ok(()) in both cases. The JSON has the result, but shell pipelines that rely on status alone can proceed after a mismatch.

### Expected Behavior

Operators can explicitly request a nonzero exit on valid-but-different snapshots while retaining the generated report.

### Proposed Solution

Add a documented strict/fail-on-difference option with a distinct status from malformed-input failures; preserve report-only behavior if needed for compatibility.

### Acceptance Criteria

- [ ] Strict mode exits nonzero on any root or count difference and still writes the report.
- [ ] Identical snapshots succeed.
- [ ] Invalid input remains a separate failure.

### Validation / Test Plan

Run the CLI on matching snapshots and each single-field divergence under normal and strict modes; assert report content and exit codes.

## Draft 100

### Title

Enforce the capability and resource assertions in SDK conformance fixtures

### Priority

Medium

### Summary

The conformance fixture advertises checks that its Rust runner silently ignores.

### Problem / Evidence

`tests/composability/sdk_conformance_fixtures.json` declares schema_version, contract_capabilities, and resource_bounds. `tests/composability/tests/sdk_conformance.rs` deserializes only default_config and cases and asserts mapped outcomes, so changing capability requirements or resource ceilings has no effect on the test.

### Expected Behavior

A fixture pass establishes its declared capabilities and measurable resource constraints as well as behavior outcomes.

### Proposed Solution

Deserialize and validate the complete fixture contract, probe required capabilities, and measure supported resource assertions around the decision. Explicitly mark unsupported metrics rather than silently ignoring them.

### Acceptance Criteria

- [ ] An unsupported capability or exceeded enforced resource bound fails the test.
- [ ] Unsupported schema versions fail parsing.
- [ ] Each advertised metric is checked or clearly declared informational.

### Validation / Test Plan

Mutate a fixture capability and lower a measured bound below observed usage, verifying each causes a failure; restore the fixture and run the standard conformance suite.

## Review record

This section is local review metadata, not part of any publishable issue body.

### Completeness and source validation

Final inventory: **100 fully expanded drafts — 3 High, 68 Medium, 29 Low**. A programmatic check verified sequential navigation 1–100, exactly one of each of the eight required sections per body, nonempty content, acceptance checkboxes, unique titles, existing repository evidence paths, 100 matching metadata rows, and proposed labels present in the fetched repository issue records. No candidate-only entries remain. The check also rejects wave names, draft-number references, complexity classifications, and first-issue wording inside bodies.

The review covered score and aggregator contracts, mock consumers, shared test support, contract/integration tests, benchmarks, schema generation and committed schema artifacts, replay/recovery/fuzz tooling, shell/Python scripts, workflows, deployment manifests, examples, formal specifications, and operator/contributor documentation. Findings describe the inspected checkout, not a claim that every proposed regression test has already run. Synthetic schema fixtures are explicitly identified where a supported renderer branch is not exercised by the currently emitted four canonical structs.

### Semantic exclusion review

The comparison corpus was refreshed through four paginated read-only GitHub requests: **259 issues and 70 PRs**, 329 records in total, ending at #329. Title and body searches across the full corpus identified related work; related issue descriptions and PR scopes were then compared with source behavior and the requested fix. A separate comparison of backlog evidence and requested outcomes checked the entries against each other. Lexical similarity was used only to locate review candidates, not as proof of semantic independence.

The following records capture the important scope boundaries. Numbers in the first column are local navigation, outside the issue bodies. Published numbers refer to `hartz0/scoregate-contracts`.

| Local navigation | Published exclusions and semantic decision |
|---|---|
| 1–6, 43–47, 98 | Issues #274/#280 and PRs #319/#329 cover additional canonical types and TypeScript integer precision. The retained findings concern independent renderer behavior: check-mode mutation, root validation, byte encoding, imports, union precedence, result tags, tuple cardinality, map fidelity, dependency resolution, integer domain validation, unknown fields, and empty Python classes. No additional-type or number-to-bigint issue is recounted. |
| 7–8, 60–65 | No matching release/provenance outcome in the published corpus. Independent build isolation, missing checkout, authenticated provenance, binding the optimized artifact, portable checksum paths, shell-safe notes, SBOM attachment, and repository-specific instructions have separate failure conditions and fixes. |
| 9 | Mutation target selection is distinct from contract WASM lint coverage in #294 and size coverage in #253. |
| 10 | #295 requests multi-contract error scanning; this finding is failure to reject an invalid comparison ref in the existing checker. |
| 11, 74–77 | #127/#213 and PRs #304/#327 concern CLI arguments and RPC failure attribution. These entries address missing on-chain enumeration, malformed records, repeated logical keys, EOF handling, and report assembly cost; they do not recount transport handling. |
| 12 | #48 changes byte measurement and #253 expands contract coverage. The current parser still cannot associate the documented 599,000-byte budget with its contract and silently falls back to 1 MiB. |
| 13 | #202–#205/#245–#248 concern mock administration, operation authorization, pause, and limits. First-initialization versus reinitialization ownership is a separate missing guard in both mocks and is kept as one combined issue. |
| 14–18 | No published traceability checkpoint/coverage issue was found. Input binding, checkpoint structure, empty evidence, identifier validity, and execution-claim wording are independent requirements. |
| 19–20 | #45/#208 and PRs #130/#306 add metric categories. The retained comparison defect is one-sided observations, including state and events; ordering is a separate reproducible-report requirement. |
| 21–22 | #275 and PR #315 concern event-to-replay format compatibility. Request bounds and atomic output replacement remain separate export reliability problems; the adapter compatibility problem is excluded. |
| 23 | Replaced the inherited service-liveness draft because its exit-code-versus-value root cause was too close to #252. The replacement concerns malformed command fences in the size guide. |
| 24, 67 | #49/#209 and PRs #129/#304 address missing network fields and fixture configuration. Address checksum validation is a helper-level correctness issue; identity resolution before deployment is a separate workflow ordering issue. |
| 25–27, 42 | #273 is mock fail-open integration coverage, not the shared helper's blanket authorization or the examples' guarantees. Arithmetic overflow is consolidated as an example calculation issue; the oracle adapter's absent Cargo target is separate. |
| 28 | #107/#161 validate cluster boundaries. Implementing the always-empty public membership query is a distinct missing behavior. |
| 29, 34 | #289 concerns token-bucket state reset during override. Score observation age and capacity reporting in flat cooldown mode are different public query results. |
| 30 | Published failover issues #59/#224/#244 concern secondary score contracts. The retained problem is the registered price oracle's self-perpetuating stale consultation branch. |
| 31 | #89/#90/#285 and PRs #151/#309 concern authorization/configuration/governance roots. This entry concerns the keyed score-record root and omitted persisted score fields. |
| 32 | #182 caps retained history; #265/PR #326 bound pending-proposal pruning. The separate `cleanup_expired_parameter_proposals` loop still scans the lifetime `1..next_id` range after invoking pruning. Its cursor/scan budget is not supplied by the pending-vector fix. |
| 33 | Published parameter-bound fixes do not cover the single-versus-bulk signer-tier validation mismatch. |
| 35 | #37 and PR #139 document supports_interface. The retained issue changes runtime metadata enumeration, not rustdoc. |
| 36 | #218 and PR #299 add required reviewer enforcement. This finding bounds the newly introduced approval-write API to actual active targets rather than requesting reviewer enforcement again. |
| 37 | #31/#114/#166 address freshness precedence; #259 adds differential tests. The retained production behavior concerns equal-timestamp aggregate ties, preserving the existing freshness rule. |
| 38–41 | #121 concerns rejection discriminants; #292 concerns failure-inject dispatch and swallowed failures. Header validation, actual event capture, numeric trade validation, and error locations are different replay behaviors. |
| 48–51, 99 | #46/#122/#123/#206/#207/#250 and PRs #130/#155/#304/#310 cover count checks, short strings, array format, date conversion, pre-action count, and invalid root verification. Retained findings concern record semantics, equivalent hex encodings, origin binding, actual action time, and an opt-in strict reconciliation status. |
| 52–53 | #47/#124/#249/#293 concern operation coverage, symbol generation, wire values, and downstream event invariants. Mutator capacity and failure-preserving shrinking are separate harness algorithms. |
| 54–55, 85 | #251 adds data-segment offsets. Zero-baseline percentages and new-module attribution are independent analysis calculations; module registration is the prerequisite that makes these files and their tests compile at all. |
| 56 | No published qualified-symbol ownership check exists. This is stronger resolution of existing references, not adding another refinement document. |
| 57 | #50/#200/#201 and PR #303 establish event checking, file coverage, and the host topic bound. The retained parser defect rejects a legal trailing-comma tuple and cannot analyze locally bound topics. No contract topic-limit issue is duplicated. |
| 58–59, 78–80 | Report preservation on failed CI, schema-check enforcement, stale local artifact attribution, explicit size-report input handling, and bounded SBOM collection have no matching published outcomes. The schema CI entry depends on read-only check behavior but is not the same CLI change. |
| 66, 69–73 | #34/#210/#211/#212/#254 address CLI spelling, pair length, retrieval failures, array quoting, and failure injection. Retained work concerns lockfile enforcement, working directory, dry-run isolation, an actual canary round trip, restoration of initial pause state, and value reconciliation. |
| 68 | #211 checks retrieval failures in verify-deployment.sh. This entry compares successful but wrong admin/service/version values in deploy.sh. |
| 81, 88–90, 100 | Published coverage requests concern other specific contract behavior. These entries expose undiscovered documentation/error tests, select the correct benchmark harness, measure the enabled noise branch, and enforce fixture fields the conformance runner currently ignores. |
| 82–84 | No corresponding published formal-model issue was found. Replacement reachability, an observable embargo gate invariant, and upgrade signer snapshot properties target different model obligations. |
| 86–87 | The missing config-drift CLI dispatch and incomplete-manifest false success are separate: wiring the existing library does not repair its validation semantics. Neither duplicates #292's failure-inject command. |
| 91–92 | #39/#277 and PRs #139/#317 concern invoking the existing finalization pipeline. Model summary fields are not populated even when their helper runs; pair volatility has no update call on any production ingestion path. These are distinct from batch-only omission of an existing pipeline. |
| 93–94 | #81/#287 and PRs #146/#309 concern correlation authorization/order; #288 concerns hysteresis authorization. Correlation value bounds and threshold/margin transition validity remain independent. |
| 95 | #220/PR #299 deliberately retained immediate cooldown updates for compatibility while adding pending proposals. The draft is an explicit compatibility/semantics improvement, not a claim that the published cooldown application fix was omitted. |
| 96–97 | Contributor package selection and broken local documentation links have no corresponding published outcome. Package selection in prose is separate from adding missing packages to the lint script in #294. |

Rejected inherited leads include already-published fee/auth/finality/event fixes, historical deletion cleanup requests, the event-export adapter compatibility issue, and build failures arising from previously reported history/dormancy/pair-bound changes. They were not counted merely because current source still exhibits a regression or a merge defect.

### Checks run and verification limits

- `cargo test -p recovery --locked`: **passed, 5 tests**.
- `python3 -m unittest discover -s tests -p test_traceability.py`: **passed, 12 tests**. Passing baseline tests do not cover the newly identified traceability edge cases.
- `cargo metadata --no-deps --format-version 1`: **passed**; confirmed that the root documentation synchronization test and oracle adapter are absent from registered targets.
- Focused local reproductions confirmed: empty traceability input reports PASSED; boolean/empty test IDs pass validation; the refinement checker accepts the wrong-owner reference `TokenBucket.score`; the event parser counts a four-topic trailing-comma tuple as five; and the reconciliation loop pattern drops an unterminated last line.
- `bash tools/check_error_discriminants.sh scoregate-nonexistent-ref HEAD`: **incorrectly exited 0**, confirming the invalid-ref finding.
- `cargo check --workspace --locked`: **failed with the same three existing score-contract errors**: missing `storage::trim_score_history` at `contracts/scoregate-score/src/lib.rs:3777`, a u64/u32 dormancy event mismatch at line 4954, and missing `Error::InvalidAssetPair` at line 9430. These were not repaired as part of backlog writing.
- `cargo fmt --all -- --check`: **failed** on existing formatting differences and the malformed delimiter in `contracts/mock-lending/src/lib.rs:209`. No formatting rewrite was applied.
- Final body/section/path/label validation: **passed for exactly 100**. Final `git diff --check`: **passed**.

Contract-dependent regression plans, generated binding compilation, live RPC/deployment behavior, release workflow execution, fuzz campaigns, Criterion measurements, and TLC mutation checks remain proposed validation work. Static findings are not represented as executed contract proofs. Builds and formatting were checked once during this continuation rather than repeatedly retried.

Only `drips wave backlog.md` was edited during this continuation. The existing rename from `drips wave 9.md` and the eight pre-existing source/example cleanup edits were preserved. Nothing was committed, pushed, published, or changed on GitHub.
