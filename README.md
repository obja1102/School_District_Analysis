# Pinehill School District Analytics Portal

An end-to-end Business Intelligence project demonstrating how Python, Tableau, and data analytics can support strategic decision-making within a K–12 school district.

**Live Dashboard:**  
▶[ https://public.tableau.com/views/tabschool/Dashboard1?:language=en-US&publish=yes](https://public.tableau.com/shared/5HXJF8QT3?:display_count=n&:origin=viz_share_link)

> **Note:** All data in this project is fictional and was created for portfolio and demonstration purposes. Pinehill School District is not a real organization.





![Landing Page](screenshots/landing_page.png)

---

# Project Overview

School districts collect data from multiple operational systems, including student information, assessments, human resources, attendance, and finance. These systems often operate independently, making it difficult for leadership to identify district-wide trends and make informed decisions.

This project simulates a 12-school district (approximately 7,500 students) and demonstrates how data from multiple sources can be transformed into an executive analytics platform.

The final solution is a role-based Tableau application designed for three primary stakeholders.

| Dashboard | Purpose |
|-----------|---------|
| **Superintendent** | District-wide performance, staffing, attendance, and budget monitoring with KPI cards, drill-down analysis, and year-over-year comparisons. |
| **Principal** | School-level performance benchmarking, subgroup achievement, attendance, staffing, and budget analysis. |
| **Human Resources** | Teacher turnover, vacancies, hiring timelines, professional development spending, and staffing trends. |

---

# Technology Stack

- **Python**
  - pandas
  - NumPy
  - Jupyter Notebook

- **Tableau**
  - Interactive dashboards
  - Dashboard navigation
  - Parameter actions
  - KPI scorecards
  - Heatmaps
  - Drill-down dashboards

- **Data Engineering**
  - Data cleaning
  - Feature engineering
  - Data validation
  - Multi-source integration
  - Tableau-ready dataset creation

---

# Data Pipeline

```
Raw Source Files
(Student Information, Assessments,
HR, Budget, Attendance)

        │
        ▼

Python Data Preparation

• Validation
• Cleaning
• Data Quality Checks
• Feature Engineering
• Record Reconciliation

        │
        ▼

7 Tableau-Ready CSV Files

        │
        ▼

Interactive Analytics Portal
```

---

# Data Quality Highlights

Significant effort was dedicated to validating and preparing the data prior to visualization.

Major corrections included:

- Corrected a major budget allocation error where a misplaced decimal created an unrealistic **952% Books & Supplies allocation** for Elm Elementary.
- Reconciled missing school identifiers across multiple source systems after discovering Dogwood Elementary was absent from the site crosswalk.
- Removed duplicate academic records.
- Identified undocumented race classifications affecting approximately **3.8%** of student records.
- Standardized categorical values, date formats, and school identifiers across all datasets.
- Engineered additional analytical metrics including:
  - Chronic absenteeism
  - Per-pupil spending
  - Intervention funding per student in need

Because several operational systems existed at different levels of detail, student-level integration was only possible within SIS data. Budget, HR, and staffing analyses were therefore performed at the school level.

---

# Key Findings

## Student Achievement

- English Learner (EL) percentage demonstrated the strongest negative relationship with academic performance (**r = -0.98**).
- Demographic and attendance variables collectively explained **94%** of the variation in school achievement (**R² = 0.94**).

## Resource Allocation

Intervention funding was not consistently aligned with student need.

Funding ranged from **$625 to $2,005 per student requiring intervention**, indicating opportunities for a more equitable funding strategy.

## Staffing

Teacher turnover showed a statistically significant relationship with chronic absenteeism (**r = 0.65**).

Schools with higher turnover generally experienced lower student engagement.

## Professional Development

Professional development spending was the only budget category significantly associated with lower teacher turnover (**r = -0.59**).

Schools investing the least in professional development experienced the highest turnover rates.

---

# Recommendations

Based on the analysis, two district priorities emerged:

### Standardize Intervention Funding

Develop a district-wide funding model that allocates intervention resources according to demonstrated student need.

### Increase Professional Development Investment

Prioritize professional development funding at high-turnover schools to improve staff retention and long-term student outcomes.

---

# Limitations

- Small district sample (12 schools)
- Two years of staffing and financial data
- Limited budget variation
- Strong collinearity between EL% and Free Lunch%
- Results identify relationships rather than causal effects

These findings should be used to guide future investigation rather than serve as definitive policy recommendations.

---

# Repository Structure

```
├── README.md
├── notebooks/
│   └── pinehill_data_cleaning_analysis.ipynb
│
├── data/
│   └── clean/
│
├── dashboards/
│   └── Pinehill School District Analytics Portal.twbx
│
├── presentation/
│   └── Pinehill Analysis and Recommendations.pptx
│
└── screenshots/
```

---

# Dashboard Preview

### Superintendent Dashboard



https://github.com/user-attachments/assets/f73b49f4-672e-4802-b855-1921519afe03









---

### Human Resources Dashboard



https://github.com/user-attachments/assets/9c55c214-e876-445b-b8fe-d46219b686c9


---

### Principal Dashboard




https://github.com/user-attachments/assets/ff77e954-85d2-49fe-8270-73f6bdca5584



# Skills Demonstrated

- Business Intelligence
- Data Cleaning
- Data Validation
- Feature Engineering
- Exploratory Data Analysis
- Dashboard Design
- Executive Reporting
- Tableau
- Python
- pandas
- Data Storytelling

---

Created by **Jared Oberg**

Python • Tableau • Business Intelligence • Data Analytics

2026

