# Tableau: NYC Citi Bikes: Q1 2018, 2019 & 2020
--------------------------------------------------
## by Shane Gatenby
--------------------------------------------------
### https://github.com/shanergy/Tableau-challenge.git
### https://public.tableau.com/profile/shane.gatenby#!/vizhome/Tableau_Citi_Bikes/CitiBike

--------------------------------------------------
#### Data Source
* citibike.nyc.com
  * https://www.citibikenyc.com/system-data
  * January - March 2018
  * January - March 2019
  * January - March 2020

  * NOTE: NYC only; not including Jersey City Stations or rides originating within Jersey City.


--------------------------------------------------
#### Key Files:
1) Python / jupyter notebook file (github repo: shanergy/Tableau-challenge: Citi_Bike_Trip_Data_v3.ipynb)
    1) Used to combine 9 downloaded CSV files (one for each month, Jan - Mar, making up the first quarter for each year, 2018 - 2020)
    2) All 9 CSVs were unioned/concatonated together for one solid dataset (easing the strain of bringing them in and letting Tableau do the heavy lifting)
    3) Cleaned the data by removing data with null station names, ids, lats
    4) One CSV was exported that was then used in Tableau
    5) Normalized Citi Bike Station Data (for instances where there was a variance in Lat/Long and Station ID, but same Station Name - used the most recent value for each station for plotting on a map)
    6) For some reason there were station data coming from stations in Montreal, Canada - these were eliminated from the final dataset.
2) Tableau / .twbx file (uploaded to Tableau Public: https://public.tableau.com/profile/shane.gatenby#!/vizhome/Tableau_Citi_Bikes/CitiBike)
    1) 1 Story: highlighting the dashboards, providing quick analysis points
    2) 3 Dashboards: covering the two noticed phenomena along with a third that was fascinating to see the most and least used stations and routes...especially utilizing the interactive features tableau provides.
    3) Multiple visualizations and analysis notes included.

--------------------------------------------------
#### Analysis & Notes:
1) Observed Phenomena 1: 2020 & impacts of COVID-19
    1) Year-over-year for the first three months of the first quarter (January, February and March) for 2018 and 2019, Citi Bike ridership increases at what appears to a growing trend, however for 2020 - this is not observed.  In fact, month-over-month for 2020, this appears to flatten in March.  March 2020 trips are less than those in February, which are less than those in January.  This may very well likely be due to the coronvirus  and New York City becoming a pandemic hotspot.
    2) Other interesting trends noted are the average trip duration is notably higher March 2020 over previous March periods and non-subscriber/customer rides percentages also increase, perhaps implying regular commuter usage is down.
2) Observed Phenomena 2: User Demographics
    1) Citi Bikes are considerably more popular with Men over Women, by a factor of at least 3x.  Subscriber rides far out-weigh non-subscriber customers and average trip duration spikes on the weekends (although overall trips are fewer).  
    2) Popular hours of usage on weekdays for subscribers contrast sharply to during the work week where they spike at each end of the workday.  For non-subscriber customers, this trend is NOT observed, suggesting that subscribers are utilizing Citi Bikes for commuting purposes, whereas non-subscribers are not.
3) Map Trends/Analysis (discovered while making the map)
    1) Mid-town, Mid-town, Mid-town is the hot spot (for Citi Bikes, at least).  Citi Bike stations are clustered heavily on the island of Manhattan, with an epicenter noticably hovering over mid-town.  Also, the most number of rides originate at these stations.
    2) Far fewer rides originate the further out you get from Mid-town.  Living is just, or nearly as dense on the Upper East and West Sides, but fewer trips originate at these stations.  Once you get out of Manhattan, stations exist in parts of Queens and Brooklyn, but stations are far more scattered and used far less.

