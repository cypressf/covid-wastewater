Scrape the [Massachusetts Water Resources Authority (MWRA) wastewater COVID-19 data](https://www.mwra.com/biobot/biobotdata.htm) from a PDF, save it as a csv file, and plot it vs the [New York Times reported covid case numbers](https://github.com/nytimes/covid-19-data).

# The Data

[Download the data as a csv](covid-19-wastewater.csv)

## Measured COVID-19 in Wastewater vs Reported Cases in Middlesex County, Massachusetts

![A line graph, showing covid prevalence for the northern region in RNA copies/mL 7 day average over time. The most recent month, Dec 2021, has a spike 10x higher than any previous record. There are smaller peaks in April 2020 and December 2020 to February 2021 but they are dwarfed by the recent spike. It also shows the reported cases, which follow the trend of the wastewater measurements, except the most recent spike is about 1/5 the height](visualization.svg "Covid prevalence in Middlesex County")

The wastewater measurements are higher than the reported cases in the most recent month. I made this chart to highlight this, and inspire people to ask why. Some possibilities:

- The confidence interval of wastewater measurements is larger the higher the valeus are. It could be that the values aren't as high as reported, if they fall in the lower half of the confidence interval.
- There aren't enough tests to keep up with case numbers
- More people are testing at home and not reporting positives
- People are asymptomatic, so they're not testing
- Testing lags behind the wastewater data, and the recent increase was so steep that the difference is most noticeable in the last month
- Viral load expelled in wastewater is higher with different new variants
- New variants infect animals, which contribute to viral load in the water
- The measured areas overlap, but are different: Middlesex County for positive tests, and the northern MWRA region for wastewater measurements. Perhaps the Northern MWRA region has a higher rate of cases than Middlesex County.

If anyone is researching this, has expert knowledge, or knows of journal articles on it, let me know.

# Install and run

- Install [`poetry`](https://python-poetry.org)
- Install python dependencies via `poetry install`
- Run `jupyter notebook plot-covid-wastewater.ipynb`
