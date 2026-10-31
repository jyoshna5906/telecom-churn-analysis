# 📊 Telecom Customer Churn Analysis & Prediction

An end-to-end Data Analytics and Machine Learning project that analyzes telecom customer behavior, identifies factors influencing customer churn, and predicts customers who are likely to leave a telecom service.

The project uses **Python, Machine Learning, and Power BI** to turn customer data into actionable business insights.

---

## 🎯 Problem Statement

Customer churn is a major challenge for telecom companies. When customers discontinue their services, companies lose revenue and business opportunities.

This project aims to understand why customers leave, identify important churn patterns, and build predictive machine learning models to help telecom companies improve customer retention.

## 🎯 Project Objectives

- Analyze customer data to understand churn behavior.
- Identify the major factors influencing customer churn.
- Perform data cleaning and Exploratory Data Analysis (EDA).
- Build and evaluate machine learning models.
- Develop a Power BI dashboard for business insights.
- Suggest strategies to reduce customer churn.

## 📁 Dataset

**Dataset:** IBM Telco Customer Churn Dataset

- Total customer records: 7,043
- Total columns: 21
- Records after data cleaning: 7,032
- Target variable: `Churn`

The dataset contains customer information such as:
- Gender and senior citizen status
- Tenure and contract type
- Internet and phone services
- Monthly and total charges
- Payment methods
- Customer churn status

## 🛠️ Tools & Technologies

| Category | Technologies |
|---|---|
| Programming | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Dashboard | Microsoft Power BI |
| Development | Jupyter Notebook |
| Version Control | Git & GitHub |

## ⚙️ Project Workflow

1. **Data Collection:** Load the IBM Telco Customer Churn dataset.
2. **Data Cleaning:** Handle missing values, correct `TotalCharges`, remove unnecessary columns and encode categorical variables.
3. **Exploratory Data Analysis:** Analyze customer demographics, tenure, contracts, payment methods and churn patterns.
4. **Feature Analysis:** Identify the important factors associated with customer churn.
5. **Model Building:** Train Logistic Regression and Random Forest models.
6. **Model Evaluation:** Compare accuracy, precision, recall, F1-score and ROC-AUC.
7. **Power BI Dashboard:** Present customer churn insights through visualizations.

## 📈 Key Business Insights

The analysis identified the following patterns:

- Overall customer churn rate is approximately **26.58%**.
- Month-to-month contract customers have a higher churn rate (42.7%) compared to two-year contract customers (2.8%).
- Fiber optic internet customers show a churn rate of approximately 41.9%.
- Electronic check users have a higher churn rate (45.3%).
- Churned customers have an average tenure of 18 months, compared to 37.7 months for retained customers.
- Churned customers have higher average monthly charges (74.44) compared to retained customers (61.31).

## 🤖 Machine Learning Model Performance

Three model configurations were evaluated:

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 80.45% | 0.648 | 0.575 | 0.609 | 0.836 |
| Random Forest | 78.68% | 0.621 | 0.508 | 0.559 | 0.818 |
| Logistic Regression (Balanced) | 72.60% | 0.491 | 0.797 | 0.608 | 0.835 |

### Best Model

**Logistic Regression** achieved the highest overall accuracy and ROC-AUC score.

The balanced Logistic Regression model achieved a higher churn recall of 0.797, making it useful when identifying more potentially churned customers is the priority.

Saved models:
- `models/churn_model.pkl`
- `models/churn_model_balanced.pkl`

## 📊 Visualizations

The project includes the following visualizations to understand customer churn patterns and model performance.

### 1. Customer Churn Distribution
![Churn Distribution](images/churn_distribution.png)

### 2. Contract Type vs Churn
![Contract vs Churn](images/contract_vs_churn.png)

### 3. Customer Dashboard
![Dashboard](images/dashboard.png)

### 4. Feature Importance
![Feature Importance](images/feature_importance.png)

### 5. Model Feature Importance
![Model Feature Importance](images/model_feature_importance.png)

### 6. Monthly Charges vs Churn
![Monthly Charges vs Churn](images/monthly_vs_churn.png)

### 7. Payment Method vs Churn
![Payment Method vs Churn](images/payment_vs_churn.png)

### 8. Tenure vs Churn
![Tenure vs Churn](images/tenure_vs_churn.png)

Explore the Jupyter Notebook for the complete Exploratory Data Analysis, charts and model evaluation.

- [View Jupyter Notebook](churn.ipynb)
- [View HTML Report](churn.html)
- [View Power BI Dashboard File](churn_dashboard.pbix)


## 💡 Business Recommendations

Based on the analysis, the following strategies can help telecom companies reduce customer churn:

1. **Contract Upgrades:** Encourage month-to-month customers to choose long-term contracts through special offers.
2. **Customer Retention:** Introduce loyalty programs and retention campaigns for new customers.
3. **Payment Methods:** Encourage automatic payment methods for convenient billing.
4. **Service Improvement:** Review pricing and service quality for fiber optic customers.
5. **Customer Support:** Provide additional support and service benefits to customers with shorter tenure.

## 📂 Project Structure

```text
telecom-churn-analysis/
│
├── data/
│   ├── Raw and cleaned datasets
│
├── images/
│   └── model_feature_importance.png
│
├── models/
│   ├── churn_model.pkl
│   └── churn_model_balanced.pkl
│
├── churn.ipynb
├── churn.html
├── churn_dashboard.pbix
└── README.md
```

## 🚀 How to Run the Project

**Step 1: Clone the repository**

```bash
git clone https://github.com/jyoshna5906/telecom-churn-analysis.git
```

**Step 2: Navigate to the project folder**

```bash
cd telecom-churn-analysis
```

**Step 3: Install the required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5:** Open `churn.ipynb` and run the notebook cells.

To explore the dashboard, open `churn_dashboard.pbix` using Microsoft Power BI Desktop.

## 📌 Project Outcome

This project demonstrates how Data Analytics and Machine Learning can be used to understand customer behavior, identify churn risks and support business decision-making.

It combines data preprocessing, exploratory analysis, predictive modeling and interactive business reporting in one project.

---

**Technologies:** Python | Machine Learning | Pandas | Scikit-learn | Power BI | Git & GitHub

**Project Category:** Data Analytics & Machine Learning