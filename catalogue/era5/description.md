ERA5 is the fifth generation ECMWF reanalysis for the global climate and weather for the past 8 decades.
Data is available from 1940 onwards on ECWMF [Copernicus Data Store](https://cds.climate.copernicus.eu/).

ERA5 provides hourly estimates of a large number of atmospheric, land and oceanic climate variables. The data cover the Earth on a 30km grid and resolve the atmosphere using 137 levels from the surface up to a height of 80km. ERA5 includes information about uncertainties for all variables at reduced spatial and temporal resolutions.

We propose a subset of the whole corpus of data based on the most popular datasets and variables. Specifically speaking ERA5 Land, ERA5 Single Levels, ERA5 pressure level and Essential Climate Variables (ECV) on selected variables. Furthermore ERA5 monthly data on single level have been added.

Datasets are presented as Zarr archives optimised specifically for time analysis and covering the whole available geographical and temporal extent of the original data. Also, resolution is preserved and data are updated until the last closed month with monthly updates.

Please refer to the specific datasets for detailed information about extent, resolution, updates and access rights.


<!--- Reanalysis combines model data with observations.
This principle, called data assimilation, is based on the method used by numerical
weather prediction centres, where every so many hours (12 hours at ECMWF) a previous
forecast is combined with newly available observations to produce
a new best estimate of the state of the atmosphere, called analysis, from which an updated,
improved forecast is issued.

Reanalysis works in the same way, but at reduced resolution
to allow for the provision of a dataset spanning back several decades.
Reanalysis does not have the constraint of issuing timely forecasts,
so there is more time to collect observations, and when going further back in time,
to allow for the ingestion of improved versions of the original observations,
which all benefit the quality of the reanalysis product.

ERA5 provides hourly estimates for a large number of atmospheric,
ocean-wave and land-surface quantities. An uncertainty estimate is sampled by an underlying
10-member ensemble at three-hourly intervals. Ensemble mean and spread have been pre-computed for convenience. Such uncertainty estimates are closely related to the information content of the available observing system
which has evolved considerably over time. They also indicate flow-dependent sensitive areas.--->
