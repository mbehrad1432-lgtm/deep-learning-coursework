# Retrieval-Augmented and Conversational Generation

Sentence-Transformer embeddings, FAISS retrieval, GPT-2 generation, conversational query handling, LangChain components and FLAN-T5 comparison on SQuAD contexts.

## Saved evidence — not rerun

Qualitative outputs show successful retrieval but wrong/repetitive generation. The stored comparison (30) returns Denver Broncos for both AFC and NFC questions with T5; the second gold answer is Carolina Panthers. GPT-2 examples incorrectly generate New England Patriots. No dataset-wide EM/F1 or factuality metric is recorded.

All metrics are copied from uploaded outputs. This preparation did not execute training, generation, evaluation or existing numerical checks. Original zero-based cell indices are cited; the public copy adds a banner.

## Setup and source variants

Read DATA_REQUIREMENTS.md for exact datasets, helper modules, model IDs and missing checkpoints. Requirements list imports, **not a tested lockfile**. In a separate Python environment, from this folder:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Reading saved outputs requires no dataset or GPU download. Executing source may require platform-specific setup, external weights and substantial compute. Notebook package-install cells should be reviewed before running.

`notebook.ipynb` retains the submitted computational source and historical outputs after publication cleanup. No revised algorithm variant is supplied.

## Recorded notebook status

19 code cells, 0 saved error outputs, 0 nonempty code cells without execution counts. Execution counts and absence of errors do not prove a clean sequential run. See REVIEW.md and ATTRIBUTION.md.
