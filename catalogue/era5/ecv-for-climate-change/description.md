The Essential Climate Variables for assessment of climate variability from 1979 to present dataset contains 
a selection of climatologies, monthly anomalies and monthly mean fields of 
Essential Climate Variables (ECVs) suitable for monitoring and assessment of climate variability and change. 

Selection criteria are based on accuracy and temporal consistency on monthly to decadal time scales. 
The ECV data products in this set have been estimated from climate reanalyses ERA-Interim and ERA5, 
and, depending on the source, may have been adjusted to account for biases and other known deficiencies. 

Data sources and adjustment methods used are described in the Product User Guide, as are various particulars
such as the baseline periods used to calculate monthly climatologies and the corresponding anomalies. 

The statistics provided are monthly average fields, climatologies and anomalies, 
as well as 12-month running mean anomalies.

Climatologies and anomalies are calculated with respect to two reference periods

1. 1981-2010 (ERA5 and ERA-Int) and 
2. 1991-2020 (ERA5 only).

The C3S monthly climate bulletin (https://climate.copernicus.eu/climate-bulletins) provides
an assessment of the monthly state of the climate with an emphasis on the European geographical domain. 
This data record is used as the basis for these monthly bulletins.

How to access:

```python

import xarray as xr

ds = xr.open_dataset(
    "s3://hedp/era5/ecv-for-climate-change-1979-2023.zarr",
    engine="zarr",
    chunks={},
    storate_options={"enpoint_url": "https://s3.gra.perf.cloud.ovh.net"}
)
```