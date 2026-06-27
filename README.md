[Job_acceptance_system.pdf](https://github.com/user-attachments/files/29403055/Job_acceptance_system.pdf)
[code.py.txt](https://github.com/user-attachments/files/29403400/code.py.txt)
Job-Acceptance-System
Tech Stack

- Language:** Python 3
- Data handling: Pandas, NumPy
- Visualization: Matplotlib, Seaborn
- Machine learning: Scikit-learn
- Database (optional): MySQL + SQLAlchemy
- Dashboard: Streamlit


Approach

1. Data Collection — Load the 50K+ record dataset and validate shape, dtypes, and sample records.
2. Data Understanding — Profile each feature group (academic, skills, experience, market) and inspect the null distribution.
3. Data Cleaning & Preprocessing
   - Impute missing values (mean / median / mode as appropriate per column)
   - Standardize inconsistent categorical labels (e.g. unify gender and Yes/No casing/whitespace)
   - Encode categorical variables (Label / One-Hot Encoding)
   - Scale numerical features
   - Remove duplicate-like records and check logical consistency across fields
4. Exploratory Data Analysis (EDA) — Examine relationships such as:
   - Interview/technical score vs. job acceptance
   - Skills match percentage vs. placement
   - Company tier vs. acceptance rate
   - Experience vs. placement probability
   - Competition level vs. job acceptance
   - Correlation analysis among numeric features
5. Feature Engineering — Derive analytical features:
   - Experience category (Fresher / Junior / Senior)
   - Academic performance bands
   - Skills match level (Low / Medium / High)
   - Interview performance category
   - Placement probability score
6. Data Storage (optional) — Persist the cleaned dataset to MySQL via SQLAlchemy for scalable querying/reporting.
7. Machine Learning Modeling
   - Target: `status` → `Placed` = 1 (job accepted), `Not Placed` = 0 (job rejected)
   - Train/evaluate classification models (e.g. Logistic Regression, Random Forest, Gradient Boosting)
   - Evaluate with accuracy, precision, recall, F1-score, ROC-AUC (important given class imbalance)
   - Interpret feature importance for business explainability
8. Dashboard — Visualize KPIs and insights interactively in Streamlit.

Analyst Tasks (EDA & ML Analytics)

- Candidate performance: academic scores vs. placement outcome, skills match vs. interview performance, certification impact on acceptance
- Placement & acceptance: acceptance rate by company tier, experience vs. placement success
- Interview & evaluation: interview score vs. placement probability, employability test score analysis


Results

- A cleaned, normalized job placement dataset with missing values handled and inconsistencies corrected
- A structured analytical dataset spanning academic, skill-based, experiential, and interview-related features
- Classification model(s) predicting job offer acceptance with strong accuracy and explainability
- Actionable insights on the key drivers of placement success
- An interactive Streamlit dashboard surfacing placement KPIs
