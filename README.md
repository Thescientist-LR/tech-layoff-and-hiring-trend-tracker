# Tech Layoff and Hiring Trend Tracker

**Tioluwani Olubowale · Python, pandas and Power BI**

Which tech sectors recorded the most job losses, and how did hiring change around their layoff peaks? Hardware led the tracker with **79,495 reported job losses** from June 1, 2023 through October 29, 2026. In the United States, durable-goods hiring returned above its pre-peak average 14 months after the April 2025 Hardware layoff peak. Retail hiring was already above its own baseline during its January 2026 peak.

| Case | What stood out |
|---|---|
| United States · Retail | Amazon accounted for all 16,000 losses in the U.S.-tagged January 2026 Retail peak. U.S. retail hires stayed above the October–December 2025 average from January through September 2026. |
| India · Education | The education recruitment index was 9.6% below its July–September average in October 2022, the month of the layoff peak. |
| Germany · Retail | Retail job postings rose above their pre-peak average in January 2025 and fell below it by June. |
| Company funding stage | Companies that had already gone public accounted for 338,249 reported job losses during the June 2023–October 2026 comparison period, the largest total of any funding-stage group. |

## Explore the project

- [Five-page report preview](Tech%20Layoff%20and%20Hiring%20Trend%20Tracker.pdf) — view all five pages in a PDF.
- [Interactive Power BI report](Tech%20Layoff%20and%20Hiring%20Trend%20Tracker.pbix) — select a country on **Layoff Impact** to explore sector rankings and monthly peaks. The country pages show hiring trends, and **Funding Stage** compares losses by company stage.
- [Analysis notebook](Tech_Layoff_and_Hiring_Trend_Tracker.ipynb) — inspect the cleaning decisions, sector rankings, case studies and source notes.
- [Cleaned layoff data](layoffs_dashboard_verified.csv) — one row per retained record, with the analysis date, reported losses, industry, country tag and funding stage.

## Reproduce the analysis

1. Open the notebook in Google Colab and supply the [raw layoff CSV](layoffs.csv) for the input-loading cell.
2. Run the cleaning cells in order before running the sector, country and funding-stage comparisons. The notebook records the reasons for exclusions and adjustments to dates and counts.
3. Follow each country section's source and baseline instructions to reproduce its hiring comparison. The historical series begins in March 2020, so some country cases precede the overall ranking period.
4. Download the Power BI file and open it in Power BI Desktop. To refresh the report on another computer, point its data sources to the local cleaned layoff CSV and country hiring files.

## How to read the numbers

Of 4,648 source records, the analysis retained 4,641. Only 3,024 retained records had a usable job-loss count. The rankings sum reported losses. A missing count means the number of jobs lost was unknown.

Country tags describe how the tracker classifies an announcement. A multinational announcement can cover workers in several countries. On charts showing percentage change from a baseline, zero means the indicator matched the reference average named on that chart.

## Sources and scope

The notebook documents the layoff announcements and links the hiring sources for each case. The U.S. comparisons use sector hires, India uses recruitment indices and a published delivery-worker demand checkpoint, and Germany uses new job-posting indices.

These indicators describe the surrounding labor market. Measuring how quickly individual companies rehired workers would require employer-level hiring records. The funding-stage comparison groups announcements by the company status recorded in the tracker. Testing whether layoffs followed a funding round would also require funding-round dates.
