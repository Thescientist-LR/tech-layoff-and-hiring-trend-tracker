# Tech Layoff and Hiring Trend Tracker

**Tioluwani Olubowale · Python, pandas and Power BI**

Which tech sectors recorded the most job losses, and what happened to hiring demand around their layoff peaks?

Hardware led the tracker with **79,495 reported job losses** from June 2023 onward. The hiring picture varied by market. U.S. retail hires stayed above their pre-peak average from January through September 2026. In Germany, retail job postings rose above their pre-peak average in January 2025 and fell below it by June.

## Explore the project

The five-page Power BI report follows two questions. Where were job losses concentrated? How did hiring indicators change around selected layoff announcements?

| Report page | What to explore |
| --- | --- |
| Layoff Impact | Compare sectors by reported job losses and use the country filter to explore monthly peaks. |
| U.S. Hiring Recovery | Track retail, durable-goods, and information-sector hires around selected layoff peaks. |
| India Hiring Demand | Compare education and finance recruitment trends and read the evidence on food-delivery demand. |
| Germany Hiring Demand | Follow retail and manufacturing job postings around the selected layoffs. |
| Funding Stage | Compare reported losses across company stages. Post-IPO companies accounted for 338,249 reported job losses from June 2023 onward. |

## Reproduce the analysis

1. Open the Python notebook and load the raw layoffs CSV.
2. Run the cleaning and validation cells in order. The notebook documents exclusions, date corrections, and adjustments to reported job-loss counts.
3. Use the cleaned export to reproduce the sector, country, and funding-stage summaries.
4. Open the Power BI report to explore the results. To refresh it on another computer, update its data-source paths to the local CSV files.

## How to read the numbers

The analysis retained **4,641 of 4,648 source records**. Of those retained records, **3,024 had a usable job-loss count**. Sector rankings sum the reported losses in those records. A missing count means the number of jobs lost was unknown.

Country labels follow the layoff tracker’s classification of each announcement. A multinational announcement can cover workers in several countries.

Each hiring chart states its comparison period. On charts showing percentage change from a baseline, zero means the indicator matched its baseline average.

## Sources and scope

The notebook documents the layoff records and the sources for each hiring case. The U.S. cases use hires, the India cases use recruitment indicators and a delivery-worker demand report, and the Germany cases use job-posting indices.

These measures describe activity in the wider labor market around a layoff peak. Establishing when a particular employer resumed hiring or whether displaced workers found new jobs would require additional evidence.
