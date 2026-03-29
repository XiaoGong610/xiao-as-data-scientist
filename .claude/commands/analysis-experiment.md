Analyze an A/B experiment dataset and deliver actionable conclusions.

Steps:

1. **Understand the experiment context**
   - What is being tested (treatment vs control)?
   - What is the hypothesis?
   - Define the key driver metric (e.g., overall conversion rate = # converted / # total)

2. **Data preparation**
   - Pivot to one row per subject with columns for each funnel stage or event
   - Join group assignment and any segmentation dimensions (channel, city, etc.)

3. **Overall results**
   - Compare key driver metric: control vs treatment
   - Compare conversion rates at each funnel stage

4. **Randomization balance check**
   - Cross-tab group × each segmentation dimension
   - Flag any imbalances that could indicate selection bias

5. **Statistical significance testing**
   - Two-proportion z-test at each funnel stage
   - Report: control rate, treatment rate, lift (pp), z-stat, p-value, significance level

6. **Segmentation analysis**
   - Break down treatment effect by each dimension (channel, city, etc.)
   - Check if the effect is consistent or concentrated in specific segments

7. **Conclusions & recommendations**
   - State whether the treatment works (effect size + significance)
   - Frame as a decision: ship, iterate, or investigate further
   - Flag limitations and what the data can't tell us

Write each major section in a separate notebook. Use pandas, scipy.stats, seaborn.
