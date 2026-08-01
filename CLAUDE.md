# CLAUDE.md

Teaching fork of `intro-stat-learning/ISLP_labs` — course "Introduction to
Statistical Learning with Python" (Constantin Lisson, BSc Data Science,
EBS Universität). All labs run in Google Colab; workflow in
`Ch00-course-introduction.ipynb`.

## Branch model

- **`main`** — permanent home of the course material (upstream content +
  Colab adaptations). Every change lands here, normally via PR.
- **`<year>-<term>`** (e.g. `2026-fall`) — frozen, student-facing semester
  snapshot of `main`. All Colab badges point at the current semester branch.
  Advance it only deliberately (fast-forward from `main`) when a fix should
  reach students; never rewrite it mid-term. Old semester branches are kept
  as archives of what each cohort saw.
- **`claude/*`** — temporary dev/session branches. PR into `main`, delete
  after merge.

Between semesters: sync upstream into `main`, resolve conflicts (they
cluster in the notebook title/setup cells and README), update the term
line and badge URLs (grep for the old branch name), then cut the new
semester branch from `main`.
