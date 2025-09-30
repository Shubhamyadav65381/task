# Road Accident Severity Prediction

This project is an assessment for an online internship. It aims to predict the severity (priority) of road accidents using machine learning models, based on the provided dataset.

## Files

- `Road Accident Data.csv`: The dataset containing accident records and features.
- `task.ipynb`: Jupyter notebook with the complete data analysis, preprocessing, modeling, and prediction workflow.
- `AI Intern Task.pdf`: Assessment instructions .
- `README.md`: Project overview and instructions.

## Workflow

1. **Data Loading & Exploration**
   - Loads the dataset using pandas.
   - Displays basic info, checks for nulls, duplicates, and outliers.
   - Visualizes distributions and relationships using seaborn/matplotlib.

2. **Data Cleaning**
   - Handles missing values and removes duplicates.
   - Removes outliers using Z-score filtering.

3. **Feature Engineering**
   - Encodes categorical features with `LabelEncoder`.
   - Scales numerical features with `StandardScaler`.
   - Renames the target column to `priority`.

4. **Model Training & Evaluation**
   - Splits data into training and test sets.
   - Trains multiple classifiers: Logistic Regression, Random Forest, XGBoost, LightGBM, SVM, CatBoost.
   - Evaluates models using accuracy and F1-score.
   - Selects the best model based on F1-score.

5. **Prediction Function**
   - Implements `predict_priority(input_dict)` to predict accident severity for new data.

6. **Saving the Model**
   - Saves the best model as a `.pkl` file for future use.

## How to Run

1. Open `task.ipynb` in Jupyter Notebook or Google Colab.
2. Ensure all dependencies are installed (see notebook for `%pip install` commands).
3. Run all cells sequentially.
4. Use the `predict_priority` function to predict severity for new accident records.

## Requirements

- Python 3.x
- pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, lightgbm, catboost, joblib

