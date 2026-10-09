# ApexPlanet Internship — Task 4: Data Storytelling & Statistical Validation

This project combines business insights from the earlier data-cleaning, exploratory analysis, and dashboard tasks into a concise stakeholder presentation and validates one business question using statistical hypothesis testing.

## Deliverables

- **PowerPoint presentation:** `ApexPlanet_Task4_Final_Presentation.pptx`
- **Hypothesis testing workbook:** `ApexPlanet_Task4_Hypothesis_Testing_Summary.xlsx`
- **Written hypothesis report:** `Task4_Hypothesis_Testing_Summary.md`

## Business story and key findings

The cleaned dataset contains 1,000 orders and 947 unique customers.

- **Total sales:** ₹139,399,439.65 (about ₹13.94 crore)
- **Average order value:** ₹139,399.44
- **Units sold:** 5,435
- **Top revenue category:** Electronics — ₹50,778,581.70
- **Top product by revenue:** Laptop — ₹25,443,008.51
- **Top city by revenue:** Patna — ₹19,285,966.89
- **Top month by revenue:** March 2025 — ₹13,059,899.94

Customer groups are presented as an **RFM-lite segmentation** (Champions, Loyal, Potential, Needs Attention, At Risk). The dataset has 947 customers across 1,000 orders, so the segments should be treated as directional indicators rather than a validated long-term churn model.

## Hypothesis test

**Business question:** Is the average order sales amount for Electronics statistically different from the average for non-Electronics orders?

- **H₀:** The mean order sales amount is equal for Electronics and non-Electronics.
- **H₁:** The mean order sales amount differs between the two groups.
- **Test:** Welch's independent two-sample t-test
- **Significance level:** α = 0.05
- **p-value:** 0.413674
- **95% confidence interval for the mean difference (Electronics − non-Electronics):** −₹8,764.16 to ₹21,280.82
- **Decision:** Fail to reject H₀. The observed difference in average order value is not statistically significant at the 5% level.

Electronics has the highest total category revenue, but this does **not** establish that its average order value is higher. Total revenue can also reflect order counts and the mix of products sold.

## Methodology and limitations

The analysis uses the cleaned dataset prepared for Task 1 and the findings developed in Tasks 2–3. Welch's t-test does not assume equal variances. The confidence interval includes zero, consistent with the non-significant p-value. Results describe this dataset and should not be interpreted as causal evidence or a forecast.

## Files

See the PowerPoint for the visual business narrative and the Excel workbook/Markdown report for the statistical test details.

## Author

Deepanshu Bhirmaan · Data Analytics Internship Project
