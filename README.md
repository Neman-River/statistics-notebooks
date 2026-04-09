# Statistics Notebooks

A statistics learning workspace covering descriptive statistics, probability theory, hypothesis testing, and inferential statistics through hands-on Jupyter notebooks.

## Notebooks

Ordered from foundational to advanced:

| # | Notebook | Topic | Dataset |
|---|----------|-------|---------|
| 01 | `01_descriptive_statistics.ipynb` | Central tendency, spread, distributions, box plots, trends over time | `games.csv` |
| 02 | `02_central_limit_theorem_CI.ipynb` | Central Limit Theorem, standard error, confidence intervals (z vs t) | simulated data |
| 03 | `03_hypothesis_testing.ipynb` | Hypothesis testing — metric distributions, spread analysis | `conversion.csv` |
| 04 | `04_t-test_annova.ipynb` | Z vs T scores, log transformation, Welch's t-test (CPC vs CPM), one-way ANOVA (platform comparison) | `ads_data.csv`* |
| 05 | `05_statistical_inference.ipynb` | London bike rentals time series — anomaly detection via rolling statistics and confidence intervals | `london.csv` |
| 06 | `06_ab_ttest.ipynb` | Full A/B test: group balance, normality testing on large samples (bootstrap stability, D'Agostino-Pearson), T-test / Mann-Whitney / Yuen / permutation test, effect size (Cohen's d) | `experiment_lesson_4.csv`* |
| 07 | `07_ab_test_anova.ipynb` | One-Way ANOVA (button color vs. likes): three approaches (scipy / statsmodels / pingouin), normality + Levene's test, Welch ANOVA, post-hoc comparisons (Bonferroni, Games-Howell); Two-Way ANOVA (ad style × age group): main effects, interaction term, interaction plot | `post_likes.csv`*, `ads_clicks.csv`* |

*Large datasets not tracked in git. Download separately and place in the project root.


## Stack

Python 3.12 · pandas · numpy · scipy · matplotlib · seaborn · plotly

## Running

```bash
uv run jupyter lab
```
