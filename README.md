# Deep Learning Coursework

Coursework portfolio edition by **Behrad Mazaheri**, based on 14 uploaded notebooks associated with Sharif University of Technology's Deep Learning course. Headers identify different assignments/semesters (including Spring 2025 and Spring 2026); they are preserved rather than relabeled into one term.

**Static source and saved-output review only. No training, generation or evaluation was rerun.** Suggested separate repository name: `deep-learning-coursework`.

| Notebook | Code cells | Saved errors | Evidence status |
| --- | ---: | ---: | --- |
| [NumPy Regression Neural Network](01-numpy-neural-network/) | 25 | 0 | Historical outputs + review |
| [Optimization on Ackley and Beale](02-optimization-landscapes/) | 24 | 0 | Historical outputs + review |
| [Synthetic Emoji CNN Classification](03-synthetic-emoji-cnn/) | 17 | 0 | Historical outputs + review |
| [Synthetic CAPTCHA Segmentation and Recognition](04-captcha-segmentation-recognition/) | 17 | 0 | Historical outputs + review |
| [RNN and LSTM Sentiment Classification](05-rnn-lstm-sentiment/) | 33 | 0 | Historical outputs + review |
| [Retrieval-Augmented and Conversational Generation](06-retrieval-augmented-generation/) | 19 | 0 | Historical outputs + review |
| [Multi-Task LoRA Specialization and Transfer](07-multitask-lora/) | 14 | 0 | Historical outputs + review |
| [LLM Inference Strategies on GSM8K](08-llm-inference-strategies/) | 15 | 0 | Historical outputs + review |
| [Face VAE Reconstruction and Latent Analysis](09-face-vae-analysis/) | 49 | 0 | Historical outputs + review |
| [MNIST DDPM and Classifier-Free Guidance](10-mnist-ddpm/) | 29 | 0 | Historical outputs + review |
| [Hierarchical VQ-VAE-2 on Omniglot](11-omniglot-vqvae/) | 11 | 0 | Historical outputs + review |
| [Latent Diffusion Sampling and Image Editing](12-latent-diffusion-editing/) | 20 | 0 | Historical outputs + review |
| [Self-Supervised SimCLR (Unexecuted)](13-simclr/) | 11 | 0 | Unexecuted source |
| [CLIP Remote Sensing, LoRA and Retrieval](14-clip-remote-sensing/) | 77 | 2 | Historical outputs; interrupted run |

## What is included

Each folder has a readable notebook, English README, dependency inventory, data/checkpoint requirements, attribution, static findings and machine-readable historical text outputs. Existing figures are retained. Six selected folders also have `revised.ipynb`: unexecuted changes with **all outputs cleared**.

No external dataset, pretrained weight, trained adapter, original helper module or checkpoint was downloaded or reconstructed. The two numerical-network notebooks from different courses are separate artifacts; results from earlier AI/ML packages are not imported into this repository.

## Findings that affect portfolio claims

- **NumPy NN:** missing utils modules; integer-cast housing targets; some full-network gradient errors exceed stated targets.
- **Emoji CNN:** overlapping training/validation generation seeds; named improved model has worse saved test results (0.53 versus 0.84).
- **RNN/LSTM:** stored test contains no negative examples, so displayed binary accuracy is misleading. Vocabulary and split design need correction.
- **RAG:** retrieval examples exist, but saved generation includes wrong answers and repetition; no aggregate QA accuracy is shown.
- **VQ-VAE:** FID 10.12 is for training-set reconstructions, not unconditional generation; codebook use is limited.
- **Face VAE:** standard, bootstrap and learned priors are different protocols. Stored posterior-bootstrap FID 134.86 is lower than GMM 156.67. Proxy attributes are not real fine-grained annotations.
- **SimCLR:** source is present, but all code cells are unexecuted with no results.
- **CLIP:** saved LoRA training was interrupted, despite later evaluation. Prompt optimization reuses test labels, and diffusion reloads are out of order.

The folder reviews give cell-specific evidence and remaining blockers. A completed filename or saved plot is not proof of an end-to-end correct run.

## Setup

Use a per-notebook virtual environment. `requirements.txt` is an import/dependency inventory, not a verified environment lock. Inspect notebook-side installation/authentication/download cells before execution. Most PyTorch training tasks benefit from a GPU; reading outputs does not require one. Large face datasets and diffusion weights can be several GB and are not bundled.

For publication, upload the contents of this top-level folder to a separate GitHub repository. Each notebook stays with its README/evidence files.

## Structural verification

`tools/validate_notebooks.py` checks notebook schemas and IPython-transformed Python syntax **without executing cells**. `STATIC_REVIEW.json` records this preparation's actual result. Runtime name resolution, data availability, training correctness and reproducibility are outside this structural check.

## Attribution

Student numbers and temporary signed download URLs are removed; original course/template credits remain. Framework models, pretrained weights and teacher scaffolds are distinguished from handwritten algorithms. No license is imposed on course/third-party assets. Confirm individual/group contributions before CV authorship claims. `PORTFOLIO_NOTES.md` suggests conservative wording; no CV file was edited.
