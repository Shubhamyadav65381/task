# Road Accident Severity Prediction

Predicting the severity of road accidents is crucial for prioritizing emergency response and improving road safety. This project leverages machine learning to classify accident severity (priority) using real-world data and advanced modeling techniques.

## 📁 Project Structure
- `Road Accident Data.csv` — Cleaned dataset of UK road accidents.  
- `task.ipynb` — End-to-end notebook: EDA, preprocessing, modeling, evaluation, and prediction.  
- `README.md` — Project overview and usage guide.  

## 🧑‍💻 What’s Inside
### 1. Data Exploration & Visualization
- Loads and inspects the dataset for missing values, duplicates, and outliers.  
- Visualizes accident severity distribution and relationships with weather, light, and road conditions.  

### 2. Data Cleaning & Preprocessing
- Removes missing values and duplicates.  
- Detects and eliminates outliers using Z-score filtering.  
- Encodes categorical features and scales numerical features for optimal model performance.  

### 3. Feature Engineering
- Renames the target column to `priority` for clarity.  
- Prepares the data for machine learning by encoding and scaling.  

### 4. Model Training & Evaluation
Trains and compares multiple classifiers:
- Logistic Regression  
- Random Forest  
- XGBoost  
- LightGBM  
- SVM  
- CatBoost  

Evaluates models using accuracy and F1-score.  
Visualizes model performance and selects the best model automatically.  

### 5. Prediction API
- Implements a robust `predict_priority(input_dict)` function for real-time predictions on new accident data.  

### 6. Model Export
- Saves the best-performing model as a `.pkl` file for easy deployment.  

## 🚀 Quickstart
1. Clone or Download this repository.  
2. Install dependencies (run in notebook or terminal).  
3. Open `task.ipynb` in Jupyter Notebook or Google Colab.  
4. Run all cells to reproduce the workflow and results.  
5. Predict severity for new data.  

## 📊 Results
- Comprehensive EDA reveals key factors influencing accident severity.  
- Multiple ML models compared; best model selected based on F1-score.  
- Ready-to-use prediction function for real-world applications.  

## 🛠️ Tech Stack
- Python 3.x  
- pandas, numpy, matplotlib, seaborn  
- scikit-learn, xgboost, lightgbm, catboost  
- joblib  

## 💡 Key Learnings
- Data cleaning and outlier removal significantly improve model accuracy.  
- Ensemble models (Random Forest, XGBoost, CatBoost) often outperform linear models for classification tasks.  
- Feature encoding and scaling are essential for robust predictions.  

## 📬 Contact
For questions or collaboration, connect via email - shubham65381@gmail.com.  

---

**Note**: For full details, see the code and comments in `task.ipynb`.  
