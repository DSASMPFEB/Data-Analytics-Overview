## 📊 Core Concepts & Statistics
### Descriptive vs Inferential Statistics:
- Descriptive: Summarizes data (mean, median, mode, etc.)
- Inferential: Makes predictions or generalizations using sample data (hypothesis testing, confidence intervals)
- Correlation vs Causation:
- Correlation: Two variables move together
- Causation: One variable directly affects the other
- Example: Ice cream sales and drowning incidents may correlate, but don’t cause each other.
- P-value:
Measures the probability of observing results as extreme as the ones in your sample, assuming the null hypothesis is true.
- Low p-value (< 0.05) → reject null hypothesis
- High p-value → fail to reject null
- Handling Missing Data:
- Remove rows/columns
- Impute with mean/median/mode
- Use algorithms that handle missing values (e.g., XGBoost)
- Central Limit Theorem (CLT):
The sampling distribution of the sample mean approaches a normal distribution as sample size increases, regardless of the population’s distribution.

## 🧮 Data Wrangling & SQL
### Types of Joins:
- INNER JOIN: matching rows
- LEFT JOIN: all from left + matches from right
- RIGHT JOIN: all from right + matches from left
- FULL JOIN: all rows from both sides
### Finding Duplicates:
SELECT column, COUNT(*)  
FROM table  
GROUP BY column  
HAVING COUNT(*) > 1;
- 
- GROUP BY vs PARTITION BY:
- GROUP BY: aggregates data across groups
- PARTITION BY: used with window functions to segment data without collapsing rows
- Optimizing SQL Queries:
- Use indexes
- Avoid SELECT *
- Use EXPLAIN to analyze query plans
- Limit subqueries and nested joins
- Normalization:

- Organizing data to reduce redundancy and improve integrity.
- 1NF: atomic values
- 2NF: remove partial dependencies
- 3NF: remove transitive dependencies

## 📈 Visualization & Reporting
- Good Dashboard Traits:
- Clear KPIs
- Minimal clutter
- Interactive filters
- Responsive layout
- Choosing Charts:
- Bar chart: categorical comparison
- Line chart: trends over time
- Pie chart: proportions (use sparingly)
- Scatter plot: correlation
- Tableau vs Power BI:
- Tableau: advanced visuals, better for data exploration
- Power BI: tight integration with Microsoft tools, cost-effective
- Handling Outliers:
- Highlight them
- Use box plots
- Consider log transformation or exclusion (with justification)
- Presenting Insights:
- Know your audience
- Use storytelling
- Focus on actionable insights
- Avoid jargon
## 🤖 Tools & Technologies
- Excel vs SQL:
- Excel: quick analysis, small datasets
- SQL: scalable, structured queries for large datasets
- Python vs R:
- Python: general-purpose, ML-friendly
- R: statistical analysis, visualization-heavy
- Common Python Libraries:
- Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- ETL (Extract, Transform, Load):
- Extract data from sources
- Transform it (clean, format)
- Load into a data warehouse or database
- Pivot Tables in Excel:
Summarize data dynamically by rows, columns, and values. Great for quick aggregations.
## 📦 Business & Scenario-Based
- Measuring Marketing Campaign Success:
- ROI
- Conversion rate
- Customer acquisition cost
- Engagement metrics
- Prioritizing KPIs:
- Align with business goals
- Use SMART criteria
- Focus on actionable metrics
- Influencing Decisions:
Example: “My analysis showed that churn was highest among users with low engagement. We launched a re-engagement campaign and reduced churn by 15%.”
- Conflicting Stakeholders:
- Clarify goals
- Prioritize based on impact
- Communicate trade-offs
- Use data to mediate
- Customer Retention Metrics:
- Churn rate
- Repeat purchase rate
- Net Promoter Score (NPS)
- Customer Lifetime Value (CLV)

## 🧪 Modeling & Predictive Analytics
- Linear Regression:
Predicts a continuous outcome based on one or more predictors.
Equation: y = \beta_0 + \beta_1x + \epsilon
- Evaluating Models:
- Classification: Accuracy, Precision, Recall, F1-score
- Regression: RMSE, MAE, R²
- Overfitting:
Model performs well on training data but poorly on new data.
- Prevention: cross-validation, regularization, pruning
- Classification vs Regression:
- Classification: categorical output (e.g., spam or not)
- Regression: continuous output (e.g., price prediction)
- Feature Selection:
- Correlation analysis
- Recursive Feature Elimination (RFE)
- Domain knowledge
- Regularization (Lasso)
