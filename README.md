# ENV872project, EPA Ozone Dataset and United States Census Bureau Demographic Data

## Summary
The Ozone dataset was created by Professor that prepared for ENV 872 Environmental Data Analytics at Duke University, Spring 2019. It contains EPA air quality data for ozone in 2017 and 2018 in North Carolina.

The Demographic Data contains population size, population density, and Median household income for different counties in North Carolina.

## Database Information
According to Readme_EPAair_PM25andO3 file created by professor,
"Data were collected from the North Temperate Lakes Long Term Ecological Research website. More information can be found here: https://lter.limnology.wisc.edu/about/overview

Data were collected using the Doanload Daily Data tool (https://www.epa.gov/outdoor-air-quality-data/download-daily-data).
The following selections were made: 
* PM2.5 and Ozone (Pollurant)
* 2017 and 2018 (Year)
* North Carolina (Geographic Area)
* Download CSV (spreadsheet)"

The demographic data is collected from United States Census Bureau Demagraphic Data https://www.census.gov/quickfacts/. Sections including population size, population density, and Median household income are searched for the corresponding counties listed in Ozone dataset. The numbers were manually collected.

csv files were saved as `EPAair_O3_NC2017_raw.csv`, `EPAair_O3_NC2018_raw.csv`, `OzoneSummary1.csv`,

Ozone Data were accessed 2018-12-10; Demographic Data were accessed 2019-04-10.

## Data Content Information
In the Ozone data, the content includes: 
"Date: month/day/year
Source: AQS (Air Quality System) or AirNow
Site ID: A unique number within the county identifying the site.
POC: “Parameter Occurrence Code” used to distinguish different instruments that measure the same parameter at the same site.
Daily Mean PM2.5 Concentration: numeric value
Daily Max 8-hour Ozone Concentration: numeric value
Units: units for concentration

Daily_AQI_VALUE: Air quality index (range 0-500). Levels: 
0-50: Good (green)
51-100: Moderate (yellow)
101-150: Unhealthy for sensitive groups (orange)
151-200: Unhealthy (red)
201-300: Very unhealthy (purple)
301-500: Hazardous (maroon)"
Reference: https://www.epa.gov/outdoor-air-quality-data/air-data-basic-information

Site Name
DAILY_OBS_COUNT: number of observations per day
PERCENT_COMPLETE
AQS_PARAMETER_CODE
AQS_PARAMETER_DESC
CBSA_CODE
CBSA_NAME
STATE_CODE
STATE
COUNTY_CODE
COUNTY
SITE_LATITUDE
SITE_LONGITUDE"

In the demographic data, the content includes: 
COUNTY, 
MeanOzoneAQI : Calculated from ozone data and grouped by county,
Population,
Density,
Income: Median Household Income in the county.

## Naming conventions and file formats
Files are named with descriptive information, and the format are .csv that can be imported to R directly.

## Additional Information and Support
For more information, please contact **Qianyi Xia** (qianyi.xia@duke.edu)