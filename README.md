Scrape the [Massachusetts Water Resources Authority (MWRA) wastewater COVID-19 data](https://www.mwra.com/biobot/biobotdata.htm) from a PDF, save it as a csv file, and plot it.

[Download the data as a csv](covid-19-wastewater.csv)

# Viral RNA copies per mL of wastewater, 7 day average

## Northern region

![A line graph, showing covid prevalence for the northern region in RNA copies/mL 7 day average over time. The most recent month, Dec 2021, has a spike 10x higher than any previous record. There are smaller peaks in April 2020 and December 2020 to February 2021 but they are dwarfed by the recent spike.](north.png "The Northern Region's covid prevalence")

## Southern region

![A line graph, showing covid prevalence for the southern region in RNA copies/mL 7 day average over time. The most recent month, Dec 2021, has a spike 10x higher than any previous record. There are smaller peaks in April 2020 and December 2020 to February 2021 but they are dwarfed by the recent spike.](south.png "The Northern Region's covid prevalence")

## Map of the two regions

![A map of the boston metro area, divided into two regions. A green northern region and a orange southern region. In the west is the boston harbor and there's a black dot there, on a peninsula in Winthrop. That's the wastewater treatment plant. The northern region has the comprises the following towns: Bedford, Wilmington, Burlington, Lexington, Waltham, Reading, Woburn, Winchester, Wakefield, Stoneham, Melrose, Medford, Arlington, Belmont, Malden, Watertown, Somerville, Everett, Revere, Chelsea, Cambridge, Winthrop, Boston, and the northern parts of Newton, Brookline, and Boston. The southern region comprises the following towns: Ashland, Walpole, Stoughton, Holbrook, Weymouth, Hingham, Framingham, Natick, Wellesley, Needham, Dedham, Westwood, Canton, Randolph, Braintree, Quincy, Milton, and the southern parts of Newton, Brookline, and Boston.](map.jpg "The northern and southern MWRA wastewater regions")

# Install and run

- Install [`poetry`](https://python-poetry.org)
- Install python dependencies via `poetry install`
- Run `jupyter notebook plot-covid-wastewater.ipynb`
