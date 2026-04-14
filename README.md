# Hospital Readmission Analysis for Diabetic Patients

##  Project Overview
Exploratory data analysis of 101,766 hospital encounters to identify drivers of 30-day readmissions in diabetic patients.

**Key Finding:** 35% readmission rate exceeds national benchmark by 75%, with care transition failures (not clinical complexity) as primary driver.

##  Business Impact
- **$6.7M** annual readmission cost burden identified
- **Medicare penalty risk** quantified at 75% above threshold
- **Targeted intervention** recommended with $2M+ savings potential

##  Dataset
- **Source:** [UCI Machine Learning Repository - Diabetes 130-US Hospitals]
- **Size:** 101,766 encounters, 71,518 unique patients
- **Time Period:** 1999-2008
- **Features:** 50 variables (demographics, clinical, medications)

##  Technologies
- **Python 3.x**
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly, SciPy
- **Tools:** Jupyter Notebook, VS Code

##  Key Findings

### 1. Readmission Crisis
- 35% of patients readmitted >30 days post-discharge
- 11% readmitted <30 days (acute clinical failures)
- 75% higher than 20% national benchmark

### 2. Demographic Patterns
- 70% of admissions are patients 60+
- Peak at age 70-80 (26% of total)
- Readmission rates consistent across age groups (unexpected)

### 3. Clinical Insights
- Weak correlation (r=0.27) between medications and lab procedures
- Longer initial stays don't reduce readmission risk
- Care transitions, not clinical intensity, drive readmissions

##  Recommendations
1. **[HIGH]** Implement 30-day post-discharge follow-up for 70+ patients
2. **[MEDIUM]** Audit geriatric discharge planning processes
3. **[LOW]** Standardize medication-lab testing protocols

##  Methodology

### Data Cleaning
- Replaced '?' missing value markers with NA
- Filtered 2,273 records (2.2%) with missing demographics
- Created patient-level dataset (first visit only) to avoid duplication bias

### Statistical Analysis
- Chi-square tests for categorical relationships (p<0.05)
- T-tests for continuous variable comparisons
- Correlation analysis for clinical metrics
- 95% confidence intervals for key
