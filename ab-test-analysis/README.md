# A/B Testing Conversion Analysis

## Project Overview

This project analyzes an A/B experiment designed to evaluate whether a new webpage design improves user conversion rates compared with the original version.

A two-proportion z-test is used to determine whether the difference between the two groups is statistically significant.

The analysis follows a typical data analytics workflow including data exploration, hypothesis testing, and visualization.

---

## Business Problem

A company is testing a new webpage design to determine whether it improves the user conversion rate.

Two groups are compared:

- **Control group:** users who see the original webpage
- **Treatment group:** users who see the new webpage

The goal is to determine whether the new design leads to a statistically significant improvement in conversion rate.

---

## Dataset

The dataset simulates an A/B testing experiment containing the following variables:

| Column | Description |
|------|-------------|
| user_id | unique identifier for each user |
| group | experiment group (control or treatment) |
| converted | whether the user converted (1 = yes, 0 = no) |

The simulated dataset contains **10,000 users** split between control and treatment groups.

---

## Methodology

The analysis follows these steps:

1. Data generation and preprocessing
2. Exploratory data analysis (EDA)
3. Conversion rate comparison
4. Hypothesis testing using a **two-proportion z-test**
5. Confidence interval estimation
6. Visualization of experiment results

### Hypothesis

Null hypothesis (H0):

Conversion rate of the treatment group equals the conversion rate of the control group.

Alternative hypothesis (H1):

Conversion rate of the treatment group is different from the control group.

---

## Results

The analysis computes:

- Conversion rate for both groups
- Difference in conversion rates
- Z-statistic
- P-value
- 95% confidence intervals

Example visualization:

### Conversion Rate by Group

![Conversion Rate](images/conversion_rate_by_group.png)

### Sample Size by Group

![Sample Size](images/sample_size_by_group.png)

### Conversion Rate with Confidence Interval

![Confidence Interval](images/conversion_rate_confidence_interval.png)

---

## Key Findings

- The treatment group shows a higher conversion rate compared with the control group.
- Statistical testing is used to determine whether the difference is significant.
- If the p-value is below 0.05, the treatment design can be considered statistically better.

---

## Tools

Python  
Pandas  
NumPy  
Matplotlib  
Seaborn  
Statsmodels  
Jupyter Notebook

---

## Project Structure

```
ab-test-analysis
│
├── data
│   └── ab_test_data.csv
│
├── images
│   ├── conversion_rate_by_group.png
│   ├── sample_size_by_group.png
│   └── conversion_rate_confidence_interval.png
│
├── ab_test.ipynb
└── README.md
```


---

## Author

Lewei Gao  
Statistics Student – McMaster University
