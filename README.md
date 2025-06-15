# Task 1: Data Understanding & Exploratory Data Analysis (EDA)

## 📌 Objective

The purpose of this task is to explore and understand the structure, quality, and insights within the historical insurance dataset provided by AlphaCare Insurance Solutions (ACIS). This analysis sets the foundation for deeper statistical modeling and machine learning in subsequent tasks.

---


---

## 📋 Key Questions Addressed

- What is the overall **Loss Ratio** and how does it vary by `Province`, `VehicleType`, and `Gender`?
- Are there outliers in **TotalClaims** or **CustomValueEstimate** that could skew analysis?
- Are there **temporal trends** in claim frequency or severity?
- Which **vehicle makes/models** are associated with the highest and lowest claim amounts?

---

## 🧪 Key Analyses Performed

### ✅ Data Summarization
- Descriptive stats for financial variables (`TotalPremium`, `TotalClaims`, etc.)
- Dtype check and column formatting
- Missing value diagnostics

### ✅ Univariate Analysis
- Histograms for numeric columns
- Bar charts for categorical variables

### ✅ Bivariate & Multivariate Analysis
- Correlation heatmaps
- Trend analysis: Monthly claims vs premiums
- Zipcode-level scatter plots

### ✅ Outlier Detection
- Box plots for key numerical fields

### ✅ Visual Insights
- 3 creative and insightful visualizations highlighting key patterns

---

## 🧠 Key Insights

- Provinces like **Gauteng** and **Western Cape** show significant variance in loss ratios.
- Certain car **Makes/Models** consistently show higher claims — e.g., high-powered sedans and SUVs.
- Some **gender/location** groups show statistically significant risk differences.

> These insights will inform premium optimization strategies and targeted marketing.

---

## 🛠️ Tools & Libraries

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `pyarrow` for Parquet handling

---

## 📎 Notes

- The original `.txt` file was **converted to Parquet** to optimize performance and memory usage.
- Git practices followed: committed early and often with meaningful messages on `task-1` branch.

---

## 🧾 References

- Insurance Glossary: [Cornerstone Insurance Brokers](https://www.cornerstoneinsurance.ca/blog/insurance-terms/)
- A/B Testing: [Optimizely A/B Testing Guide](https://www.optimizely.com/optimization-glossary/ab-testing/)
- Statistical Tests: [SciPy Stats](https://docs.scipy.org/doc/scipy/reference/stats.html)

---

## ✅ Task Completion Checklist

- [x] Data loaded and converted to Parquet
- [x] EDA notebook created and committed to GitHub (`task-1` branch)
- [x] Summary stats and plots saved
- [x] README documented and included

---

**Next Step ➡️**  
Proceed to Task 2: Hypothesis Testing and Risk Segmentation.


