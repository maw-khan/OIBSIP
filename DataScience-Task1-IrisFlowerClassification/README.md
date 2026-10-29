# Iris Flower Classification Using Machine Learning

## Project Overview

This project applies supervised machine learning to classify iris flowers into three species: Setosa, Versicolor, and Virginica. Predictions are based on four numerical measurements: sepal length, sepal width, petal length, and petal width.

The project was developed as part of the Oasis Infobyte Data Science Internship.

## Objectives

- Explore and analyze the Iris dataset.
- Visualize feature distributions and relationships between species.
- Prepare the data for machine learning.
- Train and compare multiple classification algorithms.
- Evaluate model performance using appropriate classification metrics.
- Identify the best-performing model based on test-set results.

## Dataset

The project uses the built-in Iris dataset provided by Scikit-learn, so no external dataset download is required.

- **Observations:** 150
- **Input features:** 4 numerical measurements
- **Target classes:** 3 iris species
- **Training data:** 80%
- **Testing data:** 20%

## Technologies Used

- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn

## Project Workflow

1. Import libraries and load the dataset.
2. Inspect the dataset structure, data types, missing values, and duplicates.
3. Perform exploratory data analysis and descriptive statistical analysis.
4. Visualize feature distributions, pairwise relationships, and differences between species.
5. Split the dataset into training and testing subsets using stratified sampling.
6. Train Logistic Regression, K-Nearest Neighbors, and Random Forest classifiers.
7. Evaluate and compare the models using accuracy, precision, recall, F1-score, and confusion matrices.
8. Analyze Random Forest feature importance and summarize the findings.

## Model Evaluation

The models were evaluated on the same held-out test set of 30 observations.

| Model | Test Accuracy | Macro F1-Score |
|---|---:|---:|
| Logistic Regression | 93.33% | 93.33% |
| K-Nearest Neighbors | 93.33% | 93.27% |
| Random Forest | 90.00% | 89.97% |

Logistic Regression was selected as the preferred model because it achieved the joint-highest test accuracy and the highest macro F1-score among the three evaluated classifiers.

These results reflect a single train/test split and should not be interpreted as a guarantee of performance on other datasets or splits.

## Repository Contents

- `Iris_Flower_Classification.ipynb` — Complete analysis, visualizations, model training, and evaluation.
- `requirements.txt` — Required Python packages.
- `screenshots/` — Selected project visualizations and results.

## How to Run the Project

1. Clone or download this repository folder.
2. Create and activate a Python virtual environment.
3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `Iris_Flower_Classification.ipynb` and run the cells in order.

## Conclusion

This project demonstrates an end-to-end introductory machine learning workflow, including exploratory data analysis, visualization, classification, model evaluation, and interpretation.

The comparison showed that Logistic Regression and K-Nearest Neighbors performed best in terms of test accuracy, with Logistic Regression selected based on its macro F1-score.

## Author

GitHub: [maw-khan](https://github.com/maw-khan)

**Program:** Oasis Infobyte Data Science Internship
