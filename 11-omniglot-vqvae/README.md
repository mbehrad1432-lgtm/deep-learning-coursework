# Hierarchical VQ-VAE-2 on Omniglot

Hierarchical two-level VQ-VAE with EMA codebooks, reconstruction, codebook analytics, top/bottom ablation and Inception-feature distance on Omniglot.

## Saved evidence — not rerun

Stored reconstruction FID 10.12 from 2,000 real/reconstructed images (15). Ablation SSIM: full 0.9936, top-only 0.1600, bottom-only 0.9591 (20). Early/late perplexities stay around 2–3 top codes and 5–7 bottom codes despite large codebooks (13), indicating limited code utilization.

All metrics are copied from uploaded outputs. This preparation did not execute training, generation, evaluation or existing numerical checks. Original zero-based cell indices are cited; the public copy adds a banner.

![Existing saved figure](evidence/preview.png)

## Setup and source variants

Read DATA_REQUIREMENTS.md for exact datasets, helper modules, model IDs and missing checkpoints. Requirements list imports, **not a tested lockfile**. In a separate Python environment, from this folder:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Reading saved outputs requires no dataset or GPU download. Executing source may require platform-specific setup, external weights and substantial compute. Notebook package-install cells should be reviewed before running.

`notebook.ipynb` retains the submitted computational source and historical outputs after publication cleanup. No revised algorithm variant is supplied.

## Recorded notebook status

11 code cells, 0 saved error outputs, 0 nonempty code cells without execution counts. Execution counts and absence of errors do not prove a clean sequential run. See REVIEW.md and ATTRIBUTION.md.
