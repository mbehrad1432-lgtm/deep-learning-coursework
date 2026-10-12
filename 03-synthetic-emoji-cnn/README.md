# Synthetic Emoji CNN Classification

PyTorch CNNs trained from random initialization on five classes of procedurally rendered emoji, with augmentation, error inspection and feature maps.

## Saved evidence — not rerun

Stored BaselineCNN test accuracy 0.84 and macro F1 0.828178; the named BetterCNN scores 0.53 and 0.431078 (34). Split counts are 300 train, 80 validation and 100 harder-mode test examples (9). The larger architecture did not improve this saved experiment.

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

17 code cells, 0 saved error outputs, 0 nonempty code cells without execution counts. Execution counts and absence of errors do not prove a clean sequential run. See REVIEW.md and ATTRIBUTION.md.
