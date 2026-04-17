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
| 08 | `08_anova_case_study.ipynb` | A/B test case study in a food delivery app — **Case 1:** One-Way ANOVA (photo format 16:9 vs square vs 12:4), normality (Shapiro-Wilk, D'Agostino-Pearson, QQ plots), Levene's test, Tukey HSD / Games-Howell / Holm / FDR post-hoc; **Case 2:** Two-Way ANOVA (button redesign × customer segment), interaction effect, interaction plot, Tukey HSD on all combinations | `data/5_task_1.csv`*, `data/5_task_2.csv`* |
| 09 | `09_correlation&regression.ipynb` | Correlation analysis — **Part 1:** Pearson vs Spearman (covariance, normalization, when each applies); **Part 2:** California Housing — outlier filtering, log transform, correlation matrix heatmap; **Part 3:** Anscombe's Quartet — four datasets with identical $r \approx 0.816$ but radically different structures (why visualization must come before correlation) | built-in (`tips`, `california_housing`, `anscombe`) |
| 10 | `10_bootstrap.ipynb` | Bootstrap confidence intervals for non-normal/skewed data — **Part 1:** manual bootstrap (10 000 resamples) + `scipy.stats.bootstrap` for the median of one group; **Part 2:** bootstrap CI for the difference in medians between two groups; when bootstrap beats t-test and Mann-Whitney | `data/bootstrap_data.csv`* |
| 11 | `11_test_power.ipynb` | Statistical power and MDE — **Part 1:** sample size vs. power (1% effect, 1 000 simulated A/B tests per configuration); **Part 2:** effect size vs. power (10% effect at small n); visualization of the 80% power threshold; practical A/B test design workflow | simulated data |
| 12 | `12_abtest_practice.ipynb` | Driver churn analysis for a ride-hailing service — churn definition (30-day inactivity proxy); **H1:** churn vs phone type (Chi-square → Android churns more); **H2:** churn vs city (Chi-square → Astapor highest churn); **H3:** early activity across cities (D'Agostino-Pearson normality, Kruskal-Wallis); **H4:** churned vs retained early trip counts (Shapiro-Wilk, Mann-Whitney U → churned drivers make ~2× fewer trips in first 30 days); actionable recommendations + A/B test design outline | `data/churn.csv`* |
| 13 | `13_ab_simulation.ipynb` | A/B test simulation running day-by-day — **Scenario 1:** real effect (μ_experiment = 100.5 vs μ_control = 100, 10 days), tracking cumulative means and p-value trajectory; **Scenario 2:** no true effect (identical distributions, 100 days), illustrating false positive risk from early peeking; key takeaways on when to stop a test and two sample-size methods (MDE / power analysis vs empirical / historical data) | simulated data |

*Large datasets not tracked in git. Download separately and place in the project root.


## Stack

Python 3.12 · pandas · numpy · scipy · statsmodels · pingouin · matplotlib · seaborn · plotly

## Running

```bash
uv run jupyter lab
```
