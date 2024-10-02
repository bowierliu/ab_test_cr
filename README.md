# A/B Testing Analysis on Landing Page Conversion Rates

## Project Overview
This project performs an A/B test analysis to determine whether a new landing page improves conversion rates compared to the old landing page. The dataset includes user interaction data with conversion outcomes (0 or 1) and group assignments (control or treatment). The project applies statistical methods like the Z-test and Chi-Square test to assess whether the difference in conversion rates between the control and treatment groups is statistically significant.

## Dataset
The dataset includes the following key variables:
- **user_id**: Unique identifier for each user.
- **timestamp**: Time when the user accessed the page.
- **group**: Indicates whether the user was part of the control group (old page) or treatment group (new page).
- **landing_page**: Indicates whether the user saw the old or new landing page.
- **converted**: Binary variable indicating whether the user converted (1 for converted, 0 for not converted).

## Analysis Process
1. **Data Cleaning**: Removed mismatched entries between groups and landing pages (e.g., control group seeing the new page).
2. **Exploratory Data Analysis (EDA)**: Calculated and visualized conversion rates for the control and treatment groups.
3. **A/B Test Analysis - Z-test**: Performed a Z-test to check if the difference in conversion rates between the two groups was statistically significant.
4. **A/B Test Analysis - Chi-Square Test**: Performed a Chi-Square test to validate the results of the Z-test.

## Results
Both the Z-test and Chi-Square test showed no statistically significant difference in conversion rates between the control and treatment groups. The p-values from both tests were 0.19, which is greater than the significance level of 0.05. As a result, we fail to reject the null hypothesis, indicating that the new landing page did not significantly improve conversion rates compared to the old page.

## Conclusion
The analysis suggests that the new landing page does not have a statistically significant impact on improving conversion rates. Further testing or modifications to the landing page may be needed to achieve meaningful improvements in conversion.

## Technologies Used
- **Python**: Data analysis and statistical testing
- **Pandas**: Data manipulation and preprocessing
- **Matplotlib/Seaborn**: Data visualization
- **SciPy**: Hypothesis testing
