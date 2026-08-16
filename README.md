# Disney_Genre_Revenue_Analysis

## Authors
Maram Elayan, Bar Weiss-Gill

---

## Project Description
This project investigates the association between movie genre and commercial performance for Disney films. Using a dataset covering releases from 1937 to 2016, we employed various statistical and machine learning techniques to assess whether revenue differs significantly across genres and to evaluate the predictive power of genre on blockbuster success.

---

## Research Question
**Are inflation-adjusted box office revenues significantly different across Disney movie genres?**

---

## Dataset
**Source:** [Kaggle - Disney Movies 1937-2016 Gross Income](https://www.kaggle.com/datasets/rashikrahmanpritom/disney-movies-19372016-total-gross)

**Dataset Summary:**
- **Original dataset:** 579 movies.
- **Analytical sample:** 562 movies (17 films with missing genre information were excluded).
- **Processing:** Inflation-adjusted gross revenue was converted to USD millions.

---

## Repository Contents
- The primary Python notebook containing all data cleaning, statistical analysis, and visualizations: `Disney_Box_Office_Analysis.ipynb`.
- The raw dataset used in the analysis: `disney_movies_total_gross.csv`.
- The final research paper report: `Disney Movies Statistical Analysis.pdf`.

---

## Statistical Methods
The project utilizes the following methodologies:
- **Data Preprocessing & EDA**
- **Assumption Testing:** Shapiro-Wilk (normality), Brown-Forsythe (homoscedasticity).
- **Omnibus Tests:** Welch's ANOVA, Kruskal-Wallis test.
- **Post-hoc Analysis:** Games-Howell comparisons.
- **Regression Modeling:** Robust OLS (log-transformed revenue).
- **Classification:** Logistic Regression (blockbuster prediction).

---

## Main Findings
- **Genre Significance:** Revenue differs significantly across Disney movie genres.
- **Genre Performance:** Adventure films consistently outperform lower-revenue genres.
- **Outlier Influence:** Musical films exhibit the highest mean revenue, driven by a few exceptionally successful titles.
- **Predictive Capability:** Genre is significantly associated with revenue but is not sufficient on its own to reliably predict blockbuster status.

---

## How to Reproduce the Analysis
1. Download or clone this repository.
2. Open the `Disney_Box_Office_Analysis.ipynb` notebook in [Google Colab](https://colab.research.google.com/).
3. When prompted, upload the `disney_movies_total_gross.csv` file.
4. Run all notebook cells sequentially to generate the tables and figures.

---

## Required Python Libraries
To run the analysis, ensure the following libraries are installed:
- `pandas`
- `numpy`
- `scipy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `scikit-learn`
- `pingouin`
