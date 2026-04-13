# Titanic - Machine Learning from Disaster

### Project Overview
This repository contains a comprehensive data analysis and preprocessing pipeline for the Titanic survival dataset. The goal is to predict passenger survival based on demographic, socio-economic, and family factors.

### 🧪 Scientific Data Cleaning Approach
Given the complexity of the data, I applied a rigorous cleaning process similar to clinical data management:

* **Advanced Imputation:** Instead of using a simple mean, I imputed missing **Age** values using the **Median Age per Title** (e.g., Mr., Mrs., Master). This ensures a child (Master) isn't assigned the average age of an adult.
* **Feature Encoding:** Converted categorical variables (**Sex**, **Embarked**) into numerical formats for machine learning compatibility.
* **Normalization:** Applied **Log Transformation** (`np.log1p`) to the **Fare** data to handle extreme outliers and normalize the distribution.
* **Handling Nulls:** Resolved `NaN` issues in the Sex and Embarked columns to ensure a 100% complete dataset.

### 📊 Key Visualizations
Included in the Jupyter Notebook are:
* **Correlation Heatmaps:** Identifying Sex and Pclass as the strongest predictors of survival.
* **Distribution Plots:** Visualizing the skewness of ticket fares.
* **Survival Trends:** Analyzing how family size (`Parch`) and port of embarkation impacted survival rates.

### 🛠️ Tech Stack
* **Language:** Python 3
* **Libraries:** Pandas, NumPy, Seaborn, Matplotlib
* **Environment:** Jupyter Notebook
