# Crime Analysis and Prediction Dashboard (Tableau)

MCA team project, Tableau course, Centurion University of Technology and Management.

An interactive Tableau workbook that analyses reported crimes in Indian cities: where and when crimes happen,
which crimes are most common, who the victims are, how quickly cases are closed, and how many cases to expect next.

## How to open

Open **`Crime_Analysis_and_Prediction_Dashboard.twbx`** in Tableau Desktop or the free Tableau Reader.
The data is packaged inside the file, so nothing else is needed.

## Dashboards

| Dashboard | What it shows |
|---|---|
| **Analysis Dashboard** | Total cases, crimes over time, top crime types, victim age and gender |
| **Prediction Dashboard** | Crime forecast for the coming months and the risk of cases staying unsolved |
| **City & Case Resolution** | Crimes by city on a map, case closure rate per city, days taken to close a case |

## Worksheets

City Map · Crime Forecast · Crime Over Time · Top Crimes · Total Cases · Unsolved Case Risk ·
Victim Demographics · Crimes by City · Closure Rate by City · Days to Close

## Data

`crime_dataset_india.csv`: 40,160 reported crimes in 29 Indian cities, 2020 to 2023.

Columns: Report Number, Date Reported, Date of Occurrence, Time of Occurrence, City, Crime Code,
Crime Description, Victim Age, Victim Gender, Weapon Used, Crime Domain, Police Deployed, Case Closed, Date Case Closed.

## Methods

- **Trend analysis:** monthly crime counts over time.
- **Forecast:** Tableau's built-in forecast (exponential smoothing with automatic seasonality), one year ahead, with a 95% prediction band.
- **Case resolution:** closure rate (share of cases closed) and days between report and closure, per city.
- **Calculated field:** `Case Status Check` marks each case as closed or open.

## Limitations

- The forecast continues past patterns; it cannot predict sudden changes.
- Results depend on how complete and accurate the reported data is.
