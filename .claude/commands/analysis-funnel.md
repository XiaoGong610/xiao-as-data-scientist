Analyze a funnel dataset to understand conversion progression and identify drop-off points.

Steps:

1. **Identify funnel stages**
   - Determine all unique events/stages and their logical order
   - Confirm granularity (one row per subject per event, or wide format)

2. **Overall funnel conversion**
   - Count subjects at each stage
   - Calculate conversion rate relative to the top of funnel
   - Calculate stage-to-stage conversion rates (drop-off between consecutive steps)

3. **Funnel visualization**
   - Create a funnel chart showing counts and conversion rates at each stage
   - Highlight the biggest drop-off points

4. **Segmentation**
   - Break down funnel by key dimensions (channel, city, cohort, etc.)
   - Identify which segments have the highest/lowest conversion
   - Flag segments with unusual drop-off patterns

5. **Side-by-side comparison (if applicable)**
   - Compare funnels across groups (e.g., control vs treatment, old vs new flow)
   - Visualize as side-by-side funnel charts
   - Quantify lift/drop at each stage

6. **Key findings**
   - Where are the biggest drop-offs?
   - Which segments perform best/worst?
   - What stages are candidates for improvement?

Use pandas and seaborn/matplotlib. Generate funnel visualizations as images for embedding in slides.
