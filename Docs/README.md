# **Documentation of Code Execution, Dependencies, and Example Usage**
To replicate the analysis:
## Code Execution
1 **Clone Repository**  
```bash
 git clone https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final.git
   cd Yiwei_Zhang_Final
```
2 **📌 Create a Virtual Environment (optional bu recommended**
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
3 **Install Dependencies**
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
