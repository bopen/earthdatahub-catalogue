ERA5-Land is a reanalysis dataset providing a consistent view of the evolution of land variables
over several decades at an enhanced resolution compared to ERA5.

ERA5-Land has been produced by replaying the land component of the ECMWF ERA5 climate reanalysis.
Reanalysis produces data that goes several decades back in time, providing an accurate description of the climate of the past.


The ERA5-Land dataset, as any other simulation, provides estimates which have some degree of uncertainty.
Numerical models can only provide a more or less accurate representation of the real physical processes governing different
components of the Earth System. In general, the uncertainty of model estimates grows as we go back in time,
because the number of observations available to create a good quality atmospheric forcing is lower.
ERA5-land parameter fields can currently be used in combination with the uncertainty of the equivalent ERA5 fields.


The temporal and spatial resolutions of ERA5-Land makes this dataset very useful
for all kind of land surface applications such as flood or drought forecasting.
The temporal and spatial resolution of this dataset, the period covered in time,
as well as the fixed grid used for the data distribution at any period enables decisions makers,
businesses and individuals to access and use more accurate information on land states.


Here we propose a focus on Europe ERA5-Land hourly data from 1950 to 2023 as a zarr store optimised for time-analysis.

Access is free to registered user thank to the support of the Destination Earth initiative.


How to access:


```python

import xarray as xr

ds = xr.open_dataset(
    "s3://ecmwf-era5-land/reanalysis-era5-land-no-antartica-v0.zarr",
    engine="zarr",
    chunks={},
    storate_options={"enpoint_url": "https://s3.gra.perf.cloud.ovh.net"}
)
```