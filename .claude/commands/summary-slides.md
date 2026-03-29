Create a PowerPoint (.pptx) presentation summarizing the analysis findings.

Use the `python-pptx` library. Save the output to the project's `output/` folder.

## Workflow

1. **Collect requirements** — ask the user:
   - What findings/notebooks to include?
   - Any branding (logo, colors)? Check `reference/` folder for images.
   - Audience: technical or executive?

2. **Confirm outline** — present the proposed slide list and get approval before generating.

3. **Generate slides** — create the .pptx following the structure below.

4. **Convert to PDF** — use LibreOffice (`soffice --headless --convert-to pdf`) and save alongside the .pptx.

## Slide Structure

1. **Title slide** — project name, date, author. Use brand logo if available.
2. **Executive summary** — 3-5 bullet points of key findings and recommended actions
3. **Data overview** — dataset description, scope, date range, key metrics
4. **Analysis slides** — one slide per major finding, each with:
   - A chart (embed from output/ folder if available, otherwise regenerate and save)
   - 2-3 bullet points explaining the insight and its business implication
5. **Recommendations** — actionable next steps based on the analysis
6. **Appendix** — methodology notes, data limitations, caveats

## Design Guidelines

- Check `reference/` folder for brand images and derive color scheme from them
- Keep text concise — bullets, not paragraphs
- Every chart needs a clear title and takeaway
- Max 4-5 bullet points per slide
- Frame findings as decisions, not just observations
- Flag limitations and what the data can't tell us
- Use consistent fonts, colors, and spacing throughout
