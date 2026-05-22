# 💳 Real-World Finance Data Project
### Credit & Debit Card Dataset — End-to-End Data Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange?logo=googlecolab)
![Domain](https://img.shields.io/badge/Domain-Finance-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Project Overview

This project is a **real-world data science project** in the **Finance** domain, completed as part of Task 4 of the applied data science course.

The dataset contains credit and debit card information across thousands of clients, including card brands, types, credit limits, expiry dates, chip status, and more. The goal is to perform a complete **end-to-end data analysis** — from raw data to actionable insights and predictive modeling.

---

## 🗂️ Dataset Description

**File:** `cards_data.csv`  
**Rows:** ~6,000+ | **Columns:** 13

| Column | Description |
|---|---|
| `id` | Unique card ID |
| `client_id` | Unique client identifier |
| `card_brand` | Brand: Visa, Mastercard, Amex, Discover |
| `card_type` | Type: Credit, Debit, Debit (Prepaid) |
| `card_number` | Masked card number |
| `expires` | Card expiry date (MM/YYYY) |
| `cvv` | Card CVV code |
| `has_chip` | Whether the card has a chip (YES/NO) |
| `num_cards_issued` | Number of cards issued to the client |
| `credit_limit` | Credit limit in USD |
| `acct_open_date` | Account opening date (MM/YYYY) |
| `year_pin_last_changed` | Year the PIN was last changed |
| `card_on_dark_web` | Whether card appears on dark web (Yes/No) |

---

## 🎯 Project Goals

1. **Explore** the dataset structure, distributions, and trends
2. **Clean** and preprocess raw data (dates, currency, categoricals)
3. **Visualize** key patterns and relationships
4. **Engineer** meaningful features
5. **Predict** card credit tier using machine learning
6. **Summarize** insights and business recommendations

---

## 📊 Key Analyses Performed

### Exploratory Data Analysis
- Card brand and type distribution
- Credit limit distribution and outlier analysis
- Chip-enabled card breakdown by brand
- Account opening trends over time
- Cards issued per client distribution
- Expiry year distribution and expired cards count

### Feature Engineering
- Card age (years since account opening)
- Expiry status (active vs expired)
- Years since PIN last changed
- High credit flag (above/below median)

### Machine Learning
- **Task:** Binary classification — High Credit vs Low Credit limit
- **Models:** Random Forest Classifier, Logistic Regression
- **Evaluation:** Accuracy, Precision, Recall, F1-Score, Confusion Matrix
- **Feature Importance:** Identified key drivers of credit tier

---

## 📈 Key Findings

| Finding | Insight |
|---|---|
| **Visa dominates** | Largest share of cards issued |
| **Debit > Credit** | Debit cards are issued more than credit cards |
| **Chip adoption: ~87%** | Strong security infrastructure |
| **Credit cards have higher limits** | As expected in real banking behavior |
| **PIN hygiene gap** | Some card types show 10+ years since last PIN change |
| **Random Forest accuracy: ~XX%** | Strong predictive power for credit tier classification |

---

## 🧰 Technologies Used

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core programming language |
| Google Colab | Development environment |
| Pandas | Data manipulation |
| NumPy | Numerical computing |
| Matplotlib / Seaborn | Static visualizations |
| Plotly | Interactive visualizations |
| Scikit-learn | Machine learning models |

---



## 📁 Repository Structure

```
finance-card-analysis/
│
├── finance_card_analysis.ipynb   # Main analysis notebook
├── cards_data.csv                # Dataset
├── README.md                     # Project documentation
└── requirements.txt              # Python dependencies
```

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
```

Install with:
```bash
pip install -r requirements.txt
```

---

## 📝 Conclusions & Recommendations

1. **Chip security:** Push non-chip card replacements to remaining users
2. **PIN hygiene:** Trigger PIN update campaigns for stale PINs (5+ years unchanged)
3. **Premium targeting:** Clients with multiple long-tenure cards are ideal for credit upgrade offers
4. **Expiry outreach:** Proactively contact holders of expired cards for renewal
5. **Fraud watch:** Monitor cards with long PIN inactivity + no chip for risk


*Submitted for: Real-World Data Project (Finance, Health, or Retail) — Task 4*  
*Due Date: 29 May 2026*
