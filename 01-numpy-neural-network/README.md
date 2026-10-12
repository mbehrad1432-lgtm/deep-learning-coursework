# NumPy Regression Neural Network

Modular NumPy regression MLP: affine/ReLU/sigmoid derivatives, MSE, L2 and SGD momentum; housing training depends on absent course utilities.

## Saved evidence — not rerun

Saved affine gradient errors are approximately 1e-10 (11); MSE gradient error 2.86e-9 (29). Full-network relative checks are not all below the stated 1e-7 target: W2 with reg=3.14 reports 4.8371e-4 (33). The final training log reports validation RMS error 1.533512 at epoch 20 (44), on integer-cast targets.

All metrics are copied from uploaded outputs. This preparation did not execute training, generation, evaluation or existing numerical checks. Original zero-based cell indices are cited; the public copy adds a banner.

![Existing saved figure](evidence/preview.png)

## Setup and source variants

Read DATA_REQUIREMENTS.md for exact datasets, helper modules, model IDs and missing checkpoints. Requirements list imports, **not a tested lockfile**. In a separate Python environment, from this folder:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Reading saved outputs requires no dataset or GPU download. Executing source may require platform-specific setup, external weights and substantial compute. Notebook package-install cells should be reviewed before running.

`revised.ipynb` contains selected static fixes and cleared outputs. It was not executed and may retain blockers in REVIEW.md; historical metrics do not apply to this revision.

## Recorded notebook status

25 code cells, 0 saved error outputs, 0 nonempty code cells without execution counts. Execution counts and absence of errors do not prove a clean sequential run. See REVIEW.md and ATTRIBUTION.md.
