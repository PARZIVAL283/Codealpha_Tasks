# CodeAlpha Data Science Internship Projects

This repository contains my completed projects for the **CodeAlpha Data Science Internship**. Through these tasks, I practiced data analysis, data visualization, machine learning, model evaluation, and working with real-world datasets using Python.

## Projects Overview

| Task | Project | Type | Main Objective |
|---|---|---|---|
| 1 | Iris Flower Classification | Classification | Predict iris flower species from flower measurements |
| 2 | Unemployment Analysis | Data Analysis | Explore unemployment trends and related indicators in India |
| 3 | Car Price Prediction | Regression | Predict used-car selling prices using car characteristics |

## Technologies Used

- **Python** — programming and analysis
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Seaborn** — statistical visualization
- **Scikit-learn** — machine learning, preprocessing, and evaluation
- **Google Colab** — development environment
- **Git and GitHub** — version control and project hosting

---

## Task 1: Iris Flower Classification

### Overview

The goal of this project was to build a machine learning model that classifies iris flowers into three species based on their physical measurements.

### Dataset

The `Iris.csv` dataset contains 150 records with flower measurements and species labels.

**Features used:**
- Sepal length
- Sepal width
- Petal length
- Petal width

**Target variable:** `Species`

The `Id` column was excluded from the model features.

### Workflow

1. Loaded and inspected the dataset.
2. Checked the dataset structure and missing values.
3. Performed exploratory data analysis and visualization.
4. Separated input features from the target variable.
5. Split the data into training and testing sets.
6. Trained and evaluated multiple classification models.
7. Examined feature importance using Random Forest.

### Models Evaluated

- Random Forest Classifier
- Support Vector Machine (SVM)
- Logistic Regression
- Decision Tree Classifier

### Results

The initial Random Forest model achieved **90.00% test accuracy**.

In the model comparison, the results were:

| Model | Test Accuracy |
|---|---:|
| Support Vector Machine (SVM) | 96.67% |
| Logistic Regression | 93.33% |
| Decision Tree | 93.33% |
| Initial Random Forest | 90.00% |

The SVM achieved the highest test accuracy among these reported results.

The Random Forest feature-importance analysis showed that petal width and petal length were the two most important features in that model.

---

## Task 2: Unemployment Analysis

### Overview

The objective of this project was to analyze unemployment data from India and explore patterns in estimated unemployment rates, employment, and labour-force participation.

### Datasets

Two datasets were used:

- `Unemployment in India.csv`
- `Unemployment_Rate_upto_11_2020.csv`

The first dataset contained 768 rows and 7 columns, including region, date, frequency, estimated unemployment rate, estimated employed population, estimated labour participation rate, and area.

### Workflow

1. Loaded and inspected the datasets using Pandas.
2. Examined the columns, data types, and dataset structure.
3. Prepared the data for analysis.
4. Explored unemployment-related indicators.
5. Used data visualization to investigate patterns and trends.

### Key Learning Outcomes

- Understanding employment and unemployment indicators.
- Working with real-world datasets containing dates and regional information.
- Exploring trends through data analysis and visualization.
- Using Pandas and Matplotlib to communicate findings.

---

## Task 3: Car Price Prediction

### Overview

The objective of this project was to build a regression model that predicts the selling price of a used car based on its characteristics.

### Dataset

The dataset contains information about used cars, including:

- `Car_Name`
- `Year`
- `Selling_Price`
- `Present_Price`
- `Driven_kms`
- `Fuel_Type`
- `Selling_type`
- `Transmission`
- `Owner`

The target variable was `Selling_Price`. A derived feature, `Car_Age`, was created from the manufacturing year.

### Workflow

1. Inspected the dataset and its features.
2. Performed exploratory data analysis and visualizations.
3. Examined relationships between car prices, age, mileage, fuel type, and transmission.
4. Prepared numerical and categorical features.
5. Used imputation and one-hot encoding for preprocessing.
6. Split the data into training and testing sets.
7. Trained and compared regression models.
8. Evaluated predictions using MAE, RMSE, and R².
9. Visualized actual versus predicted prices and model residuals.
10. Examined Random Forest feature importance.
11. Saved the trained model pipeline using Joblib.

### Models Evaluated

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### Evaluation Metrics

- **Mean Absolute Error (MAE):** Measures the average absolute prediction error.
- **Root Mean Squared Error (RMSE):** Gives greater weight to larger prediction errors.
- **R² Score:** Measures how well the model explains variation in selling prices.


---

## Skills Developed

Through these three projects, I gained practical experience in:

- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Data visualization and interpretation
- Classification and regression
- Feature engineering and feature selection
- Training and comparing machine learning models
- Evaluating models using appropriate metrics
- Building Scikit-learn preprocessing pipelines
- Saving trained machine learning models
- Organizing projects for GitHub

## Repository Structure

A suggested structure for organizing the three projects is:

```text
CodeAlpha_Data_Science_Internship/
│
├── README.md
│
├── Task-1-Iris-Flower-Classification/
│   ├── Iris_Classification.ipynb
│   └── Iris.csv
│
├── Task-2-Unemployment-Analysis/
│   ├── Unemployment_Analysis.ipynb
│   ├── Unemployment in India.csv
│   └── Unemployment_Rate_upto_11_2020.csv
│
└── Task-3-Car-Price-Prediction/
    ├── Car_Price_Prediction.ipynb
    └── car_price_prediction_model.pkl
```

*This is a suggested structure; adjust the filenames to match your actual files. Add datasets only when their licenses and sharing terms permit redistribution.*

## Conclusion

Completing these three projects helped me apply data science concepts to different types of problems, from classifying flower species to analyzing unemployment data and predicting used-car prices.

These projects strengthened my understanding of Python-based data analysis, visualization, machine learning, model evaluation, and the process of developing reproducible data science workflows.

## Acknowledgment

I would like to thank **CodeAlpha** for providing the opportunity to work on these data science internship projects and develop practical skills through hands-on tasks.

## Author

**Sourodip Das Gupta**

Data Science Intern — CodeAlpha

GitHub: https://github.com/PARZIVAL283

LinkedIn: www.linkedin.com/in/sourodip-das-gupta-3b97a62a6

---

*This repository documents projects completed for educational and professional development as part of the CodeAlpha Data Science Internship.*
