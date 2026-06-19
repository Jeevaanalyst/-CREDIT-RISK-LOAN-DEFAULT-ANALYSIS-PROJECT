Dataset Description :

Applicant info — loan_id, application_date, age, gender, marital_status, education, state, city_tier.

Employment — employment_type, emp_length_years, annual_income, monthly_income.

Loan details — loan_type, loan_purpose, loan_amount, loan_term_months, interest_rate, loan_grade, monthly_emi, collateral_value, ltv_ratio, co_applicant.

Credit history — credit_score, credit_history_yrs, num_open_accounts, num_credit_lines, credit_util_ratio, missed_payments, bankruptcies, derogatory_marks.

Assets — home_ownership, has_vehicle, num_dependents, existing_loans, total_debt.

Financial ratios — debt_to_income, loan_to_income, emi_to_income, default_probability.


------------------------------------------------------------------------------------------------------------------------------------------------------------

## Business Recommendations

1. Implement hard DTI cutoff at 50% : Default rate triples above this level. No exceptions without collateral worth 1.5× loan value.

2. Recalibrate the loan grading model: Grade A and Grade F borrowers defaulting at the same rate means the scoring system is broken. Rebuild it using credit score + DTI + employment type as primary inputs.

3. Create a Freelancer risk surcharge :They default 5.66 points above Government employees. Price this risk into the interest rate or require a 6-month income proof threshold.

4. Auto-decline High Risk tier :The 7,296 High Risk applicants carry a 59.5% default rate. The expected loss on this segment far exceeds any interest income. 
