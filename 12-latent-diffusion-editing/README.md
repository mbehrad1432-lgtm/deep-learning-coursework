# Latent Diffusion Sampling and Image Editing

Pretrained latent diffusion components exposed explicitly: VAE round-trip, forward noise/SNR, manual DDIM reverse loop, classifier-free guidance, prompt embeddings, Pix2Pix and inpainting.

## Saved evidence — not rerun

Stored single-image VAE round-trip PSNR 25.67 dB (15), plus grids showing sampling steps, CFG, embedding edits, sequential instruction edits and masked inpainting.

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

20 code cells, 0 saved error outputs, 0 nonempty code cells without execution counts. Execution counts and absence of errors do not prove a clean sequential run. See REVIEW.md and ATTRIBUTION.md.
