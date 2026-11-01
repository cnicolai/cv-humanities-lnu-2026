# Computer vision for the humanities

Material for the lecture *Introducing computer vision for the humanities* (Linnaeus University,
3 November 2026) and for the workshop the day after.

**The lecture handout:** [handout.pdf](handout.pdf), the lecture in twenty pages.

## Workshop notebooks

Three notebooks, ordered by difficulty. They run in Google Colab, in your browser: there is
nothing to install, and a free Google account is enough.

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

All pages and scans are public domain; [SOURCES.md](SOURCES.md) says where each one comes from.
