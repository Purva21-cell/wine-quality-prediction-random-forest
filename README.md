#  Wine Quality Prediction Using Random Forest Regression

##  Project Overview

This project focuses on predicting red wine quality using Machine Learning and Random Forest Regression.

The model uses physicochemical properties of wine, such as acidity, alcohol content, density, sulphates, and other chemical characteristics, to predict wine quality scores.

The project uses the **UCI Wine Quality Dataset** and implements a complete machine-learning workflow, from data preprocessing to model training, evaluation, visualization, and model deployment preparation.

##  Project Objectives

- Load and explore the UCI Wine Quality Dataset.
- Perform data cleaning and preprocessing.
- Handle missing values using median imputation.
- Apply feature scaling using StandardScaler.
- Train a Random Forest Regression model.
- Evaluate model performance using RMSE, MAE, and R².
- Extract and visualize feature importance.
- Save the trained model using Joblib.
- Load the saved model for future predictions.

##  Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Jupyter Notebook | Development environment |
| Pandas | Data manipulation |
| NumPy | Numerical computations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine Learning |
| Joblib | Model serialization |

##  Dataset Information

**Dataset:** UCI Wine Quality Dataset (Red Wine)

**Source:** [UCI Machine Learning Repository – Wine Quality Dataset](https://archive.ics.uci.edu/dataset/186/wine+quality)

The dataset contains 1,599 red wine samples with 11 physicochemical input features and one target variable.

### Input Features

1. Fixed Acidity
2. Volatile Acidity
3. Citric Acid
4. Residual Sugar
5. Chlorides
6. Free Sulfur Dioxide
7. Total Sulfur Dioxide
8. Density
9. pH
10. Sulphates
11. Alcohol

**Target Variable:** Quality

The target variable represents the wine quality score.

##  Project Workflow

### 1. Data Loading
Load the UCI Red Wine Quality dataset using Pandas.

### 2. Data Cleaning
- Remove duplicate records.
- Convert columns into numeric format.
- Handle infinite values.
- Remove records with missing target values.
- Handle missing feature values using median imputation.

### 3. Feature Scaling
Apply StandardScaler to standardize numerical input features.

### 4. Model Training
Train a RandomForestRegressor using the training dataset.

Model configuration:
- Number of estimators: 300
- Random state: 42
- Maximum depth: None
- Minimum samples split: 2
- Minimum samples leaf: 1

### 5. Model Evaluation
Evaluate the trained model using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

### 6. Feature Importance
Extract feature importance from the trained Random Forest model and visualize the contribution of each input feature using a bar chart.

### 7. Model Saving
Save the complete preprocessing and trained model pipeline using Joblib for future inference.

##  Visualizations

The project includes:

- Actual vs. Predicted Wine Quality Scatter Plot.
- Random Forest Feature Importance Bar Chart.

These visualizations help understand model performance and the relative importance of different wine characteristics.

*The trained model file is generated after executing the notebook.*

##  Installation and Execution

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/wine-quality-prediction-random-forest.git
```

### Step 2: Navigate to the Project Directory

```bash
cd wine-quality-prediction-random-forest
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Project

Open `Wine_Quality_Prediction.ipynb` and execute all cells sequentially.

The notebook will load the dataset, preprocess the data, train the model, evaluate performance, generate visualizations, and save the trained model.

##  Model Output

The trained model is saved as:

`wine_quality_random_forest.joblib`

The saved pipeline includes preprocessing and the Random Forest regression model, allowing new wine samples to be passed through the same preprocessing steps before prediction.

##  Expected Results

After successful execution, the notebook generates:

- Cleaned and processed dataset.
- Training and testing datasets.
- Random Forest regression model.
- RMSE, MAE, and R² evaluation results.
- Actual vs. predicted visualization.
- Feature importance visualization.
- Saved machine-learning model.

*Actual evaluation scores are generated during execution and depend on the dataset and model configuration.*

##  Future Improvements

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Cross-validation for more reliable model evaluation.
- Compare Random Forest with other regression algorithms.
- Develop an interactive web application using Streamlit.
- Deploy the trained model for real-time predictions.

##  Author

**Purva Pankaj Ghate**

Electronics and Telecommunication Engineering Student

##  License

This project is intended for educational and learning purposes. Dataset usage is subject to the terms provided by the UCI Machine Learning Repository.
