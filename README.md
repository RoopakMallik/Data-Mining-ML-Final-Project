# Data Mining, Analytics and Machine Learning Project

## Overview
This project applies exploratory data analysis (EDA) and machine learning techniques to two datasets:
- A healthcare dataset from the Open Payments program.
- A cryptocurrency dataset of Bitcoin prices fetched via the Binance API.

The goal is to analyze payment patterns in the healthcare data and predict Bitcoin prices using the cryptocurrency data.

## Datasets
- **Healthcare Dataset**:  
  A 15,000-row subset of the Open Payments data, detailing payments from drug and medical device companies to physicians and hospitals.  
  - Source: [Open Payments Dataset](https://openpaymentsdata.cms.gov/dataset/fb3a65aa-c901-4a38-a813-b04b00dfa2a9) (subset included in repository).

- **Cryptocurrency Dataset**:  
  Hourly Bitcoin price data from January 1, 2023, to April 1, 2025, fetched using the Binance API.  
  - Note: Data is pre-fetched and included in the repository; no API access is required to run the project.

## Prerequisites
To run this project, ensure you have:
- **Python 3.8+** installed.
- The following Python libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `xgboost`
  - `TA-Lib`
  - `binance` (optional, only if fetching new data)

Install the dependencies using:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost binance
```

## Setup Instructions
Follow these steps to set up and run the project:

1. **Clone the Repository**:  
   Download the project files to your local machine.
   ```bash
   git clone https://github.com/RoopakMallik/Data-Mining-ML-Final-Project.git
   ```

2. **Navigate to the Project Directory**:  
   Enter the project folder.
   ```bash
   cd Data-Mining-ML-Final-Project
   ```

3. **Open the Jupyter Notebooks**:  
   Launch the notebooks for analysis:
   - Healthcare dataset: `Dataset_1_ML_Models.ipynb`
   - Cryptocurrency dataset: `Dataset_2_ML_Models.ipynb`
   ```bash
   jupyter notebook
   ```

4. **Run the Notebooks**:  
   Open each notebook in Jupyter and execute the cells step-by-step to perform EDA and machine learning tasks.

## Project Structure
- **`Dataset_1_ML_Models.ipynb`**:  
  - **EDA**: Data cleaning, visualization, and statistical analysis of healthcare payments.
  - **Machine Learning**: Applies Random Forest and XGBoost to classify payment amounts.

- **`Dataset_2_ML_Models.ipynb`**:  
  - **EDA**: Time series visualization and feature engineering for Bitcoin price data.
  - **Machine Learning**: Uses Linear Regression and Decision Tree Regressor to predict Bitcoin prices.

- **`Data_Collection.ipynb`**:  
  - Script to fetch Bitcoin data using the Binance API (data is already included, no need to run unless updating).

## Running the Analysis
1. **Healthcare Analysis**:  
   - Open `Dataset_1_ML_Models.ipynb`.
   - Run all cells to clean data, visualize patterns, and train models.
   - Key features analyzed include payment type and recipient specialty.

2. **Cryptocurrency Analysis**:  
   - Open `Dataset_2_ML_Models.ipynb`.
   - Execute cells to visualize trends and predict Bitcoin prices.
   - Features engineered include time-based metrics from price data.

## Results
- **Healthcare**:  
  - Random Forest outperformed XGBoost in predicting payment amounts, with key predictors being payment type and specialty.
- **Cryptocurrency**:  
  - Decision Tree Regressor showed better performance than Linear Regression for Bitcoin price prediction.

## Challenges
- **Healthcare**: Managed large dataset size by using a subset.
- **Cryptocurrency**: Addressed time series complexity through feature engineering.
