# Employee Attrition Analysis

A comprehensive data analysis project investigating factors contributing to employee attrition and providing actionable business recommendations to reduce turnover rates.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Key Findings](#key-findings)
- [Analysis Sections](#analysis-sections)
- [Business Recommendations](#business-recommendations)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Conclusions](#conclusions)

## 🎯 Project Overview

This analysis examines employee attrition patterns across various dimensions including:
- **Demographics**: Age, gender, marital status
- **Job Characteristics**: Job level, role, department, involvement, satisfaction
- **Work Experience**: Total working years, tenure at company, years in current role
- **Compensation**: Monthly income, stock options
- **Work Environment**: Business travel, overtime, environment satisfaction

The goal is to identify key drivers of employee attrition and provide strategic recommendations to improve employee retention.

## 📊 Dataset Information

**Dataset**: HR_Analytics.csv

### Features Analyzed:
- **Numeric Features (12)**: Age, EnvironmentSatisfaction, JobInvolvement, JobLevel, JobSatisfaction, MonthlyIncome, StockOptionLevel, TotalWorkingYears, YearsAtCompany, YearsInCurrentRole, YearsWithCurrManager
- **Categorical Features (6)**: BusinessTravel, Department, EducationField, Gender, JobRole, MaritalStatus, OverTime

### Data Quality:
- ✅ No missing values
- ✅ No duplicated records
- Overall attrition rate: ~16%

## 🔑 Key Findings

### Attrition by Business Travel
- **Frequently Travel**: 25% attrition rate (highest risk)
- **Rarely Travel**: 15% attrition rate
- **Never Travel**: 8% attrition rate (lowest risk)

### Attrition by Department
- Sales: 20% attrition
- HR: 19% attrition
- R&D: 13.8% attrition (lowest)

### Attrition by Job Level
- **Level 1 (Entry)**: 60% of all attritions - highest risk group
- **Level 2 (Intermediate)**: 21% of attritions
- **Level 4-5 (Senior)**: Very low attrition rates

### Attrition by Tenure
- **Year 1**: 24.89% of all attritions (critical period)
- **Year 2**: 11.39% of attritions
- **After Year 2**: Attrition drops below 10% per year
- **10+ Years**: Very stable employees with minimal attrition risk

### Attrition by Age Group
- **26-30 years**: 23.63% of attritions
- **31-35 years**: 25.32% of attritions (highest)
- **40+ years**: Below 10% attrition rate

### Attrition by Marital Status
- Single: 25% attrition rate (highest)
- Married: 12.4% attrition rate (50% lower)
- Divorced: 10% attrition rate (lowest)

### Income Impact
Income difference between staying and departing employees is minimal, indicating **income is NOT the primary driver** of attrition.

### Career Path Observations
- Employees who leave show faster career progression (Levels 1-2) but slower advancement at higher levels
- Employees who stay show steady, consistent career progression (~3 years per level)

## 📈 Analysis Sections

### Univariate Analysis
- Distribution analysis of all numeric features
- Frequency distribution of categorical variables
- Statistical summaries (mean, median, quartiles)

### Bivariate Analysis
Comprehensive examination of relationships between features and attrition:
- Business Travel impact on attrition
- Department and Job Role comparisons
- Marital Status influence
- Overtime work patterns
- Age and tenure distributions
- Job Level salary progression
- Years in current role analysis

### Correlation & Satisfaction Analysis
- Heatmap analysis comparing attrition vs. staying employees
- Investigation of satisfaction metrics (job, environment)
- Analysis segmented by gender, department, marital status, and job role
- Special focus on long-tenured employees (10+ years)

## 💡 Business Recommendations

### Priority 1: Job Level 4 & 5 Employees
**Why?** Difficult to replace; highest career potential

- **For Level 4**: Reduce business travel and working hours
- Monitor manager relationships; consider manager changes after 10 years
- Improve environment and job satisfaction through surveys

### Priority 2: Job Level 1-3 Employees (Sales & R&D)
- Increase salaries, especially for Level 2 positions
- Offer promotion/level-up tests before 5 years of work (critical period)
- Target age group 18-36 for early career development

### Priority 3: Long-Tenured Employees (10+ Years)
- Survey and address manager-employee relationships
- Monitor job satisfaction and environment satisfaction
- Proactively discuss career advancement and role changes

### Priority 4: Demographic-Specific Strategies
- **Divorced employees**: Focus on work environment improvements
- **Single employees**: Emphasize job satisfaction and career development
- **Married employees**: May be more stable; focus on retention bonuses
- **Female employees in Sales/R&D**: Address income equity
- **Male HR employees**: Improve job satisfaction initiatives

### Priority 5: High-Risk Indicators
- **Overtime workers**: Workload management and flexible scheduling
- **Frequent travelers**: Travel policy review or alternative arrangements
- **New hires (Year 1-2)**: Enhanced onboarding and mentoring programs

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib**: Static visualizations
- **Seaborn**: Statistical data visualization
- **Plotly**: Interactive visualizations
- **Jupyter Notebook**: Interactive analysis environment

## 📦 Installation

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab

### Setup

1. Clone or download this repository
```bash
git clone <repository-url>
cd Employee-Attrition-Analysis
```

2. Create a virtual environment (recommended)
```bash
python -m venv venv
On Windows: venv\Scripts\activate
```

3. Install required packages
```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

4. Download the dataset and place `HR_Analytics.csv` in the project directory

5. Launch Jupyter Notebook
```bash
jupyter notebook
```

## 🚀 Usage

1. Open `Employee_Attrition.ipynb` in Jupyter Notebook
2. Update the data path in the notebook to match your local directory
3. Run all cells sequentially to execute the analysis
4. View generated visualizations and insights

### Key Cells:
- **Cells 1-6**: Data loading and environment setup
- **Cells 7-15**: Data exploration and quality checks
- **Cells 16-25**: Univariate analysis
- **Cells 26+**: Bivariate analysis and interactive visualizations
- **Final Cells**: Summary statistics and business recommendations

## 📊 Conclusion

Employee attrition is a multifaceted issue influenced by multiple factors:

1. **Tenure is Critical**: The first 2 years are make-or-break; survival past this point indicates high retention likelihood
2. **Job Level Matters**: Entry-level employees (Level 1) account for 60% of attritions
3. **Age & Career Stage**: Mid-career employees (26-35 years old) show highest attrition
4. **Work Culture Issues**: Job satisfaction, environment satisfaction, and manager relationships are key
5. **Income is Secondary**: While important, salary is not the primary attrition driver
6. **Work-Life Balance**: Overtime and frequent travel significantly increase attrition risk

### Strategic Focus Areas:
- Strengthen Year 1-2 onboarding and mentorship
- Develop clear promotion pathways, especially for entry-level roles
- Improve work environment and satisfaction initiatives
- Review travel and overtime policies
- Build strong manager-employee relationships

## 📝 License

This project is provided as-is for educational and business analysis purposes.

## 👤 Author

Data Analysis Project | Employee Attrition Study

---

**Last Updated**: 2026
**Analysis Status**: Complete with actionable insights
