# econ3916-lab02-deflation
Deflating Economic Data — Nominal vs. Real
Objective

I used CPI data from FRED to convert nominal prices and wages into constant dollars so I could see how much purchasing power actually changed over time.

Methodology
Pulled the Consumer Price Index (CPI) and average hourly earnings from FRED without an API key.
Used deflate_series() to convert nominal hourly earnings into constant 2020 dollars.
Deflated the US Big Mac price the same way, lining up each Big Mac observation with the CPI value in effect on that date.
Compared nominal growth, real growth, and CPI growth over the same dates to check how they relate.
Built an interactive deflation explorer with a base-year slider to show how changing the base year shifts the level of the real series without changing its growth rate.
Key Findings
Nominal hourly earnings rose from $20 to $30, while real earnings only moved from $35 to $15. Most of the nominal increase just kept pace with inflation.
The US Big Mac price rose 8% in nominal terms but only 4% in real terms, with CPI up 2% over the same dates.
Nominal growth minus real growth does not equal CPI growth, because growth rates compound: (1 + nominal) = (1 + real) × (1 + inflation).
Moving the base year in the explorer changes the dollar level of the real series but leaves its percentage change the same.
