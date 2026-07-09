# Expectation Decider: Probability-Based Student Pass Prediction Analysis

A statistics/probability mini-project applying core probability theory to a student performance dataset to identify which factors are associated with passing a final exam.

## Video Explanation

[Watch the project walkthrough](https://drive.google.com/file/d/1Fk5T5Bo4LBQqHmif8ZBcbVfNSn6pYqNz/view?usp=sharing)

## Dataset

`expectation_decider_dataset.csv` — 200 students, 6 columns:

| Column | Description |
|---|---|
| student_id | Unique student identifier |
| study_hours | Hours studied per week |
| attendance | Attendance percentage |
| group_discussion | Participated in group discussion (Yes/No) |
| previous_test_score | Score on previous test |
| final_exam_pass | Final exam result (Pass/Fail) |

## Concepts Covered

- **Probability basics** — P(Event) = Favourable Outcomes / Total Outcomes
- **Key terminology** — experiment, trial, outcome, sample space, event
- **Empirical vs. theoretical probability**
- **Random variables & probability distribution** — distribution of number of students passing out of 3 randomly selected students, with mean and variance
- **Venn diagrams** — study hours vs. attendance overlap
- **Contingency tables** — group discussion vs. exam result
- **Joint, marginal, and conditional probability**
- **Independence of events**
- **Bayes' Theorem**

## Analysis & Results

**Overall pass probability**
P(Pass) = 130 / 200 = **65%**

**Probability distribution — number of students (X) passing out of 3 randomly selected**

| X | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| P(X) | 0.043 | 0.239 | 0.443 | 0.275 |

Mean E[X] = 1.95, Variance = 0.6826

**Venn diagram (study hours > 10/week vs. attendance > 80%)**
- Study hours only: 25
- Attendance only: 38
- Both: 80
- Neither: 57

**Contingency table — group discussion vs. result**

| | Pass | Fail | Total |
|---|---|---|---|
| Group discussion: Yes | 90 | 20 | 110 |
| Group discussion: No | 40 | 50 | 90 |
| Total | 130 | 70 | 200 |

- Joint probability P(Group Discussion = Yes ∩ Pass) = 90/200 = 0.45
- Marginal probability P(Pass) = 130/200 = 0.65
- Conditional probability P(Pass | Group Discussion = Yes) = 90/110 = 0.818 (81.8%)

Since P(Pass | Group Discussion = Yes) ≠ P(Pass), group discussion and passing are **dependent events**. They are not mutually exclusive, since a student can both participate in group discussion and pass.

**Bayes' Theorem**

Given P(High Attendance | Pass) = 0.70, P(High Attendance | Fail) = 0.40, P(High Attendance) = 0.60, P(Pass) = 0.65:

P(Pass | High Attendance) = [P(High Attendance | Pass) × P(Pass)] / P(High Attendance) = (0.70 × 0.65) / 0.60 = **0.7583 (75.83%)**

## Conclusion

- Overall probability of passing: 65%
- Students who participated in group discussion: 81.82% pass probability
- Students with high attendance: 75.83% pass probability (via Bayes' Theorem)
- Group discussion and attendance are the strongest factors associated with passing in this dataset

## Files

| File | Description |
|---|---|
| `Expectation_Decider_Probability_Analysis_ipynb.ipynb` | Full analysis notebook (pandas, numpy, matplotlib, matplotlib_venn) |
| `expectation_decider_dataset.csv` | Source dataset (200 records) |
| `Expectation_Decider_Probability.pdf` | Handwritten notes covering the probability theory behind the analysis |

## Tools Used

Python, pandas, numpy, matplotlib, matplotlib_venn

## Author

Harshal Vora
GitHub: https://github.com/HarshalVora86
LinkedIn: https://www.linkedin.com/in/harshal-vora-344601251/
