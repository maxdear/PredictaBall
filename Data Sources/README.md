# Data Sources


### Match Data
The data for each match was downloaded from [football-data](http://www.football-data.co.uk/) in CSVs for each season (18/19 & 19/20) and then later merged together.

### League Table Data
The league table data was scraped from [TWTD.co.uk](https://www.twtd.co.uk/league-tables/competition:premier-league/daterange/) by using the date as a varaible and so downloading the table standings for every day of the required time period.
[shown here](https://github.com/maxdear/PredictaBall/blob/master/Notebooks/1.%20Web%20Scraping%20League%20Position.ipynb).


### Team ELO Data
A team's history of ELO statistics was downloaded through [Club ELO's API](http://clubelo.com/API) by using the team names that occur in the match data.
[shown here](https://github.com/maxdear/PredictaBall/blob/master/Notebooks/2.%20Teams%20ELO.ipynb).
