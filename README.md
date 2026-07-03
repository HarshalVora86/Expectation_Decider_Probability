<div align="center">

# Expectation Decider
### Probability-Based Student Pass Prediction Analysis

[![Python](https://img.shields.io/badge/Python-3.14-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy&logoColor=white)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)](https://matplotlib.org/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](#)

A probability and statistics project that analyzes student academic data to identify which factors most strongly influence the likelihood of passing a final exam.

</div>

---

## Project Overview

This project uses a dataset of 200 students to study how study hours, attendance, participation in group discussions, and previous test scores relate to the probability of passing a final exam. The notebook walks through probability fundamentals and builds up to conditional probability and Bayes' Theorem to quantify these relationships.

Video walkthrough: https://drive.google.com/file/d/1Fk5T5Bo4LBQqHmif8ZBcbVfNSn6pYqNz/view?usp=sharing

## Dataset

The dataset (`expectation_decider_dataset.csv`) contains 200 student records with the following columns:

- `student_id` - unique identifier for each student
- `study_hours` - weekly study hours
- `attendance` - class attendance percentage
- `group_discussion` - whether the student participated in group discussions (Yes/No)
- `previous_test_score` - score obtained in the previous test
- `final_exam_pass` - final exam result (Pass/Fail)

## Concepts Applied

- **Probability Basics** - calculating the probability of an event as favourable outcomes over total outcomes, applied to compute the overall probability of passing and failing.
- **Empirical vs. Theoretical Probability** - comparing probability derived from actual dataset observations against probability derived from logical assumptions.
- **Random Variables and Probability Distributions** - defining a random variable for the number of students passing out of 3 randomly selected students, and computing its full probability distribution.
- **Mean and Variance of a Random Variable** - calculating the expected value (mean) and variance of the probability distribution.
- **Set Theory and Venn Diagrams** - using set operations to visualize the overlap between students with high study hours and students with high attendance.
- **Contingency Tables** - cross-tabulating group discussion participation against final exam results.
- **Joint, Marginal, and Conditional Probability** - computing joint probability of two events occurring together, marginal probability of a single event, and conditional probability of one event given another.
- **Independent vs. Dependent Events** - testing whether group discussion participation and passing the exam are statistically independent, and identifying them as dependent events based on the data.
- **Bayes' Theorem** - applying Bayes' Theorem to calculate the probability of passing given high attendance, using prior and conditional probabilities.

## Key Findings

- Overall probability of passing the final exam: 65%
- Probability of passing given participation in group discussion: 81.82%
- Group discussion participation and passing are dependent events, not independent
- Probability of passing given high attendance (via Bayes' Theorem): 75.83%
- 80 students satisfied both conditions of studying more than 10 hours per week and attending more than 80% of classes

Based on these results, the factors most associated with a higher probability of passing are, in order of impact:

1. Group discussion participation
2. High attendance
3. Study hours
4. Previous test performance

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- matplotlib-venn

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

## Author

Harshal Vora
GitHub: https://github.com/HarshalVora86
LinkedIn: https://www.linkedin.com/in/harshal-vora-344601251/
