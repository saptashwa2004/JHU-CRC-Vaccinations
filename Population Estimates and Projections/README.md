# U.S. POPULATION ESTIMATES AND PROJECTIONS
## JHU CRC Source

The Johns Hopkins Coronavirus Resource Center (JHU CRC) GitHub page ([GovEX - US Country Map](https://github.com/govex/COVID-19/tree/master/data_tables/Data_for_UScounty_map)) sourced their population estimates and projections from the [U.S. Department of Agriculture Economic Research Services](https://www.ers.usda.gov/) Data Products site. The report version JHU CRC downloaded is based on the 2010 Census year and includes vintages up through 2018. All U.S. states and Puerto Rico were reported, but no other U.S. Territories are present nor does it include calculations by U.S. state regions or districts. A copy of this report is included here: "U.S. Department of Agriculture_Population Estimates 2010 to 2018_JHU CRC.xls".

The U.S. Department of Agriculture methods indicate that their reports are compiled from county-level U.S. census vintages that are released by the U.S. Census Bureau each year. These vintage releases include population estimates and projections for intercensal data at the state and county-level for all U.S. states and Puerto Rico. All estimates and projections are made using their “Official U.S. Estimates” method ([Table of Population Data Sources for U.S. Areas](https://www.census.gov/programs-surveys/international-programs/about/idb/island-areas.html)).


## Harmonizing census vintages from 2010-2023 for U.S. States and Puerto Rico

The U.S. Department of Agriculture currently displays population estimates and projections based on the 2020 Census with vintages up through 2023 ([County-level Data Sets](https://www.ers.usda.gov/data-products/county-level-data-sets/county-level-data-sets-download-data/)). Maintainers of this site indicated that the 2010-2019 vintage need to be sourced directly from the U.S. Census Bureau website.

The U.S. Census Bureau vintage for 2010-2019 at the county-level appeared to be missing the total state-level counts for Puerto Rico, but included county-level data ([County Population Totals: 2010-2019](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-counties-total.html)). For accuracy, the total counts were not assumed to be aggregates of the counties present in the provided data set; it was not explored whether all possible counties in Puerto Rico were present in this report.

State-level only reports included all U.S. states and Puerto Rico, and we found that the “alldata” version of the data sets were mostly complete ([State Population Totals: 2010-2019](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-state-total.html) and [State Population Totals and Components of Change: 2020-2023](https://www.census.gov/data/datasets/time-series/demo/popest/2020s-state-total.html)). These reports also included calculations over the U.S. state regions and districts ([Regional and Districts Map](https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf)). One exception was found: the 2020 Census year data was missing from the 2020-2023 vintage. Notice that this information is treated as static between vintage reports, as this information reflects the counts observed in the 2020 Census.

The two state-level vintage releases from the U.S. Census Bureau and 2020 Census year observations from the U.S. Department of Agriculture (link above) were harmonized into a complete 2010-2023 population estimates and projections table for all U.S. states and Puerto Rico.


## Harmonizing census vintages from 2010-2023 for the remaining U.S. Territories




## Other notes

Each year the U.S. Census Bereau releases additional projections, where all estimates are revised from April 1st of the census year through July 1st of the current year. This new vintage of estimates draws from the most current input data and employes methodological improvements that make these estimates superior to prior releases (U.S. Census Bereau's [Methods for County Population Totals: 2010-2019](https://www2.census.gov/programs-surveys/popest/technical-documentation/methodology/2010-2019/natstcopr-methv2.pdf)).

Please see the "Census Data Harmonization Script.R" comments for further details describing the harmonization steps taken and accuracy checks completed to ensure that data integrety is maintained.


New sources:
- U.S. Territories [2010 to 2023](https://www.census.gov/data-tools/demo/idb/#/table?COUNTRY_YEAR=2024&COUNTRY_YR_ANIM=2024&menu=tableViz&quickReports=CUSTOM&CUSTOM_COLS=POP,GR,RNI,NATINCR,CBR,BIRTHS,CDR,DEATHS,NMR,NIM&TABLE_YEARS=2010,2011,2012,2013,2014,2015,2016,2017,2018,2019,2020,2021,2022,2023&TABLE_USE_RANGE=Y&TABLE_USE_YEARS=N&TABLE_STEP=1&TABLE_ADD_YEARS=2010,2020&CCODE_SINGLE=AS&CCODE=AS,GU,MP,PR,US,VI&TABLE_RANGE=2010,2023)


Notes:
- [Population Estimates and Projections for the U.S. Island Areas](https://www.census.gov/programs-surveys/international-programs/about/idb/island-areas.html)
- [Impact of 2020 on Island Census](https://www.census.gov/newsroom/press-releases/2024/2020-island-areas-cross-tabulation-american-samoa.html)
- About [Pupulation Estimates](https://www.census.gov/programs-surveys/popest/about.html).
- About [Population Projections](https://www.census.gov/programs-surveys/popproj/about.html).

