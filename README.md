# Introduction to Statistical Learning with Python — Lab Notebooks

**BSc Data Science · EBS Universität · Fall Term 2026**

**Instructor:** Constantin Lisson

Lab notebooks for the course, accompanying
[*An Introduction to Statistical Learning, with Applications in Python*](https://www.statlearning.com)
by James, Witten, Hastie, Tibshirani and Taylor. All labs run in
**Google Colaboratory** — nothing to install, any device with a browser works.
A **Google account is required**.

## Start here

Read the course introduction notebook first. It explains the workflow, the
Google-account requirement, and the limits of Colab's free tier, and ends
with a setup check to run before the first session:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch00-course-introduction.ipynb) **Ch00 — Course Introduction and Setup**

**In short:** click a lab's badge below → in Colab choose **File → Save a
copy in Drive** → run the *Google Colab setup* cell at the top → work
top-to-bottom. Your work lives in your own Drive copy; the master copies
here stay clean, and clicking a badge again always gives you a fresh start.

## The labs

| Lab | Topic | Open in Colab |
|-----|-------|---------------|
| Ch02 | Introduction to Python | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch02-statlearn-lab.ipynb) |
| Ch03 | Linear Regression | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch03-linreg-lab.ipynb) |
| Ch04 | Logistic Regression, LDA, QDA, and KNN | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch04-classification-lab.ipynb) |
| Ch05 | Cross-Validation and the Bootstrap | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch05-resample-lab.ipynb) |
| Ch06 | Linear Models and Regularization Methods | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch06-varselect-lab.ipynb) |
| Ch07 | Non-Linear Modeling | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch07-nonlin-lab.ipynb) |
| Ch08 | Tree-Based Methods | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch08-baggboost-lab.ipynb) |
| Ch12 | Unsupervised Learning | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lissonc/islp/blob/2026-fall/Ch12-unsup-lab.ipynb) |

Lab numbers follow the book's chapters, so the list skips the chapters that
are not part of this course.

All links point to the frozen `2026-fall` branch, so lab content will not
change under you during the term.

## Backup options

If you cannot use Google Colab, contact the instructor. The labs also run in
[GitHub Codespaces](https://codespaces.new/lissonc/islp), and experienced
students can set up a local environment with Python 3.12 and
`pip install -r requirements.txt` (exact pinned package versions).

## Credits and license

These labs were written by the ISLP authors — Trevor Hastie, Gareth James,
Jonathan Taylor, Robert Tibshirani and Daniela Witten. This repository is a
teaching fork of
[intro-stat-learning/ISLP_labs](https://github.com/intro-stat-learning/ISLP_labs)
that only adds course-specific setup for running the labs in Google Colab.
Distributed under the BSD 2-Clause License (see [LICENSE](LICENSE)).
