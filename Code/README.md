## **📁 Code Folder Structure**  
This repository contains **Jupyter Notebooks** for research on **causal inference, exploratory data analysis (EDA), social network analysis, and predictive modeling**.

| **File/Folder** | **Description** |
|----------------|----------------|
| `Causal_Inference.ipynb` | Implements **Regression Discontinuity (RD) Design** and other causal inference methods. |
| `Data Preprocessing & EDA.ipynb` | Performs **data cleaning, feature engineering, and exploratory data analysis**. |
| `Machine_Learning_for_Explanations_for_Literature_Review.ipynb` | Uses automated Literature Review using arXiv API!|
| `Prediction (1).ipynb` | Builds **predictive models** for forecasting basad solely on historical price data. |
| `Prediction_2_version_(1).ipynb` | Builds **predictive models** for forecasting based on both sentiment data and historical price data. |
| `README.md` | This documentation file. |

---


## **🚀 How to Use This Repository**
### **🔹 Clone the Repository**
```bash
git clone https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final
```


## **📌 Prerequisites**

### **🔹 Required Libraries**
This repository requires **Python 3.9+** and the following key libraries:

**pandas==2.2.2**  
**numpy==1.26.4**  
**scikit-learn==1.6.1**  
**pycaret==3.0.0**  
**xgboost==2.1.4**  
**lightgbm==4.5.0**  
**matplotlib==3.10.0**  
**seaborn==0.13.2**  
**nltk==3.9.1**  
**transformers==4.48.3**  
**jupyter==1.0.0**  
**notebook==6.5.5**  

## Usage Instruction
Step-by-Step Guide on Running Each Notebook

1️⃣ Loading Datasets
To load datasets, you can use the following Python code:
```bash
python
import pandas as pd
df = pd.read_csv("dataset.csv")
If you are using Google Colab, you can upload files with:
```bash

from google.colab import files
uploaded = files.upload()
```
2️⃣ Running NLP or Social Network Analysis
For NLP tasks using transformer-based models like BERT, ensure you have the transformers library installed. Here’s an example for sentiment analysis:

python
```bash
from transformers import pipeline
sentiment_pipeline = pipeline("sentiment-analysis")
result = sentiment_pipeline("The market is very volatile today!")
print(result)
```
3️⃣ Training & Evaluating Predictive Models
To train a predictive model, such as a Random Forest Classifier, follow these steps:
python
```bash
from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
```

Evaluate model performance
```bash
from sklearn.metrics import accuracy_score
print(f"Accuracy: {accuracy_score(y_test, y_pred)}")
```
4️⃣ Running Causal Inference (RD Design)
Perform Regression Discontinuity Analysis using the following code:

python
```bash
from rdrobust import rdrobust
rd_results = rdrobust(Y, X, c=0)
print(rd_results)
```

Visualize RD Discontinuity Plot
```bash
import matplotlib.pyplot as plt
plt.scatter(X, Y, alpha=0.5)
plt.axvline(0, color='red', linestyle='--', label='Cutoff')
plt.xlabel("Running Variable (Days from Cutoff)")
plt.ylabel("Outcome Variable (Sentiment Score)")
plt.title("Regression Discontinuity Analysis")
plt.legend()
plt.show()
```
# Expected Outcome
Data Preprocessing & EDA	Summary statistics, missing values analysis, and visualizations of distributions.

Machine Learning Model Training	Model accuracy, precision-recall scores, feature importance plots.

Regression Discontinuity Analysis	Estimated treatment effect (β1), RD plots, p-values for significance testing.

# Contributors
Yiwei Zhang, Lead Researcher, Causal Inference & Prediction & Explanation & Data Preprocessing

