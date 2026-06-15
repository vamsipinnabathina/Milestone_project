# Attendance Certification System using ML

A milestone project that builds an attendance tracking and certification system for 980 students participating in an ML internship, using machine learning to predict certification eligibility.

## Problem Statement

- 980 students participated in 40 ML internship sessions.
- A student is **certified** if their attendance is **≥ 80%** (i.e., attended at least 32 out of 40 sessions).
- Total attendance records: 980 students × 40 sessions = 39,200 entries.

## Project Workflow

1. **Data Collection** – Generated attendance records (39,200 rows) capturing each student's presence/absence across 40 sessions.
2. **EDA & Preprocessing** – Checked for duplicates and missing values, then aggregated raw records into a student-level summary (980 rows) with total sessions attended, attendance percentage, and certification label.
3. **Visualization** – Scatter plot of attendance percentage per student, color-coded by certification status, with an 80% threshold line.
4. **Model Building** – Trained a Logistic Regression classifier to predict certification status from attendance data.
5. **Evaluation** – Achieved 100% accuracy on the test set (certification is a direct function of attendance percentage).

## Files

- `Attendance_Certification_ML_Project.ipynb` – Complete Jupyter notebook with all steps.
- `attendance_raw.csv` – Raw session-level attendance data (39,200 rows).
- `student_summary.csv` – Aggregated student-level summary (980 rows) with attendance %, certified label.
- `attendance_scatter.png` – Scatter plot visualization of certified vs not-certified students.
- `certification_model.pkl` – Trained Logistic Regression model.

## Results

- **Certified students:** 410
- **Not certified students:** 570
- **Model accuracy:** 100%

## How to Run

1. Open `Attendance_Certification_ML_Project.ipynb` in Jupyter Notebook or Google Colab.
2. Run all cells (Runtime → Run all / Cell → Run All).
3. The notebook generates data, performs EDA, plots results, and trains the model — all in one run.

## Tech Stack

- Python
- pandas, numpy
- matplotlib
- scikit-learn
- joblib

## Author

S.Shivakumar
