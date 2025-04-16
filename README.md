# CDDS Heat Metrics

Heat stress is one of the leading causes of weather-related injuries and deaths. This is an increasingly concerning problem due to the rising summer temperature extremes globally in recent years. This research repository contains the calculation of different heat metrics specifically on ERA5's hourly dataset spanning from 1940-2024.

There are currently two metrics included in the study: heat-index and wetbulb temperature.

## Files

#### ERA5_heat_calculations

This notebook contains all the workflow to calculate [NOAA's heat index](https://www.wpc.ncep.noaa.gov/html/heatindex_equation.shtml) and [wetbulb temperature](https://journals.ametsoc.org/view/journals/apme/50/11/jamc-d-11-0143.1.xml) using surface temperature and dewpoint.

For this study, I use [analysis-read ERA5](https://github.com/google-research/arco-era5)'s hourly dataset spanning from 1940-2024.

You can use my fork repository to retrieve the data. Original repository by Maile Sasaki
[https://github.com/KChoodam/climate_map/tree/main]

#### ERA5_analysis

This notebook apply sklearn's QuantileRegressor to different calculated metrics and display it as images.

### figures Folder

This contains all the output images

### ICN Folder

This will be used to compare between station data and ERA5 outputs


### Legacy Folder

Legacy folder consists of files that were used previously. They have a similar workflow, but they are a lot messier. You can just ignore this

#### Data_validation 
This is simply for me to make sure all the data downloaded from [ERA5](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-pressure-levels?tab=overview). 
