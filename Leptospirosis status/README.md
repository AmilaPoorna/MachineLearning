## Leptospirosis Status Prediction
This project focuses on predicting the leptospirosis disease status of patients using clinical data. The workflow includes data preprocessing, exploratory data analysis (EDA), and the training of a basic logistic regression model. Final predictions are output to a CSV file called `test_predictions.csv`.

### 🧪 Dataset
The dataset used in this project includes clinical data, collected from multiple hospitals in Sri Lanka. The data is split into training and testing sets, and is accompanied by a data description file called `lepto_description.xls`.

Training Samples: 1387

Test Samples: 347

Response Variable: Final

### 📊 Exploratory Data Analysis
Univariate analysis: Pie charts and histograms were used to understand the distribution of the response variable and predictor variables.

Bivariate analysis: Relationships between variables were visualized using stacked bar plots and box plots.

Multivariate Analysis: A correlation heatmap was used for continuous variables.

### 🧠 Model Training
A basic Logistic Regression classifier was trained using the train set from `train.csv`.

### 📈 Model Evaluation
The model’s performance was assessed using accuracy on the test set from `test.csv`.

Accuracy: **90.49%**
