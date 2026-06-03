# IT8416 Data Mining Project — Lending Club Loan Credit Risk Classification

**Group Number:** [3]  
**Project Title:** Lending Club Loan Credit Risk Classification

### Group Members:
* **Qassim Alhaddad** (ID: 202300649)
* **Ali Mohammed Radhi** (ID: 202304871)
* **Faisal Ali Ahmed ** (ID: 202305620)
* **Ali Alshuwaikh** (ID: 202302172)
* **Ali Hussain Yousif** (ID: 202301319)

---

## Project Overview
This project focuses on the Lending Club Loan dataset, a comprehensive collection of peer-to-peer lending data spanning 2007-2015 with approximately 890,000 loan records and 75 attributes. Our analysis applies supervised classification techniques to predict loan default risk and categorize borrower creditworthiness based on financial characteristics, credit history, and demographic factors. 

By leveraging the KDD (Knowledge Discovery in Databases) process, we develop predictive models to identify critical risk indicators for loan approval decisions, providing actionable insights for financial institutions, risk managers, and lending platforms to optimize portfolio management and minimize default rates.

---

## Dataset
* **Source:** Kaggle (Lending Club Loan Dataset)
* **Observations:** 890,000+ records with 75 attributes
* **Target Variable:** `Loan Status` (Fully Paid, Charged Off, Current, Late)
* **Loan Amount Range:** $1,000 - $40,000
* **Interest Rate Range:** 5.42% - 24.89%

---

## Tools Used
* **RapidMiner Studio 2023.11** — Building, preprocessing, and visualizations
* **Python 3.9+** — Data processing, analysis, and supplementary tools
* **Pandas & NumPy** — Data manipulation and analysis
* **Scikit-learn** — Machine Learning algorithm implementations
* **Matplotlib & Seaborn** — Data visualization

---

## Project Video 

Watch the complete project walkthrough [here](https://youtu.be/LtB5XJ1sVD8?si=1_AATWxwGYZw-i45).

### 📋 The video includes:
- **Project overview and business context**
- **Data exploration and visualization**
- **Preprocessing steps and transformations**
- **Model building and parameter tuning**
- **Results comparison and evaluation**
- **Key insights and recommendations**
- **GitHub repository overview**

---

## Pipeline Files

| File | Description |
| :--- | :--- |
| `task2_distribution_process.rmp` | Explores data distribution across variables |
| `task2_MissingData_process.rmp` | Pipeline for handling null entries and missing values |
| `task2_redundancy_process.rmp` | Filters redundant features and correlated attributes |
| `Task 3.rmp` | Training data with feature engineering, Time, Name Ensemble |
| `Task 4.rmp` | Classification models – Decision Tree, Naïve Bayes, Ensemble |
| `FINAL_DATA_MINING.docx` | Comprehensive documentation of final project outcomes |

---

## Models and Results

| Model | Test Accuracy | Validation Accuracy | Errors | Precision |
| :--- | :---: | :---: | :---: | :---: |
| **Decision Tree** | 99.73% | 99.78% | 19 | 8% |
| **Naïve Bayes** | 99.60% | 99.64% | 38 | 96% |
| **Vote Ensemble** | 99.73% | 99.79% | 0 | 98% |

> **Recommended Model:** **Vote Ensemble** — Highest validation accuracy and robust predictions with zero classification errors on the validation set.

### Key Finding
The Decision Tree model identified **Interest Rate** and **FICO Score** as the most critical features for predicting loan default risk. Borrowers with interest rates above 15% and FICO scores below 680 show a significantly higher default probability (87% accuracy in identifying at-risk loans), enabling financial institutions to make data-driven lending decisions and adjust portfolio risk accordingly.

---

## Project Structure
```text
├── 01_Project_Report/
│   └── FINAL_DATA_MINING.docx
├── 02_Software_Files/
│   ├── task2_distribution_process.rmp
│   ├── task2_MissingData_process.rmp
│   ├── task2_redundancy_process.rmp
│   ├── Task 3.rmp
│   └── Task 4.rmp
└── README.md

