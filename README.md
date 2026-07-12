# ML 1 & 2 Coursework

Coursework archive from two machine learning courses: **ML1** (classic ML
algorithms) and **ML2** (neural networks). Labs are implemented from
scratch in NumPy and, in most cases, compared against a scikit-learn (or
equivalent) reference implementation.

## Flagship project (extracted)

The Quarter 2 project from ML1 — a co-authored research project on
**adaptive feature-weighted KNN**, with a written proposal and evaluation
on real medical datasets (breast cancer, diabetes, heart disease) — has
been extracted into its own standalone repo:

**[KuvaKodes/adaptive-feature-weighted-knn](https://github.com/KuvaKodes/adaptive-feature-weighted-knn)**

It's no longer bundled here; everything else from both courses remains in
this archive.

## ML1 — Classic ML Algorithms

- `Lab 0.py` — Intro plotting with matplotlib/numpy.
- `Lab 2 - Kushaan Vardhan` — ARFF datasets for missing-value handling and
  discretization exercises (automobile dataset).
- `Kushaan Vardhan - Lab 4` — Dataset splitting (uniform and stratified)
  on the Iris and weather datasets.
- `Lab 7 - Kushaan Vardhan` — Naive Bayes and OneR, each implemented from
  scratch and compared against a scikit-learn implementation, on a
  diabetes dataset.
- `Lab 8 - Kushaan Vardhan` — Decision trees and random forests
  implemented from scratch (with a from-scratch `Node`/tree class) on the
  wine dataset.
- `Lab 9 - Kushaan Vardhan` — K-Nearest Neighbors implemented from scratch
  and applied across several variations/parts, on the Iris dataset.

## ML2 — Neural Networks

- `Lab 0` — SVM on Iris (scikit-learn), a warm-up before the perceptron
  material.
- `Lab 1` — A from-scratch `Perceptron` class, applied to Iris
  classification and compared against a scikit-learn labeled version.
- `Lab 2` — Hand-built perceptrons for logic gates (AND/OR/NAND/etc.) and
  related exercises.
- `Lab 3` — Backpropagation from scratch, culminating in a full
  feedforward neural network trained on MNIST digit classification
  (`Part2.py`). This is a substantial standalone implementation — forward
  pass, backprop, and weight updates all hand-written — and worth a look
  in its own right. It's an earlier, rougher effort in the same spirit as
  the later, more polished
  [mnist-neural-net-from-scratch](https://github.com/KuvaKodes/mnist-neural-net-from-scratch)
  repo from subsequent AI coursework. See `ML2/Lab 3/README.md` for notes
  on the (removed) MNIST data files needed to run it.
- `CNN Worksheet` — Convolutional neural network mechanics worked by hand
  (padding, ReLU, etc.), without a deep learning framework.

## Notes on repo hygiene

Large/broken data artifacts (a broken git-lfs pointer, raw MNIST CSVs, and
a pickled checkpoint in `ML2/Lab 3`) were removed to keep this repo small;
see `ML2/Lab 3/README.md` for how to regenerate them locally.
