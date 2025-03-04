# Project Title: A Dual Approach to Stock Market Analysis: Integrating Machine Learning Forecasting and Regression Discontinuity to Assess the Impact of the Federal Reserve’s COVID-19 Policy Intervention on Investor Sentiment

## Author
- **Yiwei Zhang** - *Brainstorm, Research Design, Data Analysis, Implementation*


## Disclaimer
This project was submitted for **STATS201: Machine Learning for Social Science**  
**Instructor:** Prof. Luyao Zhang  
**Institution:** Duke Kunshan University  
**Semester:** Autumn 2025  

## 🙏 Acknowledgments
We sincerely appreciate the guidance and support from:
- **Prof. Luyao Zhang** for her valuable feedback and mentorship.
- **Classmates** for their constructive discussions and peer reviews.
- **AIGC Tools (e.g., ChatGPT, GitHub Copilot)** for assisting in code generation and debugging.
- **Open-source libraries** including `scikit-learn`, `XGBoost`, `PyCaret`, and `Seaborn` for making this project possible.

## 🚀 Statement of Intellectual and Professional Growth
Throughout this project, we explored **machine learning techniques** in social sciences, particularly in **stock market prediction using investor sentiment analysis**.  
Key takeaways include:
- **Enhancing data preprocessing skills** using real-world financial datasets.
- **Implementing and comparing machine learning models** (Linear Regression, Ridge, XGBoost).
- **Understanding causal inference** using **Regression Discontinuity (RD) Design**.
- **Improving collaboration and version control** through GitHub and project management tools.
This experience has deepened our **statistical modeling expertise** and prepared us for further research in **computational social sciences**.

## 📺 Demo Video & Poster
🎥 **Demo Video:** [Embed or Link to Google Drive/YouTube]  
🖼️ **Project Poster:** [Embed the poster image or link to PDF]  

## 📖 Table of Contents
- [📊 Introduction](#-introduction)
- [📂 Dataset](#-dataset)
- [⚙️ Methodology](#️-methodology)
- [📈 Results](#-results)
- [📌 Key Findings](#-key-findings)
- [🔍 Limitations & Future Work](#-limitations--future-work)
- [📎 References](#-references)
- [👨‍💻 How to Run the Code](#-how-to-run-the-code)
- [📜 License](#-license)

---


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
