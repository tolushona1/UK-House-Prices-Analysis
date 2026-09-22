# UK House Prices vs Regional Employment
Analysis of UK regional house prices vs employment rates using Excel XLOOKUP

## Business Question:
Do regional employment rates relate to regional house prices across England? Specifically, do regions with stronger employment also tend to have higher house prices?

## Tools Used
- Excel (XLOOKUP, pivot tables)

## Approach
1. Combined two public datasets: HM Land Registry's UK House Price Index and ONS regional Labour Force Survey employment data.
2. Filtered both to England's 9 official regions and matched them by date and region, covering March 2015 to present (1,041 matched monthly records).
3. Merged the datasets in Excel using XLOOKUP, then summarised by region using a pivot table.

## Key Insight
Average house prices ranged from £133,538 (North East) to £341,802 (South East), tracking a similar spread in employment rates (75.2% to 81.5%). The two measures show a strong positive correlation of 0.79 — regions with higher employment rates are strongly associated with higher house prices. The relationship isn't perfectly linear, though: West Midlands and Yorkshire and The Humber have similar employment rates to the North West but noticeably different prices, suggesting other factors (housing supply, proximity to London, wages) are also at play.

## Limitations
This is a correlation, not a causal relationship as the analysis doesn’t prove employment rate causes higher house prices. Both are more likely driven by shared underlying regional economic strength. The correlation is also calculated across regions, and time combines so cross-regional differences (e.g: London/ South East demand pressure) likely account for much of the relationship more than employment changing within a single region over time.

## What I’d explore next:
- Test whether the relationship holds within individual regions over time, which would be a stronger signal of a genuine link rather than a regional-difference artefacts.
- Bring in additional variables (regional wages, housing supply/completions) to see which factors best explain price differences.
- Rebuild the same analysis in SQL and visualise it in Power BI to demonstrate the same finding using a different toolset.

## Links
- [Housing Prices vs Regional Influences Excel File.xlsx]
- (https://github.com/user-attachments/files/31435171/Housing.Prices.vs.Regional.Influences.Excel.File.xlsx)

<img width="375" height="296" alt="Excel Pivot Tables" src="https://github.com/user-attachments/assets/baeae746-195b-452b-a1e0-eb827d719c47" />
