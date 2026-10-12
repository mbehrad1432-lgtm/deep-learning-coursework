# Static review

- These are 64 selected examples, not the full 1,319-row source benchmark.
- Long /think outputs hit the 512-token limit in the saved averages, so reasoning can be truncated.
- Answer extraction and invalid-output handling affect exact-match accuracy.
- The methods have different generation budgets and number of calls.
- Hardware, warm-up and batching affect saved latency; this is not a portable performance guarantee.
- Generated details/cleaned JSON files named by code are not attached.

## Supplied revisions

None; submitted source and saved evidence remain, with limitations documented above.

Only structural schema/syntax checks were performed. No fresh model scores, gradient-test outcomes, runtime benchmarks or successful Run-All claim is made.
