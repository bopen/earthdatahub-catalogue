ERA5 is the fifth generation ECMWF reanalysis for the global climate and weather for the past 8 decades.
Data is available from 1940 onwards.

Reanalysis combines model data with observations.
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
10-member ensemble at three-hourly intervals. Ensemble mean and spread have been pre-computed for convenience.
Such uncertainty estimates are closely related to the information content of the available observing system
which has evolved considerably over time. They also indicate flow-dependent sensitive areas.
Single levels variables are computed at one vertical level which can be surface (or a level close to the
surface) or a dedicated pressure level in the atmosphere.

Here we propose a focus on ERA5 hourly data on single levels (atmospheric, ocean-wave and land surface quantities) from 1940 to 2023

How to access:

```python

import xarray as xr

    ds = xr.open_dataset(
        "s3://hedp/era5/reanalysis-era5-single-levels-1940-2023.zarr",
        engine="zarr",
        chunks={},
    )
```