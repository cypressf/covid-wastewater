Scrape the [Massachusetts Water Resources Authority (MWRA) wastewater COVID-19 data](https://www.mwra.com/biobot/biobotdata.htm) from a PDF, save it as a csv file, and plot it vs the [New York Times reported covid case numbers](https://github.com/nytimes/covid-19-data).

# The Data

[Download the data as a csv](covid-19-wastewater.csv)

## Measured COVID-19 in Wastewater vs Reported Cases in Middlesex County, Massachusetts

Note how the wastewater measurements are much higher than the reported cases in the most recent month. This could be because testing isn't keeping up with case numbers. Perhaps more people are testing at home, perhaps the testing is too slow and it's lagging behind, or perhaps many people are asymptomatic and are not testing.

![A line graph, showing covid prevalence for the northern region in RNA copies/mL 7 day average over time. The most recent month, Dec 2021, has a spike 10x higher than any previous record. There are smaller peaks in April 2020 and December 2020 to February 2021 but they are dwarfed by the recent spike. It also shows the reported cases, which follow the trend of the wastewater measurements, except the most recent spike is about 1/5 the height](wastewater-vs-reported.png "The Northern Region's covid prevalence")

## Map of the wastewater regions

![A map of the boston metro area, divided into two regions. A green northern region and a orange southern region. In the west is the boston harbor and there's a black dot there, on a peninsula in Winthrop. That's the wastewater treatment plant. The northern region has the comprises the following towns: Bedford, Wilmington, Burlington, Lexington, Waltham, Reading, Woburn, Winchester, Wakefield, Stoneham, Melrose, Medford, Arlington, Belmont, Malden, Watertown, Somerville, Everett, Revere, Chelsea, Cambridge, Winthrop, Boston, and the northern parts of Newton, Brookline, and Boston. The southern region comprises the following towns: Ashland, Walpole, Stoughton, Holbrook, Weymouth, Hingham, Framingham, Natick, Wellesley, Needham, Dedham, Westwood, Canton, Randolph, Braintree, Quincy, Milton, and the southern parts of Newton, Brookline, and Boston.](map.jpg "The northern and southern MWRA wastewater regions")

# Install and run

- Install [`poetry`](https://python-poetry.org)
- Install python dependencies via `poetry install`
- Run `jupyter notebook plot-covid-wastewater.ipynb`
