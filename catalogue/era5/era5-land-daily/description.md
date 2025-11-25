This is a subset of ERA5 data for world land surface quantities called [ERA5-Land daily data from 1950 to present](https://doi.org/10.24381/cds.e2161bac). The data are available from 1950 until the last closed month and updated monthly and are regridded to a regular lat-lon grid of 0.1 degrees.

They are presented as a NetCDF / Zarr archive optimised for both spatial and time analysis.

This dataset is produced by the Earth Data Hub Team based on the
[ERA5-Land hourly data](./reanalysis-era5-land) dataset
and uses the standard UTC day as a base for averages and accumulations.
That is, the day starts at 00:00 UTC and ends at 23:59 UTC
on all pixels irrespective of the latitude and the local time.
Note that for accumulated variables, like the _total precipitation_ `tp`, the original
ECMWF data resets the values at the start of the UTC day on all latitudes already.

For instantaneous variables, e.g. the _2 meter temperature_ `t2m`, the operation applied is
the Xarray `.resample("D").mean()` method.
For accumulated variables the values are the total accumulation for the day.
