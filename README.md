chirps-stars
================

*Exploration of CHIRPS data using R and the stars package for handling NetCDF files.*

CHIRPS data
-----------

"The Climate Hazards Group Infrared Precipitation with Station data (CHIRPS) is a high-resolution climatic database of precipitation embracing monthly precipitation climatology, quasi-global geostationary thermal infrared satellite observations from the Tropical Rainfall Measuring Mission (TRMM) 3B42 product, atmospheric model rainfall fields from National Oceanic and Atmospheric Administration – Climate Forecast System (NOAA CFS), and precipitation observations from various sources." (Retalis et al. 2017)

Overall it is a combination of station-base observations around the world, and satellite derived data for meteorology, including TRMM and NOAA, which are normally used for precipitation analysis.

The data covers information from 1981 to the present on a daily, monthly, yearly and decadal basis. It spans latitudes between 50°S and 50°N and all longitudes. The data is presented in a raster format with a cell siye of 0.05° or 0.25°. Each of the cells represent a rain gauge (Funk et al. 2015).

Data download
-------------

The global daily data which will be analyzed can be downloaded per year, either as a NetCDF file, where each band corresponds to a day; or daily as TIFF files. In this case I decided to work with NetCDF files and will explain how to explore the data using R and the `stars`package.

The data can be downloaded from this link (<ftp://ftp.chg.ucsb.edu/pub/org/chg/products/CHIRPS-2.0/>)[1]. To explore initially the data, I will use the year 2019 at 0.05° resolution, which has information up to February.

References
==========

Funk, Chris, Pete Peterson, Martin Landsfeld, Diego Pedreros, James Verdin, Shraddhanand Shukla, Gregory Husak, et al. 2015. “The climate hazards infrared precipitation with stations—a new environmental record for monitoring extremes.” *Scientific Data* 2 (December). Nature Publishing Group: 150066. doi:[10.1038/sdata.2015.66](https://doi.org/10.1038/sdata.2015.66).

Retalis, Adrianos, Filippos Tymvios, Dimitrios Katsanos, and Silas Michaelides. 2017. “Downscaling CHIRPS precipitation data: an artificial neural network modelling approach.” *International Journal of Remote Sensing* 38 (13). Taylor & Francis: 3943–59. doi:[10.1080/01431161.2017.1312031](https://doi.org/10.1080/01431161.2017.1312031).

[1] ftp links not working in Markdown.
