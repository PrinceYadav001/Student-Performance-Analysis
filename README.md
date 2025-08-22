# Student Performance Analysis Dashboard using Power BI

<img width="1373" height="771" alt="image" src="https://github.com/user-attachments/assets/eb764aa0-c3b1-49f5-8b5c-cac2a5f75f28" />

### Data collection done from: https://www.kaggle.com/datasets/rabieelkharoua/students-performance-dataset

---

### Project Overview

This project aims to analyze various factors that impact the academic performance of students. An interactive and insightful dashboard has been developed using Microsoft Power BI to visualize key metrics and uncover underlying trends from a student dataset.

The dashboard helps answer critical questions such as:
- How do study habits correlate with student GPA?
- What is the impact of demographic factors (like gender, ethnicity, and parental education) on academic success?
- How do factors like tutoring, parental support, and absences affect student grades?

---

### Project Workflow

The project was executed following a structured data analysis process:

**1. Data Preparation and Cleaning (in Power Query Editor):**
- The initial raw data was imported as a single CSV file into Power BI.
- The primary query was duplicated to create two specialized tables: `Student_Demographics` and `Student_Performance`.
- In each table, irrelevant columns were removed to create clean, focused datasets.
- Data transformation was performed to replace numeric codes with descriptive text values for better readability and analysis (e.g., Gender `0` -> `"Female"`, Parental Support `2` -> `"Moderate Support"`).

**2. Data Modeling:**
- A **one-to-one relationship** was established between the `Student_Demographics` and `Student_Performance` tables using the `StudentID` column, ensuring a robust and accurate data model.

**3. Custom Calculations & Metrics:**
- To enhance the analysis, custom calculations were created for key performance indicators.
- Dynamic **measures** were developed to calculate aggregate values like **Total Students** and **Average GPA**, which respond to user interactions and filters on the dashboard.

---

### Key Visualizations & Insights

The dashboard is composed of several key sections:
* **KPIs:** At-a-glance metrics such as **Total Students**, **Average GPA**, **Average Weekly Study Time**, and **Total Absences**.
* **Demographic Analysis:** Visual breakdowns of the student population by gender, ethnicity, and parental education level.
* **Performance Correlation:** A scatter plot visualizing the relationship between study hours and GPA.
* **Factor Impact Analysis:** Detailed charts showing the effect of parental support, tutoring, and absenteeism on student performance.
* **Grade Distribution:** A breakdown of students across different final grades (A, B, C, D, F).

---

### Tools Used
* **Microsoft Power BI**
    * Power Query Editor (for ETL)
    * Data Modeling
    * Reporting & Visualization
* **Microsoft Excel / CSV** (as the data source)

---

### How to Use
1. Clone this repository to your local machine.
2. Open the `.pbix` file in Power BI Desktop.
3. If required, update the data source paths to connect to the provided CSV files on your machine.
