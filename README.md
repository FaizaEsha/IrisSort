# 🌸 IrisSort

Classifying Iris flowers through machine learning — entirely in the browser.

## 🔍 Overview

IrisSort is a self-contained implementation of a K-Nearest Neighbors
classifier trained on Fisher's Iris dataset, built as Project 2 (*Data
Classification Using AI*) for the DecodeLabs Industrial Training Kit.

There is no backend, no build step, and no external ML library — the
entire pipeline, from data shuffling to prediction, is written in plain
JavaScript and runs the moment the page loads.

## ⚙️ How it works

On every load, the page:

1. 🔀 **Shuffles** all 150 flowers to remove any ordering bias in the dataset.
2. ✂️ **Splits** them 80/20 into a training set and a held-out test set.
3. 📏 **Standardizes** the four measurements (sepal length/width, petal
   length/width) to mean 0 and standard deviation 1, fitted on the
   training set only.
4. 🌱 **Classifies** the test set using K-Nearest Neighbors (K = 5).
5. 📊 **Reports** accuracy, weighted F1 score, and a full confusion matrix.

Because the train/test split is re-shuffled on every load, accuracy
naturally varies slightly from run to run — this is expected behavior
for a proper random split, not inconsistency.

An interactive panel also lets you adjust the four measurements by hand
and watch which training flowers "vote" on the resulting species,
visualized on a live scatter plot.

## 🌿 Dataset

Fisher's Iris dataset (1936) — 150 samples, 3 balanced classes
(*Setosa*, *Versicolor*, *Virginica*), 4 numeric features per sample.
The dataset is embedded directly in the page.

## 🛠️ Tech stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Plain HTML, CSS, and JavaScript. No frameworks, no dependencies.

## ✍️ Author

Built by **Faiza Ahmed Esha** as a Project 2(Industrial Training Kit) submission for the
DecodeLabs AI Engineering Internship, Batch 2026.
