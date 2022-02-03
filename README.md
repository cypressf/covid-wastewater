Scrape the [Massachusetts Water Resources Authority (MWRA) wastewater COVID-19 data](https://www.mwra.com/biobot/biobotdata.htm) from a PDF, save it as a csv file, and plot it vs the [New York Times reported covid case numbers](https://github.com/nytimes/covid-19-data).

# The Data

[Download the data as a csv](covid-19-wastewater.csv)

## Measured COVID-19 in Wastewater vs Reported Cases in Middlesex County, Massachusetts

![A line graph, showing covid prevalence for the northern region in RNA copies/mL 7 day average over time. The most recent month, Dec 2021, has a spike 10x higher than any previous record. There are smaller peaks in April 2020 and December 2020 to February 2021 but they are dwarfed by the recent spike. It also shows the reported cases, which follow the trend of the wastewater measurements, except the most recent spike is about 1/5 the height](visualization.svg "Covid prevalence in Middlesex County")

# Install and run

- Install [`poetry`](https://python-poetry.org)
- Install python dependencies via `poetry install`
- Run `jupyter notebook plot-covid-wastewater.ipynb`
