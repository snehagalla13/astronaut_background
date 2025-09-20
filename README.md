**Overview**

This project analyzes astronaut education data and college admissions data to explore relationships between college attendance, parental income, and astronaut profiles. The goal is to aggregate student-level data, match it with astronaut college records, and generate summary statistics and visualizations.

**Data**

The project uses three main datasets:
- CollegeAdmissions_Data.csv=
  - Contains student-level college admissions data.
  - Key columns:
    - name: College name
    - par_income_bin: Parental income group
    - attend: Frequency of students attending per income group
- astronauts colleges.csv
  - Contains astronaut names and the colleges they attended.
  - Key column: Name
- Social_Science.csv
  - Contains astronaut profile information.
  - Key column: Profile.Name

**Features**

The Python code performs the following tasks:
- Data Cleaning & Name Formatting
  - Standardizes astronaut names from First MI. Last → Last, First MI.
  - Removes duplicate astronaut profiles
- Aggregation
  - Calculates income_group*attendance per student
  - Aggregates totals per college
- Matching
  - Matches astronaut colleges to aggregated college totals
  - Creates Income Group by College for astronauts
- Summary Statistics
  - Computes max, min, mean, and median of income_group*attendance per college
  - Identifies which colleges correspond to the max/min totals
- Visualization
  - Generates a box plot summarizing the distribution of income_group*attendance across all colleges

**Code Structure**

astronauts_background.ipynb
- Contains all code for cleaning, aggregation, matching, and analysis

CollegeAdmissions_Data.csv

astronauts colleges.csv

Social_Science.csv
