# Static review

- Dataset __getitem__ synthesizes a fresh example each call, including validation. Epoch validation losses therefore use changing samples.
- The sequence reader trains on ground-truth binary masks (19), while the final pipeline uses predicted masks (33); this is a train/inference domain gap.
- Exact-sequence accuracy and per-character accuracy are distinct and must not be interchanged.
- The raw-image qualitative example in cell 31 uses its training loader, not held-out evaluation.
- Checkpoint/model artifacts are absent; synthetic fonts/rendering can vary across environments.

## Supplied revisions

None; submitted source and saved evidence remain, with limitations documented above.

Only structural schema/syntax checks were performed. No fresh model scores, gradient-test outcomes, runtime benchmarks or successful Run-All claim is made.
