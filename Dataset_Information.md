# Dataset Information

This project uses two independent datasets for credit risk analysis.

---

## Dataset 1 — Credit Risk Dataset

- **Source:** Kaggle
- **Rows:** ~32,000
- **Features:** 12
- **Target Column:** `loan_status` (0 = Healthy, 1 = Default)

### Key Columns

| Column | Description |
|--------|-------------|
| `person_age` | Age of the loan applicant |
| `person_income` | Annual income of the applicant |
| `person_emp_length` | Employment length in years |
| `person_home_ownership` | Housing status (RENT, OWN, MORTGAGE) |
| `loan_amnt` | Loan amount requested |
| `loan_intent` | Purpose of the loan (EDUCATION, MEDICAL, etc.) |
| `loan_grade` | Credit grade assigned (A through G) |
| `loan_int_rate` | Interest rate on the loan |
| `loan_percent_income` | Loan amount as a percentage of annual income |
| `loan_status` | 0 = Healthy, 1 = Default |

---

## Dataset 2 — German Credit Dataset

- **Source:** UCI Machine Learning Repository
- **Rows:** 1,000
- **Features:** 20
- **Target Column:** `target` (good / bad)

### Key Columns

| Column | Description |
|--------|-------------|
| `age` | Age of the loan applicant |
| `credit_amount` | Amount of credit requested |
| `month_duration` | Loan duration in months |
| `status_and_sex` | Combined gender and marital status field |
| `target` | Credit outcome — good or bad |

---

## Notes

- Both datasets are used independently and share no common records
- The German dataset's `target` column is converted to a binary `Default` column (bad = 1, good = 0) during preprocessing
- The `status_and_sex` column is split to extract gender for demographic analysis