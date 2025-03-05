# Project Title: Investor Sentiment in Stock Price Forecasting and Policy Analysis: A Machine Learning Approach


## Author
- **Yiwei Zhang** - *Brainstorm, Research Design, Data Analysis, Implementation*


## Disclaimer
This project was submitted for **STATS201: Machine Learning for Social Science**, instructed by **Prof. Luyao Zhang** at Duke Kunshan University in Spring 2025.

## Acknowledgments
I sincerely appreciate the guidance and support from:
- **Prof. Luyao Zhang** for her valuable guidance, feedback and mentorship during the course.
- **Classmates** for their constructive discussions and peer reviews.
- **AIGC Tools (e.g., ChatGPT-4o, Research Rabbit, Storm, Grammarly)** for assisting in literature review, code generation and debugging.
- **Open-source software** Python open source libraries (e.g.,`scikit-learn`, `XGBoost`, `PyCaret`, and `Seaborn`), Whimsical (flowchart design) for making this project possible.

## Statement of Intellectual and Professional Growth
This course has opened a new door for me, introducing two significant aspects of my learning journey. First, I gained a comprehensive understanding of the research design process—from conceptualizing thought experiments and identifying relevant datasets to selecting appropriate machine learning techniques and implementing them through coding. Second, it provided a gateway into machine learning for social sciences, demonstrating how mainstream ML methods—such as explanation, prediction, and causal inference—can be applied to high-quality open-source datasets to drive cutting-edge research.

