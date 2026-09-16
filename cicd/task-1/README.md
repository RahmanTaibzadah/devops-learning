# Task 1: CI Pipeline

## What I built
A basic CI pipeline using GitHub Actions that automatically runs unit tests
on every push and pull request to the `main` branch.

The pipeline:
- Checks out the code
- Sets up Python 3.11
- Installs dependencies (pytest) from requirements.txt
- Runs the test suite with pytest

## App used
A tiny Python calculator app (`calculator.py`) with two functions (`add`, `subtract`),
tested with `test_calculator.py`.

## Pipeline file
See `.github/workflows/ci.yml` (copy also included in this folder as `ci.yml`).

## Screenshots
See `../screenshots/` for the pipeline passing in the GitHub Actions tab.

## What I learnt
- How GitHub Actions triggers on push/PR events
- How workflow YAML is structured (jobs, steps, runs-on)
- The difference between running tests locally vs in CI
- Why .gitignore matters (accidentally committed __pycache__ files)

## Issues I solved
- Initially committed Python __pycache__ files by mistake — fixed by adding
  a .gitignore and removing them from tracking with `git rm -r --cached`.
