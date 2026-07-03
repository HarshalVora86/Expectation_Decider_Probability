<div align="center">

# Expectation Decider

### Probability-Based Student Pass Prediction Analysis

*Applying core probability theory to a real dataset to quantify what actually drives exam success.*

[![Python](https://img.shields.io/badge/Python-3.14-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge)](https://matplotlib.org/)

[![Last Commit](https://img.shields.io/github/last-commit/HarshalVora86/Expectation_Decider_Probability?style=flat-square&color=informational)](https://github.com/HarshalVora86/Expectation_Decider_Probability/commits/main)
[![Repo Size](https://img.shields.io/github/repo-size/HarshalVora86/Expectation_Decider_Probability?style=flat-square&color=informational)](https://github.com/HarshalVora86/Expectation_Decider_Probability)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)](#)

[Watch Project Walkthrough](https://drive.google.com/file/d/1Fk5T5Bo4LBQqHmif8ZBcbVfNSn6pYqNz/view?usp=sharing) &nbsp;|&nbsp; [View Notebook](./Expectation_Decider_Probability_Analysis.ipynb) &nbsp;|&nbsp; [View Dataset](./expectation_decider_dataset.csv)

</div>

<br>

## Table of Contents

- [Project Overview](#project-overview)
- [Key Metrics at a Glance](#key-metrics-at-a-glance)
- [Dataset](#dataset)
- [Analysis Workflow](#analysis-workflow)
- [Concepts Applied](#concepts-applied)
- [Key Findings](#key-findings)
- [Tools and Libraries](#tools-and-libraries)
- [Repository Structure](#repository-structure)
- [How to Run](#how-to-run)
- [Author](#author)

<br>

## Project Overview

This project uses a dataset of 200 students to study how study hours, attendance, participation in group discussions, and previous test scores relate to the probability of passing a final exam. The notebook walks through probability fundamentals and builds up to conditional probability and Bayes' Theorem to quantify these relationships and identify the strongest predictors of success.

> **Core question:** Which measurable student behaviors most increase the probability of passing the final exam, and by how much?

<br>

## Key Metrics at a Glance

<div align="center">

| Metric | Value |
|---|---|
| Students Analyzed | **200** |
| Overall Pass Probability | **65%** |
| Pass Probability with Group Discussion | **81.82%** |
| Pass Probability given High Attendance (Bayes) | **75.83%** |
| Students with High Study Hours and Attendance | **80** |

</div>

<br>

## Dataset

The dataset (`expectation_decider_dataset.csv`) contains 200 student records with the following columns:

| Column | Description |
|---|---|
| `student_id` | Unique identifier for each student |
| `study_hours` | Weekly study hours |
| `attendance` | Class attendance percentage |
| `group_discussion` | Participation in group discussions (Yes/No) |
| `previous_test_score` | Score obtained in the previous test |
| `final_exam_pass` | Final exam result (Pass/Fail) |

<br>

## Concepts Applied

- **Probability Basics** — calculating the probability of an event as favourable outcomes over total outcomes, applied to compute the overall probability of passing and failing.
- **Empirical vs. Theoretical Probability** — comparing probability derived from actual dataset observations against probability derived from logical assumptions.
- **Random Variables and Probability Distributions** — defining a random variable for the number of students passing out of 3 randomly selected students, and computing its full probability distribution.
- **Mean and Variance of a Random Variable** — calculating the expected value (mean) and variance of the probability distribution.
- **Set Theory and Venn Diagrams** — using set operations to visualize the overlap between students with high study hours and students with high attendance.
- **Contingency Tables** — cross-tabulating group discussion participation against final exam results.
- **Joint, Marginal, and Conditional Probability** — computing joint probability of two events occurring together, marginal probability of a single event, and conditional probability of one event given another.
- **Independent vs. Dependent Events** — testing whether group discussion participation and passing the exam are statistically independent, and identifying them as dependent events based on the data.
- **Bayes' Theorem** — applying Bayes' Theorem to calculate the probability of passing given high attendance, using prior and conditional probabilities.

<br>

## Key Findings

- Overall probability of passing the final exam: **65%**
- Probability of passing given participation in group discussion: **81.82%**
- Group discussion participation and passing are **dependent events**, not independent
- Probability of passing given high attendance, via Bayes' Theorem: **75.83%**
- **80 students** satisfied both conditions of studying more than 10 hours per week and attending more than 80% of classes

Based on these results, the factors most associated with a higher probability of passing are, in order of impact:

1. Group discussion participation
2. High attendance
3. Study hours
4. Previous test performance

<br>

## Tools and Libraries

<div align="center">

| Category | Technology |
|---|---|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, matplotlib-venn |
| Environment | Jupyter Notebook |

</div>

<br>

## How to Run

1. Clone the repository
   ```
   git clone https://github.com/HarshalVora86/Expectation_Decider_Probability.git
   ```
2. Install the required libraries
   ```
   pip install pandas numpy matplotlib matplotlib-venn
   ```
3. Open `Expectation_Decider_Probability_Analysis.ipynb` in Jupyter Notebook and run the cells sequentially.

<br>

## Author

<div align="center">

**Harshal Vora**

[![GitHub](https://img.shields.io/badge/GitHub-HarshalVora86-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/HarshalVora86)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/harshal-vora-344601251/)

</div>
