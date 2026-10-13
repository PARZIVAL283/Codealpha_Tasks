# Iris Flower Classification 🌸

A machine learning project developed as part of the **CodeAlpha Data Science Internship**. The project uses flower measurements to classify iris flowers into three species and compares multiple classification algorithms.

## Project Overview

The goal is to predict an iris flower's species from four numerical measurements:

- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

The dataset contains **150 samples** and three target classes: `Iris-setosa`, `Iris-versicolor`, and `Iris-virginica`.

## Dataset

The dataset used in this project is `Iris.csv`.

| Column | Description |
|---|---|
| `Id` | Record identifier; excluded from model inputs |
| `SepalLengthCm` | Sepal length in centimeters |
| `SepalWidthCm` | Sepal width in centimeters |
| `PetalLengthCm` | Petal length in centimeters |
| `PetalWidthCm` | Petal width in centimeters |
| `Species` | Target species label |

The initial inspection found no missing values. The `Id` column was excluded because it is an identifier rather than a flower measurement.

## Tools and Libraries

- Python
- Google Colab / Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Workflow

1. Load and inspect the dataset.
2. Check data types, missing values, and class distribution.
3. Explore numerical features with summary statistics and visualizations.
4. Separate the four measurement features (`X`) from the target labels (`y`).
5. Split the data into training and testing sets using an 80/20 split, with `random_state=42` and stratification by species.
6. Train and evaluate classification models.
7. Compare performance using accuracy, macro precision, macro recall, and macro F1-score.
8. Inspect Random Forest feature importance and visualize a confusion matrix.

## Models Compared

Four classification approaches were evaluated on the same train-test split:

- Support Vector Machine (SVM), with feature standardization
- Logistic Regression, with feature standardization
- Decision Tree
- Random Forest

## Results

The following results were obtained from the project's current evaluation run:

| Model | Accuracy | Macro Precision | Macro Recall | Macro F1-score |
|---|---:|---:|---:|---:|
| SVM | 96.67% | 96.97% | 96.67% | 96.66% |
| Logistic Regression | 93.33% | 93.33% | 93.33% | 93.33% |
| Decision Tree | 93.33% | 93.33% | 93.33% | 93.33% |
| Random Forest | 90.00% | 90.24% | 90.00% | 89.97% |

**Best result in this run:** SVM achieved 96.67% accuracy and a macro F1-score of 96.66%.

These scores are specific to one 80/20 train-test split of a small dataset. They should not be interpreted as a guarantee of performance on every unseen dataset. For a more robust model-selection process, cross-validation on the training data is recommended before a final evaluation on a held-out test set.

### Random Forest Feature Importance

The Random Forest model reported these feature-importance scores:

| Feature | Importance |
|---|---:|
| Petal width | 0.437185 |
| Petal length | 0.431466 |
| Sepal length | 0.116349 |
| Sepal width | 0.015000 |

In this model, petal width and petal length had the highest feature-importance scores. These values describe how the Random Forest used the features; they do not establish causation.

## How to Run

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload or open the project notebook.
3. Upload `Iris.csv` to the Colab session if the notebook reads the CSV from session storage.
4. Run the notebook cells in order.

### Option 2: Run Locally

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas matplotlib seaborn scikit-learn jupyter
   ```

3. Place `Iris.csv` in the location expected by the notebook, or update the file path in the code.
4. Open and run the notebook:

   ```bash
   jupyter notebook
   ```

## Repository Structure

```text
CodeAlpha_Iris_Flower_Classification/
├── README.md
├── Iris.csv
└── CodeAlpha_Iris_Flower_Classification.ipynb
```

Adjust the filenames in this structure to match the files you actually upload. Do not include the dataset if its license or source terms do not permit redistribution.

## Key Learnings

- Loading and inspecting a real tabular dataset
- Exploratory data analysis and data visualization
- Separating features from target labels
- Train-test splitting and stratified sampling
- Training classification models with Scikit-learn
- Evaluating models with accuracy, precision, recall, F1-score, and a confusion matrix
- Comparing algorithms and interpreting feature importance

## Future Improvements

- Use stratified cross-validation to compare models more robustly.
- Tune model hyperparameters using training data only.
- Evaluate the selected model on a held-out test set after model selection.
- Add a simple interface for entering flower measurements and viewing predictions.
- Document the dataset source and license.

## Internship Context

This project was completed as part of the **CodeAlpha Data Science Internship**.

## Author

**Sourodip Das Gupta**

---

*This project is intended for learning and demonstration. Reported metrics reflect the evaluation run described above.*