Throughout the course, I developed foundations research methodlogy design, interdisciplinary problem-solving skills, and GitHub portfolio management, which were crucial in successfully executing this project. This final project experience helped me bridge theory and application by allowing me to explore real-world financial data, compare multiple machine learning models, and critically assess their predictive performance in the context of stock market volatility. This journey has not only strengthened my technical capabilities but also broadened my perspective on how machine learning can be leveraged for impactful research in ground breaking technologies and social sciences.
## Poster
![Final Project Poster](https://github.com/user-attachments/assets/3cfc37fa-73b3-4a63-8059-997b4a473a2c)



## 📖 Table of Contents
- [Introduction](#introduction)
- [Navigation Instructions](#navigation instructions)
- [📊 Datasets and Preprocessing](https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final/blob/main/Data/README.md)
- [📂 Code](https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final/tree/main/Code)
- [⚙️ Visualizations](https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final/tree/main/Visualizations)
- [📈 Research Design Documents](https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final/tree/main/Docs)

---

## 📂 Navigation Instructions

This repository is organized into multiple directories to facilitate **code execution, dataset access, and documentation review**. Below is a guide to navigating the repository:

### 🔹 **1. Code for Simulations and Visualizations**
📍 **Location:** [`/Code`](./Code/)  
This folder contains Jupyter notebooks for **data preprocessing, machine learning predictions, and causal inference analysis**. Key files include:
- `Data Preprocessing & EDA.ipynb` – Prepares and cleans the dataset before modeling.
- `Prediction (1).ipynb` – Implements machine learning models for stock price prediction.
- `Prediction_2_version (1).ipynb` – Integrates sentiment data into stock prediction.
- `Causal_Inference.ipynb` – Conducts regression discontinuity (RD) analysis (detailed in the appendix).

---

### 📂 **2. Datasets and Preprocessing Steps**
📍 **Location:** [`/Data`](./Data/)  
This folder contains all datasets used in this study, including stock prices and sentiment analysis data. Key files include:
- `merged_stock_prices.csv` – The final dataset combining historical stock prices and sentiment scores.
- `train_stockemo.csv` – The raw dataset containing investor sentiment labels.
- `price_raw_data.zip` – Original stock price data before preprocessing.

---

### 📜 **3. Documentation and Dependencies**
📍 **Location:** [`/Docs`](./Docs/)  
This folder provides **project documentation, methodology details, and references**:
- `README.md` – Additional explanations on the project's structure and implementation.
- Dependencies are listed within the Jupyter notebooks (`.ipynb` files), which include required Python packages such as `pycaret`, `scikit-learn`, `pandas`, and `matplotlib`.

📍 **Additional Visualizations:** [`/Visualizations`](./Visualizations/)  
- Contains plots and figures summarizing the results, including final project posters.

---

### 🚀 **How to Get Started**
To replicate the analysis:
1. **Clone this repository**  
   ```sh
   git clone https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final.git
   cd Yiwei_Zhang_Final



# A Dual Approach to Stock Market Analysis: Integrating Machine Learning Forecasting and Regression Discontinuity to Assess the Impact of the Federal Reserve’s COVID-19 Policy Intervention on Investor Sentiment

# 🖥️ System Configuration Instructions

This repository contains the system configuration details, including **CPU, Memory, Disk Space, Python environment, and installed packages**. These specifications ensure compatibility and reproducibility for research and development.

## ⚙️ **System Specifications**
### **CPU Information**
- **Architecture:** x86_64
- **CPU Model:** Intel(R) Xeon(R) CPU @ 2.20GHz
- **Cores:** 1 socket, 2 CPUs, 2 threads per core
- **Virtualization:** Full (KVM)
- **Cache:**
  - **L1:** 32 KiB
  - **L2:** 256 KiB
  - **L3:** 55 MiB

### **Memory Information**
- **Total RAM:** 12 GiB
- **Available:** 11 GiB
- **Swap Memory:** Not enabled

### **Disk Space**
| Filesystem | Size | Used | Available | Usage % |
|------------|------|------|-----------|---------|
| Overlay    | 108G | 32G  | 77G       | 29%     |
| /dev/sda1  | 76G  | 56G  | 21G       | 74%     |

### **GPU Information**
- 🚫 **No GPU detected** (Runs on CPU)

---

## 🐍 **Python Environment**
- **Python Version:** `3.11.11`
- **Package Manager:** `pip`
- **Installed Packages:** (`pip list`)
  
### **📦 Key Installed Packages**
| Package | Version |
|---------|---------|
| `numpy` | 1.26.4 |
| `pandas` | 2.2.2 |
| `scikit-learn` | 1.6.0 |
| `tensorflow` | 2.17.1 |
| `torch` | 2.5.1+cu121 |
| `transformers` | 4.47.1 |
| `matplotlib` | 3.10.0 |
| `seaborn` | 0.13.2 |


---

## 🚀 **How to Use**
### **📌 Setup Environment**
To replicate this system environment, follow these steps:

1️⃣ **Clone Repository**  
```bash
git clone https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_PS2.git
cd Yiwei_Zhang_PS1
```
2️⃣ **📌 Create a Virtual Environment**
A **virtual environment** helps manage dependencies **without affecting global Python installations**.

#### **For Linux & macOS:**
```bash
# Check if Python is installed
python3 --version  

# Install Python if not available
sudo apt install python3 python3-venv python3-pip  # Ubuntu/Debian
brew install python                                # macOS

# Create a virtual environment
python3 -m venv venv  

# Activate the virtual environment
source venv/bin/activate  

# Deactivate when done
deactivate
```
#### **For Windows:**
```bash
# Check if Python is installed
python --version  

# Create a virtual environment
python -m venv venv  

# Activate the virtual environment (PowerShell)
venv\Scripts\Activate.ps1  

# Activate in Command Prompt (cmd.exe)
venv\Scripts\activate  

# Deactivate when done
deactivate
```
3️⃣ **Install Dependencies**
Once the virtual environment is activated, install all required Python packages:

```bash
pip install numpy pandas scikit-learn tensorflow torch transformers matplotlib seaborn \
    requests beautifulsoup4 Flask opencv-python scipy nltk tqdm Pillow \
    PyYAML jsonschema protobuf grpcio google-auth google-auth-oauthlib google-cloud-storage \
    google-cloud-bigquery google-cloud-firestore google-cloud-functions google-cloud-translate \
    google-api-python-client google-auth-httplib2 jupyter jupyterlab notebook ipython \
    ipykernel ipywidgets fastai datasets sentencepiece evaluate tensorboard xgboost \
    plotly openai langchain huggingface-hub fastapi uvicorn typer pydantic rich \
    networkx spacy gensim sympy pytest pylint mypy black isort flake8 autopep8
```
4️⃣ **Verify Installation**
```bash
pip list  
python --version
```
5️⃣ **Running the Project**
```bash
python EDA-2.ipynb
```
