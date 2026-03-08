This dataset features a selection of variables derived from the second-generation Climate Adaptation Digital Twin of the Destination Earth initiative. The subset includes single-level or surface variables from the ICON model's control simulation. Covering the 1990–2000 period with an hourly temporal resolution, the data has been regridded from its original HEALPix H128 grid to a regular latitude-longitude grid with a ~0.35° spatial resolution.

To support fast regional assessments and time-series analysis, the data is distributed in a compressed Zarr v3 format with underlying optimised chunking.

Accessing this dataset requires a Zarr v3-compatible library (e.g., zarr-python >= 3.x). Python users can upgrade via `pip install "zarr>3"`. Access is restricted to upgraded users only.
