# **Documentation of Code Execution, Dependencies, and Example Usage**
To replicate the analysis:
## Code Execution
1 **Clone Repository**  
```bash
 git clone https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final.git
   cd Yiwei_Zhang_Final
```
2 **📌 Create a Virtual Environment (optional but recommended)**
A **virtual environment** helps manage dependencies **without affecting global Python installations**.

#### **For Linux & macOS:**
```bash
# Install Python (if not installed)
sudo apt install python3 python3-venv python3-pip  # Ubuntu/Debian
brew install python                                # macOS

# Create & activate virtual environment
python3 -m venv venv  
source venv/bin/activate  

# Deactivate when done
deactivate
```
#### **For Windows:**
```bash
# Check Python installation
python --version  

# Create & activate virtual environment
python -m venv venv  
venv\Scripts\activate  # Command Prompt  
venv\Scripts\Activate.ps1  # PowerShell  

# Deactivate when done
deactivate
```
3 **Install Dependencies**
Once the virtual environment is activated, install all required Python packages:

```bash
pip install -r requirements.txt
```
4 **Navigate to Code Directory**
```bash
cd Code
python --version
```
5 **Run the Code**
```bash

python --version
```

## Dependencies

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

---

**Installation**  
Run the following command to install all dependencies:  
```sh
pip install -r requirements.txt
```
## Example Usage
### 1. Running Stock Price Prediction (Baseline Model):  
- To forecast stock prices using historical data only, run the following notebook:  

```sh
jupyter notebook Prediction (1).ipynb
```
### 2. Running Sentiment-Enhanced Prediction:
- To integrate investor sentiment scores into stock price forecasting, run:
```sh
jupyter notebook Prediction_2_version (1).ipynb
```
### 3. Running Causal Inference Analysis:
- To perform Regression Discontinuity (RD) analysis on the impact of Federal Reserve’s COVID-19 intervention, run:
```sh
jupyter notebook Causal_Inference.ipynb
```
