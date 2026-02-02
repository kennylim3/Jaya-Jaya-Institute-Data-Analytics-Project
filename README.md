# Solving Business Problems in an EdTech Company

## Business Understanding
**Jaya Jaya Institute** is a higher education institution that has been operating since 2000 and has produced many graduates with strong reputations. However, the institute is currently facing a significant challenge: a high number of students fail to complete their studies and eventually drop out.

A high dropout rate can negatively impact institutional performance, student outcomes, and overall reputation. Therefore, Jaya Jaya Institute aims to **detect students who are at risk of dropping out as early as possible**, enabling the institution to provide targeted academic guidance and support.

As a prospective data scientist, this project aims to assist Jaya Jaya Institute in addressing this challenge through data analysis, machine learning, and visualization.

---

### Business Problem
Despite its strong academic reputation, Jaya Jaya Institute experiences a relatively high student dropout rate. The institution needs a data-driven approach to:

- Identify students who are likely to drop out at an early stage  
- Monitor student academic performance effectively  
- Support decision-making through clear and interpretable insights  

---

### Project Scope
To address the business problem, the project includes the following components:

1. **Business Dashboard**  
   - A dashboard is developed to help stakeholders monitor student performance and key academic indicators.

2. **Machine Learning Model Development**  
   - Three machine learning algorithms are evaluated:
     - Decision Tree  
     - Random Forest  
     - Gradient Boosting  

   - Model performance is compared to select the best-performing model for dropout prediction.

3. **Prototype Implementation**  
   - The selected machine learning model is deployed into a simple prototype system to predict students with a high probability of dropping out.

---

### Data Preparation

**Data Source**: https://raw.githubusercontent.com/dicodingacademy/dicoding_dataset/main/students_performance/data.csv

Setup environment:
```
pipenv install
pipenv shell
pip install pandas matplotlib seaborn sqlalchemy scikit-learn joblib numpy streamlit
```

## Business Dashboard

The dashboard is designed to help academic stakeholders quickly understand student conditions and performance trends. It includes:

- Total number and percentage of students by academic status (Dropout, Enrolled, Graduate)  
- Age distribution of students  
- Comparison of academic performance between the first and second semesters  

These visual insights support early identification of students who may require academic intervention.

---

## Exploratory Data Analysis (EDA) Insights

Key patterns identified from the analysis include:

- Students who **drop out** generally have:
  - Lower admission grades  
  - Higher average age  
  - Fewer enrolled curricular units in both semesters  
  - Fewer approved curricular units in both semesters  
  - Lower average grades in both the first and second semesters  

- No meaningful patterns were observed in the following features:
  - Application order  
  - Previous qualification grade  
  - Credited curricular units  
  - Evaluated and non-evaluated curricular units (both semesters)  

- **Graduate students** tend to be **displaced**, while **dropout students** are more commonly non-displaced.

- No strong correlations were observed in demographic and socio-economic attributes such as:
  - Marital status  
  - Application mode  
  - Course  
  - Attendance schedule  
  - Previous qualification  
  - Nationality  
  - Parents’ education and occupation  
  - Educational special needs  
  - Financial status  
  - Gender  
  - Scholarship holder status  
  - International student status  

---

## Conclusion

The analysis indicates that **academic performance variables** are the strongest indicators of student dropout risk. Students with lower grades, fewer approved courses, and weaker academic engagement are significantly more likely to drop out.

In contrast, demographic and socio-economic factors show limited predictive power when compared to academic indicators.

---

## Actionable Recommendations

Based on the findings, the following actions are recommended for Jaya Jaya Institute:

- **Early Academic Intervention**  
  Identify students with low or declining academic performance early and provide tutoring, mentoring, or remedial programs.

- **Targeted Support for Older Students**  
  Older students may face additional challenges such as work or family responsibilities. Providing flexible learning support or personalized counseling can help reduce dropout risk.

- **Continuous Performance Monitoring**  
  Utilize dashboards and predictive models to continuously monitor student progress and proactively flag students at high risk of dropout.
