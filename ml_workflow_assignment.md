Task 1 — Label & Data Leakage
Label (Target Variable)
repeat_purchase_flag

This is the outcome you're trying to predict—whether a customer makes a repeat purchase within 30 days. If you pick anything else, you're solving the wrong problem.

Data Leakage Column
discount_used_on_repeat_order

Why:
This variable is only known after the repeat purchase happens. You're trying to predict the repeat purchase itself—so using this is like peeking at the answer sheet during the exam.

Task 2 — What Your Manager Skipped (And Why It’s a Problem)
1. Exploratory Data Analysis (EDA)

What should be done:

Check distributions (e.g., days_since_last_order)
Look for class imbalance in repeat_purchase_flag
Identify correlations and outliers

You won’t know if your model is learning real patterns or noise
You might miss obvious issues (like skewed data or useless features)
