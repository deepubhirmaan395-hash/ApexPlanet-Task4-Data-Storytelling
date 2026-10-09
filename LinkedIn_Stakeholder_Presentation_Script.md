# Task 4 Stakeholder Presentation — Video Script (7–10 minutes)

**Delivery tip:** Speak slowly, use the slides as prompts, and pause briefly between sections. This script is designed for a 7–10 minute recording.

## 1. Introduction (0:00–0:45)
Hello everyone. My name is Deepanshu Bhirmaan, and this is my Task 4 presentation for the ApexPlanet Data Analytics Internship. In this project, I bring together data cleaning, exploratory analysis, dashboard insights, and statistical validation to tell a clear business story. My goal is not only to report numbers, but also to explain what they mean for business decisions.

## 2. Dataset and approach (0:45–1:40)
I started with the cleaned sales dataset prepared in Task 1 and used the analysis and dashboard work from Tasks 2 and 3. The dataset contains 1,000 orders and 947 unique customers. The workflow included checking the data, summarizing key performance indicators, comparing sales across categories, products, cities, and months, and building an RFM-lite view of customer segments. Finally, I selected a business question and tested it statistically rather than relying only on visual differences.

## 3. Overall performance (1:40–2:35)
The dataset records total sales of approximately 139.4 million rupees, or about 13.94 crore. There are 1,000 orders and 5,435 units sold. The average order sales amount is about 139,399 rupees. These indicators provide a high-level view of the sales represented in this dataset. They should be interpreted in the context of the dataset and its time period, rather than as a forecast of future sales.

## 4. What is driving sales? (2:35–3:45)
Electronics is the highest-revenue category, generating about 50.78 million rupees. Laptop is the top product by revenue, at approximately 25.44 million rupees. Patna is the top city by revenue, contributing about 19.29 million rupees. March 2025 is the strongest month in the dataset, with sales of approximately 13.06 million rupees. These patterns can help a business decide where to investigate inventory availability, local demand, and campaign timing. However, high revenue alone does not prove high profitability, because costs and margins are not included in these figures.

## 5. Customer segmentation (3:45–4:45)
I also used an RFM-lite approach to organize customers into groups such as Champions, Loyal, Potential, Needs Attention, and At Risk. This type of segmentation can help teams think about different engagement strategies. For example, high-value customers may respond to loyalty benefits, while customers who appear less engaged may need a relevant reminder or offer. One important limitation is that there are 947 unique customers for 1,000 orders, so there is limited repeat-order history. These groups should therefore be treated as directional indicators, not as a proven churn prediction model.

## 6. Business hypothesis (4:45–5:35)
The statistical question was: is the average order sales amount for Electronics significantly different from the average for non-Electronics orders? The null hypothesis says the two means are equal. The alternative hypothesis says they differ. I used Welch's independent two-sample t-test, which is suitable for comparing two independent group means without assuming equal variances. I set the significance level at five percent before interpreting the result.

## 7. Statistical result (5:35–6:45)
The test produced a p-value of 0.413674. This is greater than 0.05, so I fail to reject the null hypothesis. The 95 percent confidence interval for the mean difference, Electronics minus non-Electronics, ranges from negative 8,764 rupees to positive 21,281 rupees. Because this interval includes zero, it is consistent with the test result: the data do not provide sufficient evidence of a statistically significant difference in average order sales amount between these groups. This does not prove that the means are exactly equal; it means the observed data do not establish a difference at the selected significance level.

## 8. What the result means for business (6:45–7:45)
An important takeaway is that the category with the highest total revenue does not necessarily have a statistically higher average order value. Total revenue is influenced by order count as well as order size. A sensible next step would be to compare order volume, gross margin, discounting, and customer-level repeat behavior. If more historical data becomes available, the business could validate customer segments over time and evaluate whether campaigns improve outcomes.

## 9. Recommendations and close (7:45–8:45)
Based on this analysis, I recommend monitoring Electronics and Laptop sales closely, investigating the drivers behind Patna's revenue, and reviewing seasonality around March. I would also recommend combining revenue metrics with margin and order-volume metrics before making resource-allocation decisions. Customer engagement experiments should be measured against a clear baseline. To conclude, this project demonstrates a complete analytics workflow: preparing data, finding patterns, communicating them through a dashboard and presentation, and using statistical testing to check whether a difference is supported by evidence. Thank you for watching.

## Recording checklist
- Keep the slide deck visible and share your screen.
- Record in a quiet place with clear audio.
- Aim for 7–10 minutes; do not rush the statistical explanation.
- Upload the video to LinkedIn and include the public GitHub repository link in the post.
