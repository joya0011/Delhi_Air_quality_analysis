# Data

`delhi_city_day_2015_2020.csv` — daily city-averaged air quality for **Delhi**, 1 Jan 2015 – 1 Jul 2020 (2,009 rows).

**Source:** Central Pollution Control Board (CPCB), Government of India, continuous ambient air quality monitoring data,
as compiled in the public dataset *Air Quality Data in India (2015–2020)* by Rohan Rao (Kaggle:
`rohanrao/air-quality-data-in-india`, file `city_day.csv`). This file is the Delhi subset of that `city_day.csv`, unmodified.

| Column | Unit | Notes |
|---|---|---|
| PM2.5, PM10 | µg/m³ | Particulate matter |
| NO, NO2, NOx | µg/m³ | NOx here is reported independently, ≈ NO + NO2 |
| NH3, SO2, O3 | µg/m³ | |
| CO | mg/m³ | |
| Benzene, Toluene, Xylene | µg/m³ | Xylene ~39% missing (dropped in analysis) |
| AQI, AQI_Bucket | – | CPCB Air Quality Index |

All cleaning (zero-as-missing, gap interpolation, PM2.5 > PM10 QA filter) is done inside the notebook; the raw file is never modified.
