This is a subset of ERA5 data on single-levels variables derived from [ERA5 post-processed daily statistics on single levels from 1940 to present](https://doi.org/10.24381/cds.4991cf48). The data is available from 1940 until the last closed month and updated monthly and is gridded to a regular lat-lon grid of 0.25 degrees.

They are presented as a Zarr v3 archive optimised for both spatial and time analysis.

This dataset is produced by the Earth Data Hub Team based on the
[ERA5 hourly data on single levels](./reanalysis-era5-single-levels) dataset
and uses the standard UTC day as a base for averages and accumulations.
That is, the day starts at 00:00 UTC and ends at 23:59 UTC
on all pixels irrespective of the latitude and the local time.
Note that for accumulated variables, like the _total precipitation_ `tp`, the original
ECMWF data resets the values at the start of the UTC day on all latitudes already.

For instantaneous variables, e.g. the _2 meter temperature_ `t2m`, the operation applied is
the Xarray `.resample("D").mean()` method.
For accumulated variables the values are the total accumulation for the day.

Accessing this dataset requires a Zarr v3-compatible library (e.g., zarr-python >= 3.x). Python users can upgrade via `pip install "zarr>3"`.
