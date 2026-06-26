# 🤖 AI Multi-Agent Data Cleaning System

An intelligent multi-agent data cleaning pipeline built using **LangGraph**, **LangChain**, **Groq Llama 3.1**, and **Pandas**. The system automatically profiles datasets, detects data quality issues, generates cleaning code using an LLM, executes the code, validates the results, and iteratively improves the dataset.

---

## 📌 Project Overview

Data cleaning is one of the most time-consuming stages of any data science workflow. This project automates the process by orchestrating multiple AI agents, each responsible for a specific task in the cleaning pipeline.

The system follows a structured workflow:

1. Profile the dataset
2. Detect anomalies and data quality issues
3. Generate Python cleaning code using an LLM
4. Execute the generated code
5. Validate the cleaned dataset
6. Repeat until no significant issues remain

---

## 🚀 Features

- Automated dataset profiling
- Missing value detection
- Duplicate record detection
- Data type analysis
- AI-generated cleaning code
- Automatic code execution
- Iterative validation loop
- Multi-agent workflow using LangGraph
- Saves cleaned dataset automatically

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- LangChain
- LangGraph
- Groq API
- Llama 3.1
- Jupyter Notebook

---

## 🏗️ System Architecture

```
Raw CSV
   │
   ▼
Profiler Agent
   │
   ▼
Analyst Agent
   │
   ▼
Engineer Agent
   │
   ▼
Execution Agent
   │
   ▼
Validation
   │
   ├── Issues Found ─────────► Engineer Agent
   │
   └── No Issues
         │
         ▼
Cleaned Dataset
```

---

## ⚙️ Workflow

### 1️⃣ Data Profiling

The profiler agent collects:

- Column information
- Data types
- Missing values
- Summary statistics
- Duplicate records

---

### 2️⃣ Data Quality Analysis

The analyst agent uses **Llama 3.1** to:

- Analyze dataset quality
- Identify anomalies
- Recommend cleaning operations

---

### 3️⃣ Cleaning Code Generation

The engineer agent generates Python code for tasks such as:

- Handling missing values
- Removing duplicates
- Correcting data types
- Standardizing formats
- Eliminating inconsistencies

---

### 4️⃣ Code Execution

The execution agent:

- Executes generated cleaning code
- Applies transformations
- Saves cleaned dataset
- Captures execution errors

---

### 5️⃣ Validation Loop

The workflow automatically validates the cleaned dataset and repeats the cleaning process until acceptable data quality is achieved.

---

## 💡 Key Concepts

- Generative AI
- Multi-Agent Systems
- Workflow Automation
- Data Cleaning
- Data Profiling
- Large Language Models (LLMs)
- Prompt Engineering
- LangGraph State Machines

---

## 📊 Applications

- Data Science Projects
- Machine Learning Pipelines
- ETL Automation
- Business Intelligence
- Data Engineering
- Automated Data Preprocessing

---

## 🎯 Learning Outcomes

- Designed a multi-agent AI workflow using LangGraph.
- Integrated Llama 3.1 via the Groq API for intelligent data quality analysis.
- Automated dataset profiling, cleaning, validation, and iterative refinement.
- Built an end-to-end AI-assisted preprocessing pipeline for structured datasets.

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/AI-Data-Cleaning-Agent.git

cd AI-Data-Cleaning-Agent
```

Install dependencies:

```bash
pip install pandas numpy langchain langgraph langchain-groq
```

---

## ▶️ Running the Project

1. Add your dataset (.csv).
2. Configure your Groq API key.
3. Open the notebook.

```bash
jupyter notebook app.ipynb
```

Run all cells to start the automated data-cleaning workflow.

---

## 🔑 Environment Variables

Set your Groq API key before running:

```python
GROQ_API_KEY=your_api_key
```

---

## 📈 Future Improvements

- Streamlit Web Application
- Support for Excel and JSON files
- Visualization dashboard
- Human approval before execution
- Support for multiple LLM providers
- Automatic report generation

---

## 👨‍💻 Author

**Utsav Sharma**

B.Tech Information Technology

Aspiring Data Scientist | Machine Learning Engineer | AI Enthusiast

---

## ⭐ Star this repository if you found it useful!
