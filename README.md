# CS4372-Project-1

Predicting Garment Worker Productivity 

**Dataset**
- We used the Productivity Prediction of Garment Employees dataset from the UCI ML Repository: https://archive.ics.uci.edu/dataset/597/productivity+prediction+of+garment+employees
- The dataset contains production performance of employee teams across two departments (Sewing & Finishing) and four quarterly periods.

**Objective**
The goal of this project was to predict the actual productivity delivered by teams (continuous range from 0 to 1) using metrics such as team composition, time efficiency statistics, department type, and production values.
Additionally, we analyzed which of the 12 teams were most significant for predicting actual productivity.

**Models Used**
SGDRegressor
Linear Regression (OLS)
Random Forest Regressor

Hyperparameter tuning was done manually and with grid/random search methods, and results were logged.

**How to Run**
1. Open the Project_1_code.ipynb notebook in Google Colab (or Jupyter).
2. The dataset is already hosted on GitHub (https://github.com/Sarvesh30/CS4372-Project-1). The notebook reads the data directly from this location, so no local file paths are required.
3. Run cells in the Project_1_code.ipynb notebook as needed

The notebook will: 
- Load and preprocess the dataset (dummy encoding categorical variables, scaling numerical variables).
- Train the models and tune hyperparameters.
- Produce diagnostic outputs, evaluation metrics (R², RMSE), and plots.

**Assumptions**
1. Binary variables (e.g., team, day, quarter, department) were dummy encoded to allow the models to interpret them numerically.
2. Features with extremely skewed distributions were tested in the model although they may have not met the assumptions of normality for linear regression.
