# Static review

- Source concatenates official IMDb train/test, constructs a vocabulary on the combined corpus, then slices contiguous rows.
- Ordering creates single-class validation/test tails.
- Vocabulary selection before splitting leaks holdout distribution.
- Recurrent models use final states without masking/right-padding length control; padding can affect predictions.
- Custom RNN/LSTM cells are handwritten, while nn.RNN/nn.LSTM are PyTorch models.
- Revised stratified splitting fixes class coverage only, not vocabulary leakage or loss of official partitions.

## Supplied revisions

- Replaced contiguous ordered splitting with seeded class-wise random splitting.
- Vocabulary is still fitted before splitting, and official IMDb partitions are still combined; these limitations are NOT fixed.
- Padding-aware recurrent state/length handling still requires a coherent redesign.

Only structural schema/syntax checks were performed. No fresh model scores, gradient-test outcomes, runtime benchmarks or successful Run-All claim is made.
