# boston_crime

## Context: 
Understanding patterns in crime rates is a topic of major interest for policymakers and law enforcement. Whereas research historically focused on socio-demographics such as age, gender, or socio-economic status, modern approaches also consider contextual factors to criminal behavior. More recently, weather parameters such as temperature, precipitation, or wind speed were found to play a pivotal role in understanding crimes. Crime rates of major US cities and regions correlate significantly with temperature. This project investigates the weather impact on Boston crime rates by applying correlation analysis, significance tests, and linear regression.

## Research Question:
This project investigates the extent to which weather parameters can explain variation in daily crimes in Boston in 2021. Furthermore, weekly, monthly, and annual patterns are researched.

## Data & Processing Steps:
Data from two sources are combined, standardized (z-score), and detrended before statistical testing. First, to calculate daily crime rates, the API of the Boston Police Department is called for the timespan between January 1st and December 31st, 2021. The time-series data is then joined with weather data requested through the national oceanic and atmospheric administration NOAA. The final dataset consists of 365 entries containing daily records of crime rates, average temperature, rain- and snowfall, and wind speed. The two additional data fields ‘day-of-week’ and ‘day-of-month’, are added to investigate weekly or monthly patterns. The data retrieved from the Boston Police Department further includes the category of registered incidents and their geo-location. Several incident types are removed from the dataset as they are not criminal offenses (e.g., Medical Assistance).

## References:
- Page Link https://rpubs.com/wypa93/888578
- Crime Incident Reports BPD https://data.boston.gov/
- NCDC NOAA Climate Data https://www.ncdc.noaa.gov/
