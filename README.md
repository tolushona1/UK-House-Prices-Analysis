# UK-House-Prices-Analysis
Analysis of UK regional house prices vs employment rates using Excel XLOOKUP

Question:
Do regional employment rates relate to regional house prices across England? Specifically, do regions with stronger employment also tend to have higher house prices?

Data & Method:
I combined two public datasets: HM Land’s Registry’s UK House Price Index (average house price and 12-month price growth by region, monthly) and ONS regional Labour Force Survey data (employment rate, aged 16-64, by region). Both were filtered to England’s 9 official regions and matched by date and region, covering March 2015 to present (1, 041 matched monthly records). The two datasets were merged in Excel using XLOOKUP then summarised by region using a pivot table.

Findings:
Average house prices vary substantially by region, from £133, 538 in the North East to £341,802 in the South East. Employment rates show a similar regional spread, ranging from 75.2% (North East) to 81.5% (South East).
The two measures show a strong positive correlation of 0.79 across the full dataset where regions and periods with higher employment rates are strongly associated with higher prices. This holds at the regional level too: the two highest-price regions (South East, East of England) also have the two highest employment rates, while the lowest-price region (North East) has the lowest employment rate.
The relationship isn’t perfectly linear, however, West Midlands and Yorkshire and The Humber have similar employment rates to North West but noticeably different average prices, suggesting other factors (such as housing supply, proximity to London, wage levels) are also at play. Interestingly, average annual price growth doesn’t track the same pattern: West Midlands shows the highest average 12-month growth (5.1%) despite mid-range price and employment levels, indicating that growth rate and price level are driven by somewhat different dynamics.

Limitations:
This is a correlation, not a casual relationship as the analysis doesn’t prove employment rate causes higher house prices. Both are more likely driven by shared underlying regional economic strength. The correlation is also calculated across regions, and time combines so cross-regional differences (e.g: London/ South East demand pressure) likely account for much of the relationship more than employment changing within a single region over time.

What I’d explore next:
Test whether the relationship holds within individual regions over time (not just across regions), which would be a stronger signal of a genuine link rather than a regional-difference artefacts.
Bring in additional variables (regional wages, housing supply/completions) to see which factors explain price differences best.
Rebuild the same analysis in SQL and visualise it in Power BI to demonstrate the same finding using a different toolset.

[Housing Prices vs Regional Influences Excel File.xlsx](https://github.com/user-attachments/files/31435171/Housing.Prices.vs.Regional.Influences.Excel.File.xlsx)

<img width="375" height="296" alt="Excel Pivot Tables" src="https://github.com/user-attachments/assets/baeae746-195b-452b-a1e0-eb827d719c47" />
