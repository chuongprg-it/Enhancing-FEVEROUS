# Enhancing FEVEROUS



## Setup

We recommend to create a new environment for experiments using conda:

```bash
conda create -y -n mla python=3.9
conda activate mla
```

Then, install `mla` from the repository:

```bash
git https://github.com/nii-yamagishilab/MLA-FEVEROUS-COLING24.git
cd MLA-FEVEROUS-COLING24
pip install -r requirements.txt
pip install feverous
pip install einops
pip install wandb
python -c "import wandb; wandb.login()"
```

To ensure that PyTorch is installed and CUDA works properly, run:

```bash
python -c "import torch; print(torch.__version__); print(torch.cuda.is_available())"
```

We should see:

```bash
1.12.1+cu113
True
```

:warning: We use PyTorch 1.12.1 with CUDA 11.3. You may need another CUDA version suitable for your environment.

For further development or modification, we recommend installing `pre-commit`:
```bash
pre-commit install
```

## Experiments

See [experiments](experiments).

## Pre-trained modesl 

[Pre-trained models part 1] : https://doi.org/10.5281/zenodo.10901784

[Pre-trained models part 2] : https://doi.org/10.5281/zenodo.10902611



