<img width="1324" height="744" alt="image" src="https://github.com/user-attachments/assets/90e935b7-3da5-4fac-b549-e13b8f63d7e7" />
# Student Performance Analysis Dashboard using Power BI
### Data collection done form : https://www.kaggle.com/datasets/rabieelkharoua/students-performance-dataset
### Project Overview

This project aims to analyze various factors that impact the academic performance of students. An interactive and insightful dashboard has been developed using Microsoft Power BI to visualize key metrics and uncover underlying trends from a student dataset.

The dashboard helps answer critical questions such as:
- How do study habits correlate with student GPA?
- What is the impact of demographic factors (like gender, ethnicity, parental education) on academic success?
- How do factors like tutoring, parental support, and absences affect student grades?

---

### Project Workflow

The project was executed following a structured data analysis process:

**1. Data Preparation and Cleaning (in Power Query Editor):**
- The initial raw data was imported as a single CSV/Excel file into Power BI.
- The primary query was duplicated to create two specialized tables: `Student_Demographics` and `Student_Performance`.
- In each table, irrelevant columns were removed to create clean, focused datasets.
- Data transformation was performed to replace numeric codes with descriptive text values for better readability and analysis (e.g., Gender `0` -> `"Female"`, Parental Support `2` -> `"Moderate Support"`).

**2. Data Modeling:**
- A relationship was established between the `Student_Demographics` and `Student_Performance` tables.
- A **one-to-one relationship** was created using the `StudentID` column as the primary key, ensuring a robust and accurate data model.

**3. DAX Implementation:**
- Custom calculations were written using DAX (Data Analysis Expressions) to add deeper analytical capabilities.
- **Measures** were created for key performance indicators.
- A **Calculated Column** was added to derive new insights from existing data.

---

### DAX Calculations

The following DAX formulas were implemented:

* **Measures:**
    * `Total Students = COUNTROWS('Student_Demographics')`
    * `Average GPA = AVERAGE('Student_Performance'[GPA])`

---

### Key Visualizations & Insights

The dashboard is composed of several key sections:
* **KPIs:** At-a-glance metrics such as Total Students, Average GPA, Average Weekly Study Time, and Total Absences.
* **Demographic Analysis:** Visual breakdowns of the student population by gender, ethnicity, and parental education level.
* **Performance Correlation:** A scatter plot visualizing the relationship between study hours and GPA.
* **Factor Impact Analysis:** Detailed charts showing the effect of parental support, tutoring, and absenteeism on student performance.
* **Grade Distribution:** A breakdown of students across different final grades (A, B, C, D, F).

---

### Tools Used
* **Microsoft Power BI**
    * Power Query Editor (for ETL)
    * Data Modeling
    * DAX
    * Reporting & Visualization
* **Microsoft Excel / CSV** (as the data source)


### How to Use
1.  Clone this repository to your local machine.
2.  Open the `.pbix` file in Power BI Desktop.
3.  If required, update the data source paths to connect to the provided CSV files on your machine.
