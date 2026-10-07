# ApexPlanet Task 4 – Data Storytelling & Statistical Validation

## Project Overview

This project is part of the **ApexPlanet Software Pvt Ltd Data Analytics Internship – Task 4**.

The objective of Task 4 is to transform the analytical findings from previous tasks into a clear business story, communicate insights through a professional presentation, and validate a business hypothesis using statistical testing.

---

## Objectives

This task focuses on:

- Converting analytical findings into a clear business narrative
- Presenting key findings and recommendations
- Formulating a testable business hypothesis
- Performing statistical hypothesis testing
- Calculating p-value and confidence interval
- Measuring effect size
- Translating statistical results into business conclusions

---

## Dataset

The analysis uses the cleaned sales dataset prepared during the previous internship tasks.

### Dataset Summary

- **Records:** 1,000
- **Unique Orders:** 992
- **Unique Customers:** 947
- **Total Units Sold:** 5,435
- **Total Revenue:** ₹13,93,99,439.65

---

## Business Story

The overall analytical journey follows the sequence:

**Data Cleaning → Exploratory Analysis → Business Intelligence → Customer Deep Dive → Statistical Validation**

The analysis identified important patterns in revenue, products, categories, customers, and customer segments. Task 4 extends this analysis by validating one of the business questions statistically.

---

## Hypothesis Testing

### Business Question

**Is there a statistically significant difference in mean customer-level revenue between male and female customers?**

### Hypotheses

**Null Hypothesis (H₀):**

The mean customer-level revenue is equal for male and female customers.

**Alternative Hypothesis (H₁):**

The mean customer-level revenue differs between male and female customers.

### Statistical Test

An **independent two-sample Welch's t-test** was used because the comparison involves two independent customer groups and does not require equal population variances.

### Significance Level

**α = 0.05**

---

## Hypothesis Testing Results

| Metric | Result |
|---|---:|
| Female Customers | 463 |
| Male Customers | 484 |
| Female Mean Revenue | ₹144,561.77 |
| Male Mean Revenue | ₹149,725.91 |
| Mean Difference (Female − Male) | −₹5,164.14 |
| t-statistic | −0.6383 |
| p-value | 0.5235 |
| 95% Confidence Interval | −₹21,042.49 to ₹10,714.21 |
| Cohen's d | −0.0415 |

---

## Statistical Conclusion

Since the **p-value (0.5235) is greater than 0.05**, the null hypothesis is not rejected.

Therefore, the available sample does **not provide sufficient statistical evidence** to conclude that mean customer-level revenue differs between male and female customers.

The confidence interval also includes zero, which is consistent with the hypothesis-test conclusion.

---

## Business Interpretation

Although the observed mean revenue differs between male and female customers, the difference is relatively small compared with the variability in customer-level revenue.

The statistical analysis suggests that **gender alone should not be treated as a strong predictor of customer revenue based on this dataset**.

Business decisions should therefore consider additional variables such as:

- Customer segment
- Purchase frequency
- Recency
- Product category
- City
- Customer lifetime behavior

---

## Key Business Insights

The combined analysis from previous tasks highlighted several important findings:

- **Electronics** is the highest-revenue product category.
- **Laptop** is the highest-revenue individual product.
- **March** records the highest monthly revenue.
- Customer segmentation reveals different levels of customer value and recency.
- Customer-level analysis supports more targeted retention and re-engagement strategies.

---

## Business Recommendations

Based on the overall analysis:

1. Focus retention strategies on high-value and loyal customers.
2. Use re-engagement campaigns for customers identified as at risk.
3. Monitor customer behavior beyond demographic variables.
4. Prioritize product and category performance when planning sales strategies.
5. Use data-backed statistical validation before making broad business assumptions.

---

## Presentation

The final Task 4 presentation contains:

- Business story and analytical journey
- Key business findings
- KPI and dashboard evidence
- Customer segmentation insights
- Hypothesis formulation
- Statistical methodology
- p-value and confidence interval
- Business interpretation
- Recommendations and conclusion

---

## Project Structure

```text
ApexPlanet-Task-4-Data-Storytelling-Statistical-Validation/
│
├── data/
│   └── Cleaned_ApexPlanet_Sales_Dataset.xlsx
│
├── presentation/
│   ├── ApexPlanet_Task4_Final_Presentation.pptx
│ 
│
├── statistics
│   ├── Hypothesis_Testing_Summary_formatted.xlsx
│   └── Hypothesis_Testing.ipynb
│
└── README.md
