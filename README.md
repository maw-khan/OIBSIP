# Oasis Infobyte — Data Science Internship Projects

**A collection of three Python and machine-learning projects completed as part of the Oasis Infobyte (OIBSIP) Data Science Internship.**

## Overview

This repository brings together three practical projects covering classification, regression, and natural-language processing. Each project has its own folder containing its notebook and task-specific README.

The projects demonstrate a practical data-science workflow, including data inspection, preprocessing, exploratory data analysis, feature engineering, model development, evaluation, and prediction.

## Projects

### 1. Iris Flower Classification

**Project folder:** [`DataScience-Task1-IrisFlowerClassification/`](./DataScience-Task1-IrisFlowerClassification/)

A classification project that predicts an Iris flower species based on its numerical measurements.

- **Problem type:** Supervised classification
- **Models:** Logistic Regression, K-Nearest Neighbors (KNN), Random Forest
- **Key work:** Data inspection, feature preparation, scaling where appropriate, model training, and performance comparison
- **Technologies:** Python, pandas, scikit-learn, Matplotlib, Seaborn

### 2. Car Price Prediction

**Project folder:** [`DataScience-Task3-CarPricePrediction/`](./DataScience-Task3-CarPricePrediction/)

A regression project that estimates vehicle prices from available car attributes.

- **Problem type:** Supervised regression
- **Models:** Linear Regression, Random Forest Regressor, Extra Trees Regressor
- **Key work:** Data cleaning, exploratory data analysis, feature engineering, model training, and error analysis
- **Evaluation metrics:** Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), R²
- **Technologies:** Python, pandas, NumPy, scikit-learn, Matplotlib, Seaborn

### 3. SMS / Email Spam Detection

**Project folder:** [`DataScience-Task4-EmailSpamDetection/`](./DataScience-Task4-EmailSpamDetection/)

A text-classification project that identifies messages as spam or legitimate (ham) using machine-learning techniques. The implementation uses an SMS-message dataset.

- **Problem type:** Text classification / Natural Language Processing (NLP)
- **Models:** Multinomial Naive Bayes, Logistic Regression, Linear Support Vector Classifier
- **Key work:** Text data inspection, TF-IDF feature extraction, model training, performance comparison, and predictions on new messages
- **Evaluation metrics:** Accuracy, precision, recall, F1-score, classification report, and confusion matrix
- **Technologies:** Python, pandas, scikit-learn, Matplotlib, Seaborn, Joblib

## Repository Structure

```text
OIBSIP/
├── DataScience-Task1-IrisFlowerClassification/
│   └── Notebook and project-specific README
├── DataScience-Task3-CarPricePrediction/
│   └── Notebook, supporting outputs, and project-specific README
├── DataScience-Task4-EmailSpamDetection/
│   └── Notebook and project-specific README
└── README.md
```

Each project folder contains its own README with more detailed implementation information, dataset notes, and setup instructions.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming language | Python |
| Data manipulation | pandas, NumPy |
| Machine learning | scikit-learn |
| Text feature extraction | TF-IDF |
| Data visualization | Matplotlib, Seaborn |
| Model persistence | Joblib |
| Development environment | Jupyter Notebook, VS Code |
| Version control | Git, GitHub |

## General Workflow

1. **Data inspection:** Understand the dataset, features, labels, and data quality.
2. **Data preparation:** Perform relevant cleaning and preprocessing.
3. **Exploratory analysis:** Investigate distributions and relationships in the data.
4. **Feature engineering:** Prepare useful model inputs where appropriate.
5. **Model development:** Train suitable algorithms for each problem.
6. **Evaluation:** Compare models using relevant classification or regression metrics.
7. **Prediction:** Test the trained models on examples and save reusable artifacts where included.

The specific workflow varies by project and is documented in its corresponding folder.

## Getting Started

### Prerequisites

- Python
- Jupyter Notebook or VS Code with the Python and Jupyter extensions
- Git (for cloning the repository)

### Run a project locally

Clone the repository:

```bash
git clone https://github.com/maw-khan/OIBSIP.git
cd OIBSIP
```

Then:

1. Open the folder of the project you want to run.
2. Read its `README.md` for project-specific instructions.
3. If a `requirements.txt` file is provided, install the dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Open the notebook, select the appropriate Python kernel, and execute the cells in order.

Some notebooks download datasets at runtime and may require an internet connection.

## Notes on Results

Model performance depends on the dataset, preprocessing choices, train/test split, and model configuration. Results should not be interpreted as a guarantee of performance on unseen real-world data. Consult each project's notebook and README for its specific evaluation results.

## Internship Information

- **Organization:** Oasis Infobyte
- **Program:** Data Science Internship
- **Repository:** [maw-khan/OIBSIP](https://github.com/maw-khan/OIBSIP)

## Author

**Muhammad Ali Waris Khan**  
[GitHub Profile](https://github.com/maw-khan)

---

*This repository documents practical work in data preparation, machine learning, model evaluation, and notebook-based workflows completed during the internship.*
