A/B Test Analysis — B2B Shop
🧠 Objective

Evaluate whether a new product variant increases conversion rate compared to the control group.

📁 Dataset
File: ab_test_data_B2Bshop_2.xlsx
Unit of analysis: user
Features:
user_id — unique user
test_group — control / test
orders — number of orders
geo_region — region
marketing_group — segment
🎯 Metric
Primary Metric:

Conversion Rate (CR)
CR = orders / users

🧪 Methodology
1. Exploratory Data Analysis
Checked group balance
Aggregated metrics by group
Segmented analysis (geo, marketing)
2. Hypothesis Testing

Null Hypothesis (H0):
Conversion rates are equal

Alternative Hypothesis (H1):
Conversion rates are different

Test used:

Chi-square test for proportions

Significance level:

α = 0.05
3. Bootstrap Analysis
Estimated distribution of difference
Calculated 95% confidence interval
4. Power Analysis
Target power: 80%
Estimated required sample size
📊 Results
Conversion (Control): X.XX%
Conversion (Test): X.XX%
Uplift: X.X%
p-value: X.XXXX
95% CI: [X.XXXX, X.XXXX]
🏁 Conclusion
Result: Significant / Not significant / Inconclusive
Recommendation:
Roll out / Do not roll out / Collect more data
💼 Business Impact

Estimated effect:

+X% conversion uplift
→ +X additional orders per 1000 users
🚀 How to Run
pip install pandas numpy scipy matplotlib seaborn statsmodels bootstrapped
jupyter notebook A_B_testing.ipynb
📌 Key Takeaways
Statistical significance ≠ business significance
Always validate results with bootstrap
Power analysis is critical before running experiments
