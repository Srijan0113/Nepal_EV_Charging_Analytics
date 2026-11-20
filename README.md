# Nepal EV Charging Stations — Data Audit

## What was the plan?
Analyze the status and coverage of EV charging stations in Nepal.

## What did I do?
I collected and cleaned 350 EV charging station records for Nepal.

## What did I find?

**1. No one has a complete list.**
Different sources give different numbers:
- nepalevs.com: 352+ stations
- NEA (government): 62 fast chargers
- Ministry report: ~1,000 stations
- Media (citing NEA): 2,300+ stations

Each source counts different things. There is no official national registry.

**2. The data is incomplete.**
- 57% of rows have no power specifications.
- 60% of rows have no coordinates.
- Only about 150 rows (43%) have enough data to analyze.

**3. The data has errors.**
- About 10 duplicate listings were found.
- Several coordinates are wrong (for example, two different districts share the same coordinates).
- **Older data had mismatched locations and was incomplete**, making it unreliable.

**4. Private companies run most stations.**
Vehicle dealers and hotels own most charging stations. They do not publish station-level details.

## Why I stopped the original analysis
Only ~150 rows have enough data for real analysis. That is not enough to represent the whole country. Guessing the missing values would make the results unreliable. Scraping more data would take a lot of time, which was not possible in this timeline.

## What this means
Nepal's EV charging data is fragmented and incomplete. A real analysis needs:
1. An official government database, or
2. Data-sharing from private operators, or
3. A longer scraping and field-verification project.

