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
  model's errors. Unzip it and double-click `cer.html`; it opens in your browser and works offline.
- **LM Studio** from [lmstudio.ai](https://lmstudio.ai), on a Mac with Apple Silicon and macOS 14
  or newer, or on a Windows laptop, with at least 8 GB of memory. Step 0 of the guide says
  which Gemma 4 model fits your laptop. If you can, install LM Studio and download the model
  before the workshop: the larger ones take long over a shared Wi-Fi.

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
folder; there is nothing else to fetch. All three run on Colab's free processor. In notebook 03,
the cell that trains the network takes a few minutes.

## Sources

All pages, scans and letters are public domain; [SOURCES.md](SOURCES.md) says where each one
comes from.
