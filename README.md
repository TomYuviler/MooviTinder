![Screenshot](logo.png)
# MooviTinder
MooviTinder Apllication - Tom Yuviler &amp; Lidor Asulin - Technion

## Overview
The MooviTinde application hepls the user to finde the fastest possible way to get from  an origin point in Dublin and to get to the desiered desteniation (in Dublin) by using Dublin bus. By activate the Tinder Mode, the user will be able to see other users that chose neraby destination.

## Find the fastest possible way
By setting the origin point (coordinates: logintude and latitude) and the destination point (coordinates: logintude and latitude) by the user the apllication will show the user the fastest possible travel by using Dublin bus. the calculation of the travel time is based on four different calculations:
1. **Walking time from origin point to the bus station:** the apllication calculate the distance between the origin point to every bus stastion in Dublin. The estimated walking time based on the assumption of walkin 1 meter per second. The relvant data (accurate locations and names) regarding the bus stastions was download from https://data.gov.ie/dataset/bus-stops-served-by-dublin-bus, and was inegretad to to Dublin bus data.
2. **Waiting time in the bus station:** The calculations of the waiting time in the bus station is based on streaming/online data - for each journey pattern of each bus line the apllication finds the last stop of the bus, and the time that passed from the stop, and integrate it with the estimation of the travel time between two bus stations (based on offline data - read from Elasticsearch - see part 3). 
3. **Travel time between two bust stations:** FOR RAC.





