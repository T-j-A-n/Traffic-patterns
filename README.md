# Urban Rush: Bengaluru Metro Traffic Patterns

## About the Project

As a team, we are studying Bengaluru Metro passenger patterns and
exploring how ridership relates to weather and air-quality conditions.
By combining these datasets, we aim to understand when passenger
activity is highest and identify patterns that may be useful for
understanding urban mobility.

This case study covers **1--18 August 2025**, with a focused
station-level analysis of **Bangalore City Station**.

## What We Analysed

-   Hourly metro passenger counts across stations.
-   Weekday and weekend ridership patterns.
-   Weather conditions, including temperature, humidity and rainfall.
-   Air-quality measurements, including PM10, NO₂ and SO₂.
-   Time-based comparisons between ridership and environmental data.

## Our Approach

We used Python and PySpark to load, clean and transform the datasets. We
reshaped hourly traffic records, aligned timestamps across the different
sources, explored trends and correlations, and created visualisations to
communicate the findings. We also prepared the processed data for
storage and querying using MySQL.

## Tools Used

-   **Python, Pandas and NumPy** -- data preparation and analysis.
-   **PySpark** -- traffic data processing.
-   **Matplotlib and Seaborn** -- data visualisation.
-   **SciPy** -- statistical analysis.
-   **MySQL** -- relational data storage.
-   **Jupyter Notebook** -- analysis workflow.

## Repository Contents

  File / Folder                               Description
  ------------------------------------------- --------------------------------------
  `notebook.ipynb`                            Main analysis notebook.
  `traffic.csv`                               Metro ridership data.
  `airQuality.csv`, `aqi.xlsx`                Air-quality data.
  `weather.json` and weather CSV/JSON files   Weather observations.
  Processed CSV files                         Cleaned and transformed datasets.
  `figures/`                                  Generated charts and visualisations.
  `requirements.txt`                          Python dependencies.
  `Urban_Rush_Report.docx`                    Case-study report.

## Running the Project

1.  Clone this repository:

    ``` bash
    git clone https://github.com/T-j-A-n/Traffic-patterns.git
    cd Traffic-patterns
    ```

2.  Install the required packages:

    ``` bash
    pip install -r requirements.txt
    ```

3.  Open `notebook.ipynb` in Jupyter Notebook and run the cells in
    order.

A compatible Java installation may be needed for PySpark. The MySQL
section also requires a running local MySQL server and locally
configured credentials. Do not upload database passwords or other
secrets to GitHub.

## Key Considerations

The traffic data covers 18 days, while the available air-quality data
covers a shorter period. Comparisons between these datasets therefore
use only overlapping timestamps. Weather observations are taken from a
location near the selected station, not from sensors at every metro
station.

Our analysis is observational: correlations can highlight patterns, but
they do not prove that one factor causes another.

## Conclusion

Through this case study, we bring together transport, weather and
air-quality data to explore Bengaluru's urban mobility patterns. The
project gives us practical experience in data cleaning, processing,
visualisation, statistical analysis and database integration.

------------------------------------------------------------------------

*Team case study for the Data and Storytelling course.*
