# Statistics Notebooks

A statistics learning workspace covering descriptive statistics, probability theory, hypothesis testing, and inferential statistics through hands-on Jupyter notebooks.

## Notebooks

| Notebook | Topic | Dataset |
|----------|-------|---------|
| `descriptive_statistics.ipynb` | Central tendency, spread, distributions, box plots, trends over time | `games.csv` |
| `central_limit_theorem_CI.ipynb` | Central Limit Theorem, standard error, confidence intervals (z vs t) | simulated data |
| `hypothesis_testing.ipynb` | Hypothesis testing — metric distributions, spread analysis | `conversion.csv` |
| `statistical_inference.ipynb` | London bike rentals time series — anomaly detection via rolling statistics and confidence intervals | `london.csv` |
| `t-test_annova.ipynb` | Z vs T scores, log transformation, Welch's t-test (CPC vs CPM), one-way ANOVA (platform comparison) | `ads_data.csv`* |

*`ads_data.csv` is not tracked in git (235 MB). Download separately and place in the project root.

## Stack

Python 3.12 · pandas · numpy · scipy · matplotlib · seaborn · plotly

## Running

```bash
uv run jupyter lab
```
