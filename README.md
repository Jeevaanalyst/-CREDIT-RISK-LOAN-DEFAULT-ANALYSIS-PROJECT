Dataset Description  : 

Applicant info — loan_id, application_date, age, gender, marital_status, education, state, city_tier.

Employment — employment_type, emp_length_years, annual_income, monthly_income.

Loan details — loan_type, loan_purpose, loan_amount, loan_term_months, interest_rate, loan_grade, monthly_emi, collateral_value, ltv_ratio, co_applicant.

Credit history — credit_score, credit_history_yrs, num_open_accounts, num_credit_lines, credit_util_ratio, missed_payments, bankruptcies, derogatory_marks.

Assets — home_ownership, has_vehicle, num_dependents, existing_loans, total_debt.

Financial ratios — debt_to_income, loan_to_income, emi_to_income, default_probability.


Here are the complete insights from your Credit Risk Analysis Report across all 9 sheets:


##  Overview

The portfolio covers 1,00,000 loans worth ₹3,530 Crore with an average loan size of ₹3.53 lakh. The overall default rate is 23.13% meaning roughly 1 in 4 borrowers defaulted. Average credit score is 674 and average interest rate is 16.73%.


## Insight 1  Credit Score is the Strongest Default 

| Credit Band | Default Rate |

| Poor (< 580) | 59.50 % |

| Fair (580–640) | 27.89 % |

| Good (640–720) | 19.39 % |

| Excellent (720+) | 9.77% |

Key finding: Poor credit borrowers default at 6× the rate of Excellent credit borrowers. Any applicant below 580 should be flagged immediately.

## Insight 2  DTI Ratio is a Critical Threshold Indicator

| DTI Band | Default Rate |

| 0–27.9% (Low) | 9.25% |

| 27.9–50.8% (Moderate) | 13.89% |

| 50.8–73.6% (High) | 30.83% |

| 73.6–96.7% (Very High) | 31.25% |

| 96.7–120% (Extreme) | 30.48% |

Key finding: There is a sharp cliff at DTI = 50.8%. Below 50% the default rate is under 14%. Above 50% it triples to over 30%. This 50% threshold should be a hard underwriting rule applicants.

## Insight 3  Employment Type Reveals Hidden Risk

| Employment Type | Default Rate | Avg Income |

| Freelancer | 28.66% | ₹39,565 |

| Salaried | 23.00% | ₹63,068 |

| Self-Employed | 22.94%  | ₹54,501 |

| Business Owner | 22.19% | ₹1,25,708 |

| Government | 20.17% | ₹65,184 |

Key finding: Freelancers default at the highest rate despite being the lowest income group. Government employees are the most reliable segment. Business Owners earn the most but still carry moderate risk .

## Insight 4  Loan Purpose Risk is Narrow but Meaningful

| Loan Purpose | Default Rate |

| Debt Consolidation | 23.39% — Highest |

| Vehicle Purchase | 23.25% |

| Home Purchase | 23.26% |

| Personal | 22.89% — Lowest |

| Wedding | 22.96% |

Key finding: Debt Consolidation carries the highest default risk borrowers already in financial stress are consolidating existing debt, making them inherently more vulnerable. The spread is narrow (22.89%–23.39%) .


## Insight 5 Loan Grade Does Not Differentiate Risk 

| Loan Grade | Applications | Default Rate |

| A | 15,094 | 22.98% |

| B | 24,896 | 22.90% |

| C | 28,014 | 23.50% |

| D | 18,152 | 23.16% |

| E | 9,800 | 23.27% |

| F | 4,044 | 21.98%|

Key finding: Default rates across all loan grades are nearly identical (22–23.5%). Grade F borrowers are defaulting at almost the same rate as Grade A this indicates the loan grading model is not working effectively and needs to be recalibrated. A well-functioning grade system should show a clear gradient from A to F.


## Insight 6 Geography: East and North India are Higher Risk

| Top 3 High-Risk States | Default Rate |

| West Bengal | 23.78% |

| Bihar | 23.60% |

| Rajasthan | 23.56%|

| Uttar Pradesh | 23.56% |


| Lowest Risk States | Default Rate |


| Haryana | 22.23% |

| Andhra Pradesh | 22.43% |

| Delhi | 22.65% |

Key finding: East and North Indian states show higher default rates. Southern states (Andhra Pradesh, Kerala, Karnataka) are comparatively safer. The spread is only 1.55 percentage points geography is a weak predictor compared to credit score and DTI.


## Insight 7 Risk Tier Summary (Most Actionable)

| Risk Tier | Applications | Default Rate | Avg Loan |

| High Risk | 7,296 (7.3%) | 59.50%| ₹3.58L |

| Medium Risk | 31,451 (31.5%) | 27.89% | ₹3.52L |

| Low Risk | 42,648 (42.6%) | 19.39%| ₹3.54L |

| Very Low Risk | 16,697 (16.7%) | 9.77% | ₹3.51L |

Key finding: The 7,296 High Risk customers are defaulting at nearly 60%  approving these loans is generating massive losses. Rejecting this segment entirely would cut the portfolio default rate from 23.13% to approximately 18%.


## Insight 8 High Risk Customer Profile (100 deep-dive records)

From the 100 high-risk customer records:

Average credit score: 551 (Poor band)

Average DTI: 0.997 (Extreme: nearly 100% of income goes to debt)

Average default probability: 55.9%

Average loan amount: ₹18.9 lakh : these are large ticket loans going to the riskiest borrowers

73% are in Mortgage or Rent : no owned assets as buffer

47% are Salaried : even stable employment doesn't save them when DTI is extreme

58% are already delinquent (Charged Off + Late 31-120 days + Default + Late 16-30 days)


## Top 4 Business Recommendations

1. Implement hard DTI cutoff at 50% : Default rate triples above this level. No exceptions without collateral worth 1.5× loan value.

2. Recalibrate the loan grading model: Grade A and Grade F borrowers defaulting at the same rate means the scoring system is broken. Rebuild it using credit score + DTI + employment type as primary inputs.

3. Create a Freelancer risk surcharge :They default 5.66 points above Government employees. Price this risk into the interest rate or require a 6-month income proof threshold.

4. Auto-decline High Risk tier :The 7,296 High Risk applicants carry a 59.5% default rate. The expected loss on this segment far exceeds any interest income. 
