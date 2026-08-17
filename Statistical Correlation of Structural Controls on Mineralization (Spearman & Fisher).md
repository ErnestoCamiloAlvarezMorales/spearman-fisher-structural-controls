# Statistical Correlation of Structural Controls on Mineralization (Spearman & Fisher)

Python workflow to mathematically validate the spatial and lithological dependence of ore grades using non-parametric statistical tests.

---

## The Problem
In economic geology, proving that a mineralization is structurally or lithologically controlled is often based on subjective field observations. How can we mathematically prove that copper grades increase near a fault plane, or that mineralization is strictly dependent on the host rock?

---

## The Solution
This script integrates structural coordinates (distance to fault) and geochemical data (Cu %) to run two robust statistical tests:

1. **Spearman's Rank Correlation:** Evaluates if there is a statistically significant correlation between the distance to the fault plane and the copper grade (accounting for non-normal, log-normal geological distributions).
2. **Fisher's Exact Test:** Determines if the presence of mineralization is independent of the host rock lithology (e.g., Sandstone vs. Volcanic rock).

---

## Tech Stack
* **Python**
* **Pandas** (Data manipulation)
* **SciPy** (Statistical tests: Spearman & Fisher)
* **Seaborn / Matplotlib** (Statistical visualization)

---

## Key Outputs
The script generates:
* A scatter plot with a regression line displaying the Spearman Rho ($\rho$) and $p$-value.
* A count plot visualizing the categorical distribution of mineralized vs. barren samples by lithology, including the Fisher $p$-value.

![Prueba de Fisher](fisher_plot.png)
![Correlación Spearman](spearman_plot.png)

---

## How to Use

1. Clone the repository.
2. Install dependencies: pip install pandas scipy seaborn matplotlib
3. Run the Jupyter Notebook.
4. Input your integrated dataset (CSV with Distance to fault, Cu %, and Lithology) to validate your own exploration targets.

---

## Author

**Ernesto Álvarez** — Geology Student | Self-Taught Data Science Practitioner

Applying data science and statistical methods to economic geology and mineral exploration.
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ernesto-alvarez-1400ba190/)


