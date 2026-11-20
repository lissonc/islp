# CLAUDE.md

Teaching fork of `intro-stat-learning/ISLP_labs` — course "Introduction to
Statistical Learning with Python" (Constantin Lisson, BSc Data Science,
EBS Universität). All labs run in Google Colab; workflow in
`Ch00-course-introduction.ipynb`.

## Branch model

- **`main`** — permanent, term-independent home of the course material
  (upstream content + Colab adaptations + general fixes). Keeps the full
  set of material, including chapters a given semester leaves out.
- **`<year>-<term>`** (e.g. `2026-fall`) — student-facing semester branch,
  cut from `main` and then tailored for that term: de-scoped chapters or
  sections, term line, badge URLs, term-specific edits. It may stay
  permanently different from `main`. All Colab badges point at the current
  semester branch. Never rewrite its history; old semester branches are
  kept as archives of what each cohort saw.
- **`claude/*`** (and other feature branches) — temporary branches. PR into
  whichever branch the change belongs to, delete after merge.

### Where a change goes

- **General change** (bug fix, upstream sync, improvement to the material
  as such): feature branch → PR into `main`. To give it to students, carry
  it into the semester branch (see below).
- **Semester-specific change** (de-scoping, term dates, edits only right
  for this cohort): feature branch cut from the semester branch → PR
  directly into the semester branch. It never goes to `main`.
- **Never merge a semester branch into `main`** — that would apply its
  de-scoping to `main`.

### Carrying fixes from `main` into a semester branch

- **Single fix mid-term (preferred):** `git cherry-pick <commit>` onto a
  feature branch cut from the semester branch, PR into the semester branch.
  Brings only that commit.
- **Bulk update:** merge `main` into the semester branch. Changes since the
  last common point apply; chapters deleted on the semester branch stay
  deleted (if `main` edited one, resolve the modify/delete conflict by
  keeping the deletion). Caveat: files *newly added* to `main` come along —
  remove them in the merge (`git merge main --no-commit`, `git rm`, commit)
  if they should not reach students.
- `git log <semester>..main` lists what `main` has that students don't.

Between semesters: sync upstream into `main`, resolve conflicts (they
cluster in the notebook title/setup cells and README), then cut the new
semester branch from `main` and apply that term's tailoring there (term
line, badge URLs — grep for the old branch name — and de-scoping).
