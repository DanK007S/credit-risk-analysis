# Credit Risk Analysis: Identifying High-Risk Bank Customers

## Overview

This project analyzes **1,125 bank customers** to identify patterns in credit risk and payment behavior. By examining customer demographics, account balance, and payment history, we uncover actionable insights that can inform lending decisions and risk mitigation strategies.

**Key Finding:** 20% of customers exhibit high-risk characteristics, with 2x higher rates of overdue payments compared to low-risk customers.

---

## Business Problem

Banks need to identify customers at risk of default to:
- Make informed lending decisions
- Allocate resources for proactive customer outreach
- Adjust interest rates based on risk profiles
- Reduce loan portfolio losses

This analysis provides a data-driven approach to segmenting customers by risk level.

---

## Dataset

| File | Description | Records | Key Columns |
|------|-------------|---------|------------|
| `customer_data.csv` | Customer demographics & account info | 1,125 | Age, Balance, Income, Account Status |
| `payment_data.csv` | Payment history & defaults | - | Payment Status, Overdue Days, Transaction Amount |

---

## Key Questions Investigated

1. **What percentage of customers are high-risk?**
   - Answer: 20% (225 out of 1,125 customers)

2. **How do payment patterns differ between risk groups?**
   - High-risk customers have **2.4x more overdue payments** (369 vs 151)

3. **Which customer characteristics correlate with default risk?**
   - High account balance is a strong indicator
   - Older customers show different risk profiles

4. **Can we segment customers into actionable risk tiers?**
   - Yes: High, Medium, Low-risk segments identified

---

## Methodology

### Tools & Libraries
- **Language:** Python 3.x
- **Environment:** Google Colab
- **Key Libraries:** 
  - Pandas (data manipulation & analysis)
  - Matplotlib & Seaborn (visualization)
  - NumPy (numerical computations)

### Analysis Steps
1. **Data Import & Cleaning**
   - Loaded customer and payment datasets
   - Handled missing values and data type conversions
   - Merged datasets on customer ID

2. **Exploratory Data Analysis (EDA)**
   - Analyzed distribution of key variables
   - Identified outliers and anomalies
   - Explored correlations between features

3. **Risk Segmentation**
   - Defined risk tiers based on overdue payment frequency
   - Profiled each segment by demographics & behavior
   - Compared payment patterns across segments

4. **Visualization & Insights**
   - Created comparative charts for high vs. low-risk customers
   - Visualized relationships between balance and default risk
   - Documented findings in executive summary

---

## Key Findings

### 1. Risk Distribution is Uneven
- **20% High-Risk** (225 customers): Show consistent overdue payment behavior
- **80% Low-Risk** (900 customers): Mostly on-time payers

### 2. Overdue Payments are a Strong Differentiator
| Risk Group | Avg Overdue Payments | Ratio |
|-----------|---------------------|-------|
| High-Risk | 369 | 2.4x |
| Low-Risk | 151 | 1x |

### 3. Account Balance Matters
- High-balance customers (>$50K): **22% high-risk**
- Low-balance customers (<$10K): **15% high-risk**
- Insight: Higher exposure may correlate with higher default rates

### 4. Age Shows Patterns
- Customers aged 40-55: Highest concentration of high-risk profiles
- Younger customers (<30): Generally lower risk

---

## How to Use This Project

### Prerequisites
```bash
pip install pandas matplotlib seaborn numpy
```

### Running the Analysis
1. **Open in Google Colab:**
   - Upload `credit_risk_analysis.ipynb` to Google Colab
   - Upload both CSV files to the session
   - Run cells sequentially

2. **Locally:**
   ```bash
   jupyter notebook credit_risk_analysis.ipynb
   ```

3. **Expected Output:**
   - Summary statistics of customer segments
   - Comparative visualizations (high vs. low-risk)
   - Correlation heatmaps
   - Risk distribution charts

---

## File Structure

```
credit-risk-analysis/
├── README.md                      # This file
├── credit_risk_analysis.ipynb     # Main analysis notebook
├── customer_data.csv              # Customer information (1,125 records)
├── payment_data.csv               # Payment history & defaults
└── requirements.txt               # Python dependencies (optional)
```

---

## Key Recommendations

### For Risk Management
1. **Implement risk-based pricing:** Apply higher interest rates to high-risk segment
2. **Enhanced monitoring:** Automated alerts for customers showing early warning signs
3. **Proactive outreach:** Contact customers before they miss payments

### For Further Analysis
1. **Predictive modeling:** Build a classification model to predict default probability
2. **Cohort analysis:** Track customer segments over time
3. **Feature engineering:** Create derived metrics (debt-to-income ratio, payment consistency score)

---

## Insights & Learnings

This project demonstrates:
- ✅ Data cleaning and merging from multiple sources
- ✅ Exploratory Data Analysis (EDA) best practices
- ✅ Pattern recognition and segmentation
- ✅ Business storytelling with data
- ✅ Clear visualization of complex patterns

**Next Steps for Portfolio:**
- Add SQL queries for reproducibility
- Build a predictive model (Logistic Regression, Random Forest)
- Create an interactive dashboard (Streamlit/Tableau)
- Deploy findings as a web app

---

## Author Notes

**Background:** This analysis was conducted as part of a career transition from iGaming Customer Support into Data Analysis. The project showcases the ability to translate business problems into data-driven insights—a skill directly applicable from customer service experience.

**Lessons Applied:**
- Customer behavior analysis (from iGaming CS experience)
- Pattern recognition in complex datasets
- Clear communication of findings to non-technical stakeholders

---

## Future Enhancements

- [ ] Add SQL version of analysis for reproducibility
- [ ] Implement predictive model for default probability
- [ ] Create Streamlit dashboard for interactive exploration
- [ ] Add statistical significance testing (Chi-square, t-tests)
- [ ] Expand analysis to include time-series patterns
- [ ] Build feature importance analysis

---

## License

This project is open source. Feel free to fork, modify, and use for educational purposes.

---

## Contact & Questions

If you have questions about the methodology or findings, feel free to open an issue on the repository.

**LinkedIn:** [Add your LinkedIn]  
**Portfolio:** [Add your portfolio website]

---

*Last Updated: May 2026*
