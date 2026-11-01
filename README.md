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

### Option 1 – Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `Lab01_Big_Data_Processing_with_PySpark.ipynb` and the CSV file.
3. Run the cells in order. The first cell installs PySpark if needed.

### Option 2 – Local

```bash
pip install pyspark findspark
# Make sure Java 8/11/17+ is installed
jupyter notebook Lab01_Big_Data_Processing_with_PySpark.ipynb
```

## Lab Requirements Covered

### PySpark DataFrame Operations (≥ 3)

1. **Exploration** – `printSchema()`, `describe()`, distinct counts
2. **Filtering + Ordering** – Failures in EEI6366, high performers in Colombo
3. **GroupBy + Aggregations** – Average marks & pass rate by Center and by Course
4. **Bonus** – Derived column (`ca_exam_gap`) + Window ranking (Top 3 per course)

### Spark SQL Operations (≥ 3)

1. Pass rate & average marks by Academic Year + Center
2. Grade distribution for EEI6366 with ordered CASE
3. Window function – difference from center average
4. Pattern discovery – strong CA but weak Exam students

## Key Insights

- High overall pass rate (~90%).
- Performance differs across regional centers.
- A subset of students score well in Continuous Assessment but poorly in the Final Exam – useful for academic support interventions.
- Window functions and multi-level aggregations work efficiently even on 150k+ rows.

## Repository Structure

```
├── README.md
├── Lab01_Big_Data_Processing_with_PySpark.ipynb   # Main notebook
└── open_university_student_performance.csv       # Dataset
```

## Author / Group

Prepared for EEI6366 Lab 01.

---

**GitHub:** https://github.com/missarii/Big-Data-Processing-with-PySpark
