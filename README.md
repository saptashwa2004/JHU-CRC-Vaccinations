# Coffee, Cookie and Coding $\left(C^3\right)$

From Yale's Public Health Data Science and Data Equity (DSDE) Team

Workshop: Getting Started with Git and GitHub

Platform: Hybrid

Date: November $4^{\text{th}}$, 2024

## About The Workshop

These workshops are created by the DSDE data science team to assist Public Health and Biostatistics masters-level students effectively leverage computational tools and analytical methods in their educational and future professional endeavors.

We will be launching our Coffee, Cookie and Coding $\left(C^3\right)$ workshops with a starter guide on Git and GitHub. Upon completing the workshop, you will be able to:
- Understand why it is good to learn to use Git and GitHub.
- Configure your local Git and personal GitHub accounts and set up security keys.
- Learn how to share and contribute to projects with an example created in RStudio.

The live workshop is not recorded, however, videos that complement the live session are posted on our groups YouTube (link) page and website (link). These cover the same material as was done in the live workshop.

Please find out more about our group on our lab website (Mukherjee lab website link). You can reach us ___.

## About This Repository

This GitHub repository is one of two that was used in the workshop. The other repository can be found [JHU-CRC-Cases-and-Recoveries](https://github.com/ysph-dsde/JHU-CRC-Cases-and-Recoveries).

Enclosed are the Analysis, Cleaning, and Harmonization R scripts with their associated files. Users of this repository will only need to open the Analysis Script_Vaccinations Time-Series Plot.R, as the cleaning and census harmonization scripts have already been run to generate the necessary files called in the analysis workflow.

NOTE: Re-running the cleaning script might result in result variations as a product of the isotonic regression.

This project uses a renv() lock so that the enviroment is reporducible for all users. Here we used R version 4.4.1. Users not using this version of R may experience problems running the script, even with the renv() activated. After initially establishing your local copy (mirror) from this remote repository, activate the enviroment by runing ``renv::restore()`` in the R Console and following the prompts.

NOTE: You may need to run ``renv::restore()`` twice to initialize and install all the packages indicated for by the lockfile. You know you are all set to go when running ``renv::restore()`` gives you ``- The library is already synchronized with the lockfile.``

## About The Data Used

The [Johns Hopkins Coronavirus Resource Center](https://coronavirus.jhu.edu/) (JHU CRC) tracked and made publically available COVID-19 pandemic data from January 22, 2020 and March 10, 2023. Here, we imported cumulative vaccination counts for the U.S. from their [GovEX/COVID-19](https://github.com/govex/COVID-19/tree/master/data_tables/vaccine_data) GitHub repository. The raw data used in the analysis script can be found in the data_tables/vaccine_data/us_data/time_series subdirectory ([original source](https://github.com/govex/COVID-19/blob/master/data_tables/vaccine_data/us_data/time_series/time_series_covid19_vaccine_us.csv)).

The data dictionary provided by JHU CRC has been copied to this repository ([original source](https://github.com/govex/COVID-19/tree/master/data_tables/vaccine_data/us_data)). Additional details and methods for harmonizing the U.S. Census Bureau's 2010 to 2019 population projections with 2020 to 2023 vintages can be found in the "Population Estimates and Projections" subdirectory.







