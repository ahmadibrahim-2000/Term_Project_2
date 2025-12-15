# Term Project 2: Disaster Data Analysis

## Course
This project is part of the 2IS course at UT Capitole.

## Description
This project analyzes disaster data from 1900 to 2021 sourced from EM-DAT (Emergency Events Database). The analysis includes data preprocessing, exploratory data analysis, visualization, and machine learning models to predict economic damages caused by natural disasters.

Key components:
- Data loading and preprocessing
- Handling missing values and inflation adjustment using CPI
- Exploratory data analysis with visualizations
- Regression modeling to predict disaster damages
- Model evaluation and comparison

### Machine Learning Models
The project implements and compares three regression models for predicting economic damages:

1. **Random Forest Regressor**: Achieved high training accuracy (R²: 0.91) but poor generalization (Test R²: 0.13), indicating overfitting.

2. **XGBoost Regressor**: Improved generalization (Test R²: 0.21) compared to Random Forest, with balanced performance.

3. **Tuned XGBoost Regressor**: Optimized using RandomizedSearchCV for hyperparameter tuning, providing the best performance (Test R²: 0.221) with reduced overfitting and stable cross-validation scores (Mean CV R²: 0.447).

Models are evaluated using metrics such as R², MAPE, RMSE, and MAE. The tuned XGBoost model demonstrated the most stable and generalizable results.

## Files
- `1900_2021_DISASTERS_emdat_data.csv`: The dataset containing disaster records.
- `Term_Project_2.ipynb`: Jupyter notebook with the complete analysis and code.

## Requirements
- Python 3.x
- Jupyter Notebook
- Required libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

Install dependencies using:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run
1. Ensure all requirements are installed.
2. Open `Term_Project_2.ipynb` in Jupyter Notebook.
3. Run the cells in order to execute the analysis.

## Data Source
The dataset is from EM-DAT, the International Disaster Database. It includes records of natural disasters worldwide from 1900 to 2021.

## Author
Ahmad Ibrahim

## Repository
[GitHub Repository](https://github.com/ahmadibrahim-2000/Term_Project_2)
