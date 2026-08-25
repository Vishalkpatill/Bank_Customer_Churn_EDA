# Bank Customer & Card Member Behavior Analysis — EDA

## 📌 Project Overview

This project performs an **Exploratory Data Analysis (EDA)** on a bank customer dataset containing customer demographics, financial characteristics, banking behavior, card ownership, satisfaction, complaints, loyalty points, and churn.

The objective is to understand **customer behavior and identify patterns associated with customer churn**, then convert those findings into meaningful business insights.

---

## 🎯 Business Objective

The analysis aims to answer questions such as:

- What is the overall customer churn rate?
- Which customer segments have higher churn?
- Does customer activity relate to churn?
- Does geography show differences in churn?
- How does age relate to churn?
- Does credit-card ownership appear to influence churn?
- How does card type relate to customer behavior?
- Are satisfaction scores associated with churn?
- What is the relationship between complaints and churn?
- Which customer segments could be potential retention targets?
- What business actions could improve customer retention?

---

## 📊 Dataset

**Dataset:** Customer Churn Records  
**Rows:** 10,000  
**Columns:** 18

### Main Variables

| Column | Description |
|---|---|
| `RowNumber` | Row identifier |
| `CustomerId` | Unique customer identifier |
| `Surname` | Customer surname |
| `CreditScore` | Customer credit score |
| `Geography` | Customer country |
| `Gender` | Customer gender |
| `Age` | Customer age |
| `Tenure` | Number of years with the bank |
| `Balance` | Customer account balance |
| `NumOfProducts` | Number of bank products held |
| `HasCrCard` | Whether the customer has a credit card |
| `IsActiveMember` | Whether the customer is an active member |
| `EstimatedSalary` | Estimated customer salary |
| `Exited` | Churn indicator: 1 = exited, 0 = retained |
| `Complain` | Whether the customer made a complaint |
| `Satisfaction Score` | Customer satisfaction score |
| `Card Type` | Customer card category |
| `Point Earned` | Loyalty/reward points earned |

---

## 🛠️ Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 🔍 EDA Workflow

1. **Data Loading** — Load the CSV and inspect its size.
2. **Data Understanding** — Inspect rows, columns, data types, and business meaning.
3. **Data Quality Checks** — Check missing values, duplicates, and unique values.
4. **Data Preparation** — Remove identifier columns from behavioral analysis and create readable labels.
5. **Descriptive Statistics** — Examine distributions, averages, ranges, and spread.
6. **Univariate Analysis** — Study individual variables.
7. **Bivariate/Multivariate Analysis** — Compare customer characteristics with churn.
8. **Customer Segmentation** — Explore potentially at-risk and high-value customer groups.
9. **Business Insights** — Convert patterns into actionable observations and recommendations.

---

## 📈 Analysis Performed

### Customer Churn
- Overall retained vs exited customers
- Overall churn rate

### Demographics
- Geography
- Gender
- Age groups

### Financial Characteristics
- Credit score
- Account balance
- Estimated salary

### Banking Behavior
- Number of products
- Tenure
- Customer activity
- Credit-card ownership

### Card Member Analysis
- Card type
- Loyalty points
- Card type vs churn
- Card type vs satisfaction

### Customer Experience
- Satisfaction score
- Complaint status
- Complaint vs churn

### Advanced Exploration
- Correlation heatmap
- Geography + activity segmentation
- High-balance customer analysis
- Exploratory risk segmentation

---

## 📊 Key Visualizations

The notebook contains:

- Customer retention vs churn count plot
- Numerical-variable histograms
- Geography distribution
- Gender distribution
- Churn rate by geography
- Churn rate by gender
- Churn rate by age group
- Credit score vs churn boxplot
- Balance vs churn boxplot
- Churn rate by number of products
- Churn rate by customer activity
- Churn rate by credit-card ownership
- Churn rate by card type
- Churn rate by satisfaction score
- Churn rate by complaint status
- Correlation heatmap
- Geography + activity segmentation

---

## 💡 Key Findings

Some important patterns identified during the analysis include:

- The overall churn rate is approximately **20.4%**.
- Germany shows a substantially higher observed churn rate than France and Spain.
- Older customer groups, particularly **46–55** and **56–65**, show higher observed churn.
- Inactive customers have a higher observed churn rate than active customers.
- Credit-card ownership alone shows only a small difference in churn.
- Card types show relatively modest differences in churn.
- The relationship between complaints and churn is **extremely strong** in this dataset.

### ⚠️ Important Data Quality Observation

The complaint variable requires special attention.

Almost every customer marked as having a complaint is classified as exited. This is unusually strong and should **not automatically be interpreted as causation**.

Before using `Complain` in a predictive model, investigate whether:

- The complaint was recorded after the customer exited.
- The variable contains target leakage.
- The variable was generated or encoded in a way that reflects churn.
- There is another data-generation issue.

This demonstrates an important analyst skill: **critically evaluating the data instead of blindly trusting a correlation.**

---

## 💼 Business Recommendations

1. **Retention targeting** — Focus retention efforts on customer segments with elevated churn.
2. **Customer engagement** — Investigate why inactive customers show higher churn and test engagement strategies.
3. **Customer service** — Investigate complaints and service interactions, especially because of their unusually strong association with churn.
4. **Geographic strategy** — Investigate the reasons for higher churn in Germany.
5. **Age-based targeting** — Investigate the needs and behavior of older customer segments with higher churn.
6. **Card strategy** — Compare card types using churn, satisfaction, and loyalty engagement before designing targeted offers.
7. **High-value retention** — Monitor high-balance customers who also show behavioral signals associated with churn.

---

## 📁 Project Structure

```text
Bank-Customer-Churn-EDA/
│
├── Customer-Churn-Records.csv
├── Bank_Customer_Churn_EDA.ipynb
└── README.md
```

---

## ▶️ How to Run

### 1. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 2. Keep the CSV and notebook in the same folder

```text
Customer-Churn-Records.csv
Bank_Customer_Churn_EDA.ipynb
```

### 3. Start Jupyter

```bash
jupyter notebook
```

### 4. Open

```text
Bank_Customer_Churn_EDA.ipynb
```

### 5. Run the cells from top to bottom.

---

## 🧠 Skills Demonstrated

- Python
- Pandas
- NumPy
- Data cleaning
- Missing-value analysis
- Duplicate detection
- Descriptive statistics
- GroupBy and aggregation
- Filtering
- Feature creation
- Binning
- Univariate analysis
- Bivariate analysis
- Multivariate analysis
- Data visualization
- Customer segmentation
- Business interpretation
- Critical data-quality evaluation
- Business recommendations

---

## 🚀 Future Improvements

This project can be extended with:

- Customer segmentation using clustering
- Churn prediction using machine learning
- Feature engineering
- Statistical hypothesis testing
- Model evaluation
- Power BI dashboard
- Executive business report
- Customer lifetime value analysis
- More advanced offer/targeting analysis

---



## 👤 Project Focus

**Domain:** Banking / Customer Analytics  
**Primary Skill:** Exploratory Data Analysis  
**Target Variable:** `Exited`  
**Dataset Size:** 10,000 customers × 18 columns  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook


