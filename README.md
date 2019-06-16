# Time-Series-Predicition-for-Energy-Consumption
Time Series Prediction for Energy Consumption
Context
To better follow the energy consumption, the government wants energy suppliers to install smart meters in every home in England, Wales and Scotland. There are more than 26 million homes for the energy suppliers to get to, with the goal of every home having a smart meter by 2020.

This roll out of meter is lead by the European Union who asked all member governments to look at smart meters as part of measures to upgrade our energy supply and tackle climate change. After an initial study, the British government decided to adopt smart meters as part of their plan to update our ageing energy system.

In this dataset, you will find a refactorised version of the data from the London data store, that contains the energy consumption readings for a sample of 5,567 London Households that took part in the UK Power Networks led Low Carbon London project between November 2011 and February 2014. The data from the smart meters seems associated only to the electrical consumption.

There is infomations on the ACORN classification details that you can find in this report or the website of CACI.

I added weather data for London area, I used the darksky api to collect this data.

Content
There is 19 files in this dataset :

informations_households.csv : this file that contains all the information on the households in the panel (their acorn group, their tariff) and in which block.csv.gz file their data are stored

halfhourly_dataset.zip: Zip file that contains the block files with the half-hourly smart meter measurement

daily_dataset.zip: Zip file that contains the block files with the daily information like the number of measures, minimum, maximum, mean, median, sum and std.

acorn_details.csv : Details on the acorn groups and their profile of the people in the group, it's come from this xlsx spreadsheet.The first three columns are the attributes studied, the ACORN-X is the index of the attribute. At a national scale, the index is 100 if for one column the value is 150 it means that there are 1.5 times more people with this attribute in the ACORN group than at the national scale. You can find an explanation on the CACI website

weather_daily_darksky.csv : that contains the daily data from darksky api. You can find more details about the parameters in the documentation of the api

weather_hourly_darksky.csv : that contains the hourly data from darksky api. You can find more details about the parameters in the documentation of the api

Acknowledgements
All the big work of data collection has been done by the UK power networks for the smart meter data.

The details related at the acorn group are provided by the CACI.

The weather data are from darksky.

Inspiration
For me some ideas to analyze the data:

Segmentation of the consumption daily pattern
Disaggregation of the electricity load curve
Cross the consumption result and the acorn information
Forecast the electricity consumption of a household, I wrote an article on this subject
What if I add electrical heating system ? an EV battery system ?
Forecast at a global scale (London consumption)
