# Car Pricing Data Analysis

This repository contains a comprehensive workflow for analyzing and modeling a car pricing dataset sourced from the UCI Machine Learning Repository. The process includes data preprocessing and cleaning, exploratory data analysis (EDA), important variable selection, model development, and model evaluation.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Data Preprocessing and Cleaning](#data-preprocessing-and-cleaning)
- [Exploratory Data Analysis (EDA) and Important Variables](#exploratory-data-analysis-eda-and-important-variables)
- [Model Development](#model-development)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The aim of this project is to perform a thorough analysis of the car pricing dataset. This includes a step-by-step approach from data preprocessing to model evaluation. The goal is to identify important variables, develop predictive models, and evaluate their performance to understand and predict car prices.

## Dataset

The dataset used in this project is sourced from the UCI Machine Learning Repository. The data can be accessed and downloaded from the following URL:

- [Car Pricing Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.data)

## Installation

pip install pandas numpy matplotlib scikit-learn

## Project Structure
data/

raw/: Contains raw data files.
processed/: Contains processed data files.
notebooks/

1_data_preprocessing_and_cleaning.ipynb: Jupyter notebook for data preprocessing and cleaning.
2_eda_and_important_variables.ipynb: Jupyter notebook for exploratory data analysis and identifying important variables.
3_model_development.ipynb: Jupyter notebook for developing machine learning models.
scripts/

preprocess.py: Script for data preprocessing.
clean.py: Script for data cleaning.
eda.py: Script for exploratory data analysis.
variable_selection.py: Script for selecting important variables.
model.py: Script for developing machine learning models.
evaluate.py: Script for evaluating machine learning models.
results/

eda/: Directory for storing EDA results and visualizations.
models/: Directory for storing trained machine learning models.
evaluation/: Directory for storing model evaluation results.
README.md: Markdown file containing project overview and instructions.

requirements.txt: Text file listing dependencies required to run the project.

LICENSE: File containing details about the project's licensing information.

## Data Preprocessing and Cleaning

The data preprocessing and cleaning process involves several steps to prepare the raw data for analysis:

- Replacing headers
- Replacing "?" with NaN
- Understanding the data
- Dealing with missing values
- Checking the data types
- Data normalization
- Data standardization
- Indicator variable creation (using get_dummies)
- Saving the cleaned data

Details of these steps are provided in the DataPreprocessing and Cleaning.ipynb notebook.

## Exploratory Data Analysis (EDA) and Important Variables

In this phase, we analyze individual feature patterns using visualization techniques. Key analyses include:

- Continuous numerical variables using regplot for:

Engine-size and price
Highway-mpg and price
Peak-rpm and price
Stroke and price

- Categorical variables:

Engine-location vs price
Body-style and price

- Correlation and causation analyses are also performed to understand the relationships between variables.

- The identified important variables for predicting car price include:

Continuous Numerical Variables:

Length
Width
Curb-weight
Engine-size
Horsepower
City-mpg
Highway-mpg
Wheel-base
Bore

Categorical Variable:
Drive-wheels

- Detailed analysis can be found in the EDA_and_ImportantVariables.ipynb notebook.

## Model Development

This phase involves building machine learning models to automate the analysis. We develop both Simple Linear Regression (SLR) and Multiple Linear Regression (MLR) models. After fitting the models, their accuracy is evaluated:

SLR achieved 34% accuracy.
MLR achieved 75% accuracy.

Thus, the MLR model is chosen as the best fit for the data. Details of the model development process are provided in the 3_model_development.ipynb notebook.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
