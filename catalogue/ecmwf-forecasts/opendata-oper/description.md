The high-resolution forecast is a single forecast included in the ECMWF medium-range forecasts. The forecast has a horizontal resolution of around 9 km and provides a description of a possible evolution of the weather out to 10 days ahead.

How to access:

```python

    import xarray as xr
    
    ds = xr.open_dataset(
        "s3://hedp/ecmwf-forecasts/opendata-oper-20231016T00.zarr",
        engine="zarr",
        chunks={},
    )
    ```