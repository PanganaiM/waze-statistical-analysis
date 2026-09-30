# Waze User Behaviour — Statistical Analysis and Hypothesis Testing

## Project Overview
This project uses statistical hypothesis testing to determine whether average driving activity differs between Waze users on iPhone and Android devices.

## Business Question
Is there a statistically significant difference in the mean number of drives between iPhone and Android Waze users?

## Hypotheses
**Null hypothesis (H₀):** There is no difference in the mean number of drives between iPhone and Android users.

**Alternative hypothesis (H₁):** There is a difference in the mean number of drives between iPhone and Android users.

The analysis uses a 5% significance level.

## Tools and Technologies
- Python
- pandas
- SciPy
- Jupyter Notebook

## Analytical Workflow
1. Load and inspect the Waze dataset.
2. Review the relevant device and driving variables.
3. Separate users into iPhone and Android groups.
4. Calculate descriptive statistics for each group.
5. Perform Welch's two-sample t-test.
6. Compare the p-value with the 0.05 significance level.
7. Interpret the result in a business context.

## Selected Output
The dataset contains **14,999 users**:
- iPhone users: **9,672**
- Android users: **5,327**

Average number of drives:
- iPhone: approximately **67.86**
- Android: approximately **66.23**

Difference in group means: approximately **1.63 drives**.

Welch's two-sample t-test:
- **t-statistic:** approximately 1.464
- **p-value:** approximately 0.1434

## Statistical Conclusion
Because the p-value is greater than 0.05, the null hypothesis is not rejected. The sample does not provide sufficient evidence of a statistically significant difference in mean driving activity between iPhone and Android users.

## Business Interpretation
Although iPhone users recorded a slightly higher mean number of drives in the sample, the observed difference is not statistically significant at the 5% level. Device type alone therefore does not provide strong evidence for different average driving behaviour in this analysis.

## Business Recommendation
Device type can remain available for future analysis, but stronger behavioural predictors should receive greater attention when investigating engagement and churn.

## Repository Contents
- `waze_statistical_analysis.ipynb` — hypothesis-testing notebook
- `waze_dataset.csv` — project dataset
- `README.md` — project documentation

## How to Run
1. Clone or download the repository.
2. Install the required Python libraries.
3. Open `waze_statistical_analysis.ipynb` in Jupyter.
4. Run the notebook from top to bottom.

## Skills Demonstrated
- Statistical hypothesis testing
- Descriptive statistics
- Welch's two-sample t-test
- p-value interpretation
- Python data analysis
- Translation of statistical results into business insights
