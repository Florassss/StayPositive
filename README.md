# Introduction

This is a small demo for the CVPR submission _Stay Positive: Non-Negative Image Synthesis for Augmented Reality_.
The demo requires a simple installation process (presented in the next section).
It takes an input image (e.g. `trainA.png`) and a proposed target image (e.g. `trainB.png`), and run the optimization process proposed in Section 3 of the paper to produce an output image that tries to be perceptually similar to the propose target while fulfilling the non-negative constraints.
The whole optimization process is written in a jupyter notebook `Demo.ipynb`, whose usage will be presented in the following section.

# Installation

This demo depends on the following packages:
* Conda (4.8.5)
* Pytorch (1.7.0)
* Matplotlib (3.3.2)
* Numpy (1.19.2)
* tqdm (4.51.0)
* Jupyter notebook (1.0.0)

Following is a simple way to install the required dependencies.

```bash
conda env create -f environment.yml
conda activate non_negative
python -m ipykernel install --user --name non_negative
```

# Usage

To see the demo, install the environment following instructions from previous section, then run the jupyter notebook.
The demo will be in `Demo.ipynb`:

```bash
conda activate non_negative
jupyter notebook
```
