# Static review

- This is an educational QA/retrieval pipeline, not an established high-accuracy production chatbot.
- Correct retrieval does not ensure grounded generation; examples demonstrate hallucination.
- Conversational query rewriting does not guarantee correct answer selection.
- A small SQuAD validation subset provides corpus and example questions; this is not an independent generalization benchmark.
- Language models, embeddings and FAISS caches are external and not bundled.

## Supplied revisions

None; submitted source and saved evidence remain, with limitations documented above.

Only structural schema/syntax checks were performed. No fresh model scores, gradient-test outcomes, runtime benchmarks or successful Run-All claim is made.
