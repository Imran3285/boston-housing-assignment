# 🏠 Boston Housing — Statistical Analysis with Python

A data-driven statistical analysis of Boston housing prices using hypothesis testing, correlation analysis, and regression modelling.

---

## 🎯 Business Problem

As a Data Scientist working for a housing agency in Boston, MA, management requires actionable insights from U.S. Census housing data to support informed decision-making.

Specifically, they need to understand:

- Whether proximity to the Charles River significantly affects home values
- How the age of housing stock influences median prices
- The relationship between industrial activity and air pollution (NOX)
- How distance from employment centres impacts property values

---

## 📊 Dataset

**506 Boston neighbourhoods** with 14 features including:

| Feature | Description |
|---|---|
| MEDV | Median value of owner-occupied homes ($1000s) |
| CHAS | Charles River boundary (1 = Yes, 0 = No) |
| AGE | % of owner-occupied units built before 1940 |
| NOX | Nitric oxide concentration (parts per 10M) |
| INDUS | Proportion of non-retail business acres per town |
| DIS | Weighted distance to 5 Boston employment centres |

---

## 🔍 Key Findings

### 1. Charles River — Home Value Premium
River-bounded homes average **$28.44K** vs **$22.09K** for non-river homes.
A Welch's T-test confirmed this difference is **statistically significant (p < 0.05)**.

### 2. Housing Age vs Median Value
Newer neighbourhoods (≤35% pre-1940 units) command significantly higher prices.
One-Way **ANOVA confirmed significant differences** across all three age groups (p < 0.05).

### 3. Industrial Activity & Air Pollution
**Strong positive Pearson correlation (r ≈ 0.76)** between INDUS and NOX.
Towns with more industrial land consistently show higher nitric oxide levels.

### 4. Distance to Employment Centres
**Linear regression slope = 1.09** — for every unit increase in DIS, MEDV increases by ~$1,090.
Homes further from industrial employment centres command a measurable price premium.

---

## 📈 Visualisations

| Chart | Insight |
|---|---|
| Bar Plot (CHAS) | River-bounded homes worth ~29% more on average |
| Boxplot (MEDV) | Right-skewed distribution, median ~$21K, several high-value outliers |
| Boxplot (MEDV vs Age Group) | Clear decline in values from New → Middle → Old housing |
| Histogram (AGE) | Boston housing stock is predominantly old (mean 68.6%, median 77.5%) |
| Scatter Plot (NOX vs INDUS) | Strong positive trend — industrial zones drive pollution |
| Scatter Plot (DIS vs MEDV) | Positive slope — suburban distance adds home value |

---

## 🧪 Statistical Tests Used

- **Levene's Test** — checked equality of variances before T-test
- **Welch's T-test** — compared MEDV between CHAS groups
- **One-Way ANOVA** — compared MEDV across three housing age groups
- **Pearson Correlation** — measured NOX vs INDUS linear relationship
- **Linear Regression** — quantified DIS impact on MEDV

---

## 💡 Recommendations to Management

- **Prioritise river-adjacent developments** — they command a consistent price premium
- **Invest in newer housing stock** — age of units is a strong predictor of value
- **Address pollution in high-INDUS zones** — industrial land directly raises NOX levels
- **Recognise suburban premium** — distance from employment hubs positively impacts prices

---

## 🚀 How to Run

```bash
git clone https://github.com/Imran3285/boston-housing-assignment.git
cd boston-housing-assignment
pip install pandas numpy matplotlib seaborn scipy jupyter
jupyter notebook
```

Run all cells in `-Optional--Peer-Graded-Assignment-jupyterlite-v2.ipynb`

---

## 🛠 Stack

Python · Pandas · NumPy · Matplotlib · Seaborn · SciPy · Jupyter

---

## 👤 Author

**Muhammad Imran**
