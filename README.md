# 🌸 IrisSort

> A supervised learning pipeline that classifies Iris flowers by species, built as a Python notebook, then reimplemented as a dependency-free interactive site.

## 📖 About

IrisSort classifies Iris flowers into one of three species (*Setosa*, *Versicolor*, *Virginica*) using their sepal and petal measurements. It was built as **Project 2: Data Classification Using AI** for the DecodeLabs AI Engineering Internship, Batch 2026.

The repo contains two things:

- **`Iris_Classification__Project2_.ipynb`** — the actual assignment: a Python notebook covering the full supervised learning pipeline (load → explore → split → scale → train → evaluate) using scikit-learn.
- **`index.html`** — a self-contained, dependency-free reimplementation of the same KNN pipeline in plain JavaScript, built afterward as an interactive extension so the same logic can be explored live in a browser.

## ✦ Highlights

- 📊 **Full ML pipeline** — EDA, feature scaling, stratified train/test split, KNN classification
- 🔍 **K exploration** — tests K = 1 to 20 and plots the error curve instead of assuming K = 5
- 📈 **Evaluation** — accuracy, weighted F1, confusion matrix, full classification report
- 🌱 **Custom prediction** — tests the trained model on a hand-picked flower outside the dataset
- 🖱️ **Interactive site** — sliders to build your own flower and watch live KNN voting on a scatter plot

## 🛠️ Built With

- **Python** — pandas, NumPy, scikit-learn, Matplotlib *(notebook)*
- **HTML / CSS / JavaScript** — no frameworks, no dependencies *(interactive site)*

## ⚙️ How It Works

**Load Iris dataset → EDA → Standardize features → Stratified 80/20 split → K-Nearest Neighbors (K = 5) → Evaluate on held-out test set**

Both the notebook and the site follow this exact pipeline — the site simply re-derives it in the browser instead of relying on scikit-learn, so its accuracy naturally varies slightly on each reload since it reshuffles the split live.

## 🚀 Getting Started

### Run the notebook

1. Clone the repo:
   ```
   git clone https://github.com/FaizaEsha/IrisSort.git
   ```
2. Open `Iris_Classification__Project2_.ipynb` in Jupyter Notebook, JupyterLab, or upload it to Google Colab.
3. Run all cells top to bottom.

No dataset download needed — the Iris dataset loads directly from scikit-learn.

### Run the interactive site

**Locally:** download `index.html` and open it directly in any browser — no install, no build step.

## 📁 Project Structure

```
├── Iris_Classification__Project2_.ipynb   # Python notebook — the core assignment
├── index.html                              # Interactive browser version (JS, no dependencies)
└── README.md
```

## ✍️ Author

**Faiza Ahmed Esha**
DecodeLabs AI Engineering Internship, Batch 2026
