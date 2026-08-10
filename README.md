# Used Car Price Analysis & Prediction in Canada

A machine learning and data analysis project investigating the factors associated with used-car prices in Canada and evaluating regression models for price prediction.

## Project Overview

This project analyzes used-car listings from the US & Canada dataset to investigate how **mileage, vehicle age, make, body type, and province** relate to used-car prices.

The project includes exploratory data analysis (EDA), data cleaning, feature engineering, visualization, and regression modeling. Three approaches were evaluated:

* Simple Linear Regression using mileage as a baseline
* Multiple Linear Regression using multiple vehicle and location features
* A Linear Regression model implemented using gradient descent

The project also compares predicted prices with listed prices to identify potentially undervalued listings by province.

## Key Results

Using the cleaned dataset:

* **Simple Linear Regression:** Test R² ≈ 0.179
* **Multiple Linear Regression:** Test R² ≈ 0.713
* **Gradient Descent:** Test R² ≈ 0.712

The results show that mileage alone is insufficient for predicting used-car prices. Including additional features such as vehicle age, make, body type, and province substantially improved predictive performance.

## Technologies & Tools

* **Python**
* **pandas**
* **NumPy**
* **scikit-learn**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook / Google Colab**
* **Git & GitHub**

## Machine Learning Techniques

* Exploratory Data Analysis
* Data cleaning
* Feature engineering
* One-hot encoding
* Target encoding
* Feature transformation
* Train/test splitting
* Multiple Linear Regression
* Gradient Descent
* Mean Squared Error (MSE)
* R² evaluation
* Model comparison

## Project Structure

```text
Analyzing-and-predicting-used-cars-in-canada/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── Analysing_and_Predicting_Used_Canadian_Car_Prices.ipynb
│
├── figures/
│   ├── good_deals_by_province.png
│   ├── price_v_province.png
│   ├── prices_v_miles.png
│   ├── prices_v_type.png
│   ├── prices_v_year.png
│   └── ...
│
└── report/
    └── Project_Report_Analysing_and_Predicting_Used_Car_Prices_in_Canada.pdf
```

## Dataset

The project uses the **Used Cars Listings for US & Canada** dataset available through Kaggle.

The dataset is **not included in this repository** because its ambiguous about licensing terms.

To reproduce the analysis, obtain the dataset directly from its original source [here]('https://www.kaggle.com/datasets/rupeshraundal/marketcheck-automotive-data-us-canada') and place `used_cars_canada.csv` in the location expected by the notebook.

## Reproducing the Analysis

1. Install the required Python packages:

```bash
pip install -r requirements.txt
```

2. Obtain the dataset from its original source.

3. Open the notebook:

```text
notebooks/Analysing_and_Predicting_Used_Canadian_Car_Prices.ipynb
```

4. Update the dataset path in the notebook if necessary.

5. Run the notebook from beginning to end.

The notebook contains the data-cleaning, exploratory analysis, feature engineering, model training, evaluation, and visualization steps.

## Current Limitations

This project was originally developed as a university course project. The current version focuses primarily on demonstrating the complete data-analysis and regression workflow.

Some limitations include:

* Only a subset of potentially relevant vehicle features was used.
* The models are primarily linear and may not capture nonlinear relationships.
* The original feature-engineering workflow can be improved to prevent potential data leakage during model evaluation.
* Cross-validation was not included in the original analysis.
* The dataset may contain geographic and sampling biases.
* Vehicle condition, accident history, and other potentially important pricing factors were not included.

## Planned Improvements

I am using this repository to iteratively improve the project and strengthen the machine-learning workflow.

Planned improvements include:

* [ ] Refactor preprocessing into a reproducible pipeline
* [ ] Add k-fold cross-validation
* [ ] Improve train/test preprocessing to prevent data leakage
* [ ] Compare additional models such as Random Forest and Gradient Boosting
* [ ] Add hyperparameter tuning
* [ ] Perform feature importance analysis
* [ ] Improve model evaluation and visualization
* [ ] Add automated tests for important preprocessing/modeling steps
* [ ] Explore deployment of the trained model as an API
* [ ] Explore containerization with Docker

These improvements will be added incrementally and documented through GitHub commits.

## Report

The project report contains the detailed research questions, methodology, analysis, results, limitations, and conclusions.

## Academic Project

This project was originally completed as part of a university data analysis course. The repository has been organized and updated as a portfolio project to demonstrate practical experience with Python, data analysis, machine learning, and reproducible project workflows.

## Author

**Dharmrajsinh Gohil**

Bachelor of Science
