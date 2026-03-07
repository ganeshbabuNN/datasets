https://nycflights13.tidyverse.org/

Source of data :https://www.transtats.bts.gov/releaseinfo.asp

This package contains information about all flights that departed from NYC (e.g. EWR, JFK and LGA) to destinations in the United States, Puerto Rico, and the American Virgin Islands) in 2013: 336,776 flights in total. To help understand what causes delays, it also includes a number of other useful datasets.

This package provides the following data tables.

flights: all flights that departed from NYC in 2013
weather: hourly meterological data for each airport
planes: construction information about each plane
airports: airport names and locations
airlines: translation between two letter carrier codes and names

If you’re interested in other subsets of flight data, see:
nycflights for flights departing from NYC in the last year.
anyflights for flights departing from any airport in any year.
airlines to maintain a local SQL database of all flight departure data.

Flights:
=======
On-time data for all flights that departed NYC (i.e. JFK, LGA or EWR) in 2013.

Format
Data frame with columns

year, month, day
Date of departure.

dep_time, arr_time
Actual departure and arrival times (format HHMM or HMM), local tz.

sched_dep_time, sched_arr_time
Scheduled departure and arrival times (format HHMM or HMM), local tz.

dep_delay, arr_delay
Departure and arrival delays, in minutes. Negative times represent early departures/arrivals.

carrier
Two letter carrier abbreviation. See airlines to get name.

flight
Flight number.

tailnum
Plane tail number. See planes for additional metadata.

origin, dest
Origin and destination. See airports for additional metadata.

air_time
Amount of time spent in the air, in minutes.

distance
Distance between airports, in miles.

hour, minute
Time of scheduled departure broken into hour and minutes.

time_hour
Scheduled date and hour of the flight as a POSIXct date. Along with origin, can be used to join flights data to weather data.

Source
RITA, Bureau of transportation statistics, https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236


weather:
=======
Hourly meterological data for LGA, JFK and EWR.


Format
A data frame with columns:

origin
Weather station. Named origin to facilitate merging with flights data.

year, month, day, hour
Time of recording.

temp, dewp
Temperature and dewpoint in F.

humid
Relative humidity.

wind_dir, wind_speed, wind_gust
Wind direction (in degrees), speed and gust speed (in mph).

precip
Precipitation, in inches.

pressure
Sea level pressure in millibars.

visib
Visibility in miles.

time_hour
Date and hour of the recording as a POSIXct date.

Source
ASOS download from Iowa Environmental Mesonet, https://mesonet.agron.iastate.edu/request/download.phtml.


planes:
=======
Plane metadata.
Plane metadata for all plane tailnumbers found in the FAA aircraft registry. American Airways (AA) and Envoy Air (MQ) report fleet numbers rather than tail numbers so can't be matched.

Format
A data frame with columns:

tailnum
Tail number.

year
Year manufactured.

type
Type of plane.

manufacturer, model
Manufacturer and model.

engines, seats
Number of engines and seats.

speed
Average cruising speed in mph.

engine
Type of engine.

Source
FAA Aircraft registry, https://www.faa.gov/licenses_certificates/aircraft_certification/aircraft_registry/releasable_aircraft_download/


airports
=========
Airport metadata
Useful metadata about airports.

Format
A data frame with columns:

faa
FAA airport code.

name
Usual name of the aiport.

lat, lon
Location of airport.

alt
Altitude, in feet.

tz
Timezone offset from GMT.

dst
Daylight savings time zone. A = Standard US DST: starts on the second Sunday of March, ends on the first Sunday of November. U = unknown. N = no dst.

tzone
IANA time zone, as determined by GeoNames webservice.

Source
https://openflights.org/data.html, downloaded 2014-06-27


airlines
========
Airline names.
Look up airline names from their carrier codes.

Format
Data frame with columns

carrier
Two letter abbreviation.

name
Full name.

Source
https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236