# Big Data Processing with PySpark

**EEI6366 | Lab 01: Big Data Processing with PySpark**

This repository contains the practical exploration of a large student performance dataset using **PySpark DataFrame API** and **Spark SQL**.

## Dataset

- **File:** `open_university_student_performance.csv`
- **Rows:** 150,500 (well above the 100,000 minimum requirement)
- **Columns:**
  - `student_id`
  - `course_code` (6 courses including EEI6366 - Big Data Processing)
  - `academic_year` (2023/2024, 2024/2025, 2025/2026)
  - `center` (Colombo, Kandy, Matara, Jaffna, Kurunegala, Batticaloa)
  - `continuous_assessment_mark`
  - `final_exam_mark`
  - `overall_mark`
  - `grade`
  - `status` (Pass / Fail)

## How to Run

### Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `Lab01_Big_Data_Processing_with_PySpark.ipynb` and the CSV file.
3. Run the cells in order. The first cell installs PySpark if needed.

## Lab Requirements Covered

### PySpark DataFrame Operations (4)

1. Basic Exploration & Descriptive Statistics  
2. Filtering and Ordering  
3. GroupBy and Aggregations  
4. Derived Column and Window Ranking  

### Spark SQL Operations (4)

1. Filtering and Aggregation  
2. Grade Distribution with CASE  
3. Window Function  
4. Finding Interesting Patterns  

## Repository Structure

```
├── README.md
├── Lab01_Big_Data_Processing_with_PySpark.ipynb
└── open_university_student_performance.csv   (upload this yourself)
```

**GitHub:** https://github.com/missarii/Big-Data-Processing-with-PySpark
