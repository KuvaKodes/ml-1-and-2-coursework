# Lab 3 — Backpropagation & a From-Scratch MNIST Neural Net

- `Part1.py` — A minimal, hand-worked backpropagation example (fixed toy
  weights/inputs, sigmoid activations) that trains for 10,000 epochs and
  plots the error trend. Self-contained, no external data needed.
- `Part2.py` — A full feedforward neural network implemented from scratch
  (forward pass, backpropagation, weight/bias updates — no ML framework)
  trained on MNIST digit classification.

## Data files (not included in this repo)

`Part2.py` expects two CSV files in this folder, in the standard
"MNIST in CSV" format (first column = digit label 0-9, remaining 784
columns = flattened 28x28 pixel values 0-255):

- `mnist_train.csv`
- `mnist_test.csv`

These are **not committed** here:

- The `mnist_train.csv` that was originally in this folder was a broken
  git-lfs pointer file (~134 bytes of metadata only — the real ~110MB file
  was never actually uploaded/tracked correctly), so it was non-functional
  anyway.
- `mnist_test.csv` (~17MB) and the pickled checkpoint `save_data.pkl`
  (~2MB) were large committed binary artifacts that bloated the repo, so
  they were removed to keep this a lean coursework archive.

To run `Part2.py`, download "MNIST in CSV" (e.g. from Kaggle or OpenML)
and place `mnist_train.csv` / `mnist_test.csv` in this directory.

This script is an earlier, rougher effort compared to the more polished
[mnist-neural-net-from-scratch](https://github.com/KuvaKodes/mnist-neural-net-from-scratch)
repo from later AI coursework — but it's a substantial standalone
implementation in its own right and worth a look.
