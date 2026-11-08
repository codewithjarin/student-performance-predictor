# Student Performance Predictor

This project predicts a student's final grade (0-20) using study habits, family details and absences.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/codewithjarin/student-performance-predictor/blob/main/student_performance_predictor.ipynb)

## Dataset

UCI Student Performance dataset (math course). 395 students.

## What I did

1. Loaded and explored the data
2. Removed G1 and G2 (earlier grades) so the model uses habits, not old marks
3. Trained two models: Linear Regression and Random Forest
4. Checked them using MAE and R²

## Results

| Model | MAE (lower is better) | R² (higher is better) |
|---|---|---|
| Linear Regression | 3.40 | 0.14 |
| Random Forest | 2.97 | 0.31 |

Random Forest is better. Absences and failures are the most important features.

## Limits

- Small dataset (395 students, two schools in Portugal)
- Weak at very low and very high marks

## How to run

Click the Colab badge, then choose Runtime → Run all.
Upload `student-mat.csv` if it asks for a file.

## Tools

Python, pandas, scikit-learn, matplotlib
