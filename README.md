# Climate Data Analysis

Using PySpark, the project processes climate data.  Data is initially obtained from https://www1.ncdc.noaa.gov/pub/data/ghcn/v4/ and the file ```ghcnm.tavg.v4.0.1.20200407.qcf.dat``` is first processed by ```DatToJson2.py```.  This reduces the .dat file to an ~100 MB single line JSON file which is processed by ```DatSpark.py```.

Program calculates the average yearly temperature change for a given country code and year range, and the average temperature change over that time.  Displays temperature recordings for that timeframe in a Pyplot graph.

ClimatePaper.pdf has implementation details as well as an analysis of the results and performance analytics for running the program on a Raspberry Pi cluster.

To run, download spark, findspark, and pandas, and make pathnames specific to your machine.  You will run into issues if not using Java 8.
