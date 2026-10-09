# Hypothesis Testing Summary — Task 4

## Business question
Is the mean order sales amount (`Total_Sales`) for Electronics orders different from that of non-Electronics orders?

## Hypotheses
- **Null hypothesis (H₀):** The population mean order sales amount is equal for Electronics and non-Electronics.
- **Alternative hypothesis (H₁):** The population mean order sales amount differs between Electronics and non-Electronics.

## Test design
- **Variable:** `Total_Sales`
- **Groups:** Electronics vs. all other categories
- **Statistical test:** Welch's independent two-sample t-test (two-sided)
- **Significance level:** α = 0.05
- **Confidence level:** 95%

## Results
- **p-value:** 0.413674
- **95% confidence interval for mean difference (Electronics − non-Electronics):** −₹8,764.16 to ₹21,280.82
- **Decision:** Fail to reject H₀ because p > 0.05.
- **Interpretation:** The data do not provide sufficient statistical evidence at the 5% significance level that the average order sales amount differs between Electronics and non-Electronics orders.

## Business interpretation
Electronics generated the highest total category revenue (₹50,778,581.70), but the hypothesis test does not find a statistically significant difference in mean order sales amount. These are different metrics: total revenue is affected by both the number of orders and the value of orders. Business decisions should examine revenue, order volume, margin, and customer behavior together.

## Data and limitations
The cleaned dataset contains 1,000 orders and 947 unique customers. Customer segmentation is RFM-lite and should be interpreted directionally because repeat-order history is limited. This analysis is observational and does not establish causality. The confidence interval includes zero, which agrees with the non-significant p-value.

## Reproducibility
The Excel workbook `ApexPlanet_Task4_Hypothesis_Testing_Summary.xlsx` contains the hypothesis test summary and results. The PowerPoint `ApexPlanet_Task4_Final_Presentation.pptx` presents the business story and stakeholder conclusions.
