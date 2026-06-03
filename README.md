# Social Media Engagement — Exploratory Data Analysis (Python)

> Python-based EDA on a simulated social media usage dataset, examining patterns in user engagement, posting behavior, and follow dynamics across major platforms.

![Python](https://img.shields.io/badge/Python-3.x-3776AB) ![Pandas](https://img.shields.io/badge/Pandas-Yes-150458) ![Seaborn](https://img.shields.io/badge/Seaborn-Yes-2E97B8) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626)

---

## Business Question

How does user behavior vary across social media platforms — which apps drive higher engagement, what is the relationship between posting frequency and likes received, and are there detectable patterns between time spent on a platform and engagement outcomes?

## Dataset

- **Source:** Simulated social media usage dataset (1,000 users)
- **Variables:** User ID, App (Pinterest, Facebook, Instagram, Twitter, etc.), Daily Minutes Spent, Posts Per Day, Likes Per Day, Follows Per Day

## Approach

End-to-end exploratory data analysis in a Jupyter Notebook:

1. **Data inspection** — used pandas methods (`.head()`, `.tail()`, `.describe()`, `.info()`, `.shape`) to understand structure and distributions.
2. **Data quality checks** — used `missingno.matrix()` to visualize null patterns, checked for duplicates, examined skewness and kurtosis for each numeric variable.
3. **Aggregation** — grouped data by App to compare engagement metrics across platforms.
4. **Univariate analysis** — histograms, count plots, and distribution plots for each key variable.
5. **Bivariate analysis** — scatter plots, box plots, and regression plots to explore relationships between posting behavior, time spent, and engagement.
6. **Multivariate analysis** — Seaborn pairplot across four engagement variables, plus correlation heatmap to identify the strongest pairwise relationships.

## Tools & Techniques

- **pandas** — data manipulation, groupby aggregation, descriptive statistics
- **NumPy** — numerical operations
- **matplotlib** — base plotting
- **seaborn** — statistical visualizations (pairplot, distplot, boxplot, regplot, heatmap)
- **missingno** — missing-data visualization

## Files

- [`SocialMediaDataAnalysis.ipynb`](SocialMediaDataAnalysis.ipynb) — full notebook with code, visualizations, and observations
- [`social_media_usage.csv`](social_media_usage.csv) — source dataset (1,000 user records)

## How to Run

```bash
pip install pandas numpy matplotlib seaborn missingno
jupyter notebook SocialMediaDataAnalysis.ipynb
```

## Notes

This project was built as part of self-directed learning in Python-based data analysis, with a focus on practicing the standard EDA workflow before moving to dashboard tools like Power BI and Tableau.
