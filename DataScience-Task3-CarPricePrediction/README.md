# Car Price Prediction

**Oasis Infobyte Data Science Internship — Task 3**

## Project Overview

This project develops a machine-learning regression system to estimate the selling price of a used car from its characteristics. It demonstrates an end-to-end data science workflow, from data cleaning and exploratory data analysis to model training, evaluation, and interpretation.

## Objectives

- Inspect and clean a real-world used-car dataset.
- Explore selling prices and vehicle characteristics through visualizations.
- Engineer useful features, including vehicle brand and car age.
- Handle missing values and categorical variables using a reusable preprocessing pipeline.
- Train and compare multiple regression models.
- Evaluate predictions using MAE, RMSE, and R².
- Examine prediction errors and feature importance.

## Dataset

The project uses the CarDekho used-car dataset distributed through this public repository:

[Car details dataset — GitHub source](https://raw.githubusercontent.com/HarshKapadia2/car-details/main/data/car_details_v3.csv)

The dataset includes fields such as vehicle name, year, selling price, kilometres driven, fuel type, seller type, transmission, ownership history, mileage, engine size, maximum power, torque, and seating capacity.

The notebook cleans the data and extracts numeric values from specification fields containing units. It also derives the vehicle brand and car age. The `torque` column is excluded from modeling because its formats are inconsistent.

## Project Structure

```text
DataScience-Task3-CarPricePrediction/
├── Car_Price_Prediction.ipynb
├── README.md
├── requirements.txt
├── model_metrics.csv
├── data/
│   └── car_details_v3.csv
└── screenshots/
    ├── selling_price_distribution.png
    ├── car_age_distribution.png
    ├── median_price_by_fuel.png
    ├── km_driven_vs_price.png
    ├── model_comparison_mae.png
    ├── actual_vs_predicted.png
    ├── residual_distribution.png
    └── feature_importance.png
```

The feature-importance image is generated when the selected model supports tree-based feature importance. The exact files available may therefore vary.

## Workflow

1. **Data loading and inspection:** Review the dataset dimensions, data types, missing values, and duplicate records.
2. **Data cleaning:** Remove exact duplicate records and records with invalid target prices; convert vehicle specifications to numeric values where appropriate.
3. **Feature engineering:** Derive the vehicle brand and calculate car age using 2026 as the reference year.
4. **Exploratory data analysis:** Visualize price distribution, car age, median price by fuel type, and kilometres driven versus price.
5. **Preprocessing:** Impute missing numeric values using the median, impute missing categorical values using the most frequent category, and one-hot encode categorical features.
6. **Model training:** Compare a median baseline, Linear Regression, Random Forest Regressor, and Extra Trees Regressor.
7. **Evaluation:** Compare models on a held-out test set and select the model with the lowest test MAE.
8. **Interpretation:** Inspect actual versus predicted prices, residuals, feature importance where supported, and sample predictions.

## Models and Evaluation Metrics

| Model | Purpose |
|---|---|
| Median Baseline | Establishes a simple reference performance |
| Linear Regression | Provides a linear regression benchmark |
| Random Forest Regressor | Learns nonlinear patterns using an ensemble of decision trees |
| Extra Trees Regressor | Provides an alternative randomized tree ensemble |

The notebook reports these metrics:

- **MAE:** Mean Absolute Error; lower is better.
- **RMSE:** Root Mean Squared Error; lower is better.
- **R²:** Coefficient of determination; higher is generally better.

The actual comparison results are saved to `model_metrics.csv` when the notebook runs. Results are not hard-coded in this README because they depend on the data and execution environment.

## How to Run

1. Clone or download this repository.
2. Open the `DataScience-Task3-CarPricePrediction` folder.
3. Ensure `data/car_details_v3.csv` is present.
4. Install the required packages.
5. Launch Jupyter Notebook from this project folder.
6. Open `Car_Price_Prediction.ipynb`.
7. Select **Restart Kernel and Run All Cells**.
8. Review the notebook outputs, `model_metrics.csv`, and charts saved under `screenshots/`.

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Results and Outputs

Running the notebook produces:

- Exploratory data analysis charts.
- A comparison table of regression models.
- MAE, RMSE, and R² evaluation metrics.
- Actual-versus-predicted and residual visualizations.
- Feature-importance analysis when supported by the selected model.
- A CSV file containing model comparison metrics.

The model selected for further inspection is the one with the lowest MAE on the held-out test set. Consult the notebook output and `model_metrics.csv` for the actual results from this run.

## Limitations

- The dataset may not represent current prices or every used-car market.
- Evaluation uses a random train/test split rather than a time-based split.
- Outliers, missing specifications, and inconsistent listings can affect model performance.
- Brand is extracted from the first word of the vehicle name, which may not always identify a manufacturer perfectly.
- Feature importance does not establish causation.
- Predicted prices are estimates, not guaranteed market valuations.

## Conclusion

This project demonstrates a complete supervised regression workflow, including data preparation, feature engineering, visualization, reusable preprocessing, model comparison, and evaluation. It provides practical experience with common Python data science and machine-learning tools.

## Tools and Technologies

- Python
- Jupyter Notebook
- pandas and NumPy
- Matplotlib and Seaborn
- scikit-learn
- Git and GitHub

---

**Internship:** Oasis Infobyte Data Science Internship  
**Task:** Task 3 — Car Price Prediction