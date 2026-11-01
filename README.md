# Computer vision for the humanities

Material for the lecture *Introducing computer vision for the humanities* (Linnaeus University,
3 November 2026) and for the workshop the day after.

**The lecture handout:** [handout.pdf](handout.pdf), the lecture in twenty pages.

## Workshop

Two paths: read handwritten letters with a language model on your own laptop, or work through
three notebooks in your browser. Take one, or both one after the other.

## Read a letter page, in LM Studio

A language model on your own laptop reads letters from the 1860s. You measure how wrong it is,
write a better prompt, and try it on the next letter. There is no code, and nothing leaves your
laptop.

- **The guide:** [read-a-letter-page.pdf](read-a-letter-page.pdf), one step per page.
- **The letters:** [letters.zip](https://raw.githubusercontent.com/cnicolai/cv-humanities-lnu-2026/main/letters.zip):
  three letter pages, each as a scan and as transcribed, and `cer.html`, which counts the
  model's errors. Unzip it and double-click `cer.html`. It opens in your browser and works offline.

### Install LM Studio and Gemma 4

If you can, do this before the workshop: the download takes a while over a shared Wi-Fi.

LM Studio runs on a Mac with Apple Silicon and macOS 14 or newer, or on a Windows laptop, with at
least 8 GB of memory. It does not run on an Intel Mac: take the notebooks instead, or pair up
with someone.

1. Download LM Studio from [lmstudio.ai](https://lmstudio.ai) and install it.
2. In LM Studio, open *Model Search* and search for `gemma-4`.
3. Download **Gemma 4 E2B**, a good first choice that runs with 8 GB of memory:
   - on a Mac, the **MLX** version in **4-bit** (about 4.3 GB)
   - on Windows, the **GGUF** version in **`Q4_K_M`** (about 4.4 GB)

## Three notebooks, in Colab

Three notebooks, ordered by difficulty. They run in Google Colab, in your browser: there is
nothing to install, and a free Google account is enough. The short guide:
[three-notebooks.pdf](three-notebooks.pdf).

| notebook | what you do | |
|---|---|---|
| **01 Filters: the page as numbers** | lay filters over a page of a letter by George Stephens, then set one filter's numbers yourself | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cnicolai/cv-humanities-lnu-2026/blob/main/notebooks/01-filters.ipynb) |
| **02 The learning loop** | run the loop from the lecture on twelve points and turn its knobs: the step size, the number of parameters, the amount of training data | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cnicolai/cv-humanities-lnu-2026/blob/main/notebooks/02-learning-loop.ipynb) |
| **03 Straighten the scans** | make training data from pages known to be straight, train a small neural network, and let it straighten six crooked scans | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cnicolai/cv-humanities-lnu-2026/blob/main/notebooks/03-straighten.ipynb) |

### How to start

1. Click *Open in Colab* beside a notebook and sign in with your Google account.
2. Choose *File → Save a copy in Drive*. Your copy opens in a new tab: work there, because changes
   to the notebook opened from GitHub are not saved.
3. Run the cells one at a time with Shift+Enter. If Colab warns that the notebook was not
   authored by Google, choose *Run anyway*.

The first code cell of notebooks 01 and 03 downloads their pages from this repository's `data`
folder. There is nothing else to fetch. All three run on Colab's free processor. In notebook 03,
the cell that trains the network takes a few minutes.

## Sources

All pages, scans and letters are public domain. [SOURCES.md](SOURCES.md) says where each one
comes from.
