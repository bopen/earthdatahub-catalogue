The daily GLORYS12V1 product is the CMEMS global ocean eddy-resolving
(1/12° horizontal resolution, 50 vertical levels) reanalysis covering the
altimetry (1993 onward).

How to access:


```python

import xarray as xr

ds = xr.open_dataset(
    "s3://cmems-reanalysis/cmems_mod_glo_phy_my_0.083_P1D-m.zarr",
    engine="zarr",
    chunks={},
    storate_options={"enpoint_url": "https://s3.gra.perf.cloud.ovh.net"}
)
```