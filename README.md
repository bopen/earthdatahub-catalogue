# Earth Data Hub Catalogue

Catalogue for the [Earth Data Hub][1] project within the EU [Destin Earth][2] initiative. This catalogue is aimed at producing a [STAC API][3] implementation and defines a simplified version of the [STAC][4] specification as a schema for its objects, written as [JSONSchema][5] in the `schema/` folder.

## Assumptions

The data in this repository needs to respect the following assumptions:

- The catalogue files and folders must be located inside the `catalogue/` folder;
- Each folder in `catalogue/` represents a *collection* and each of its folders represents a *dataset* (corresponding to a STAC item) associated to that collection;
- Collections and datasets are univoquely identified by their folder names;
- Collections and datasets metadata are written as YAML files (respectively `__collection__.yaml` and `__item__.yaml`) inside their relative folders and must respect the simplified version of the STAC specification defined in the `schema/` folder;
- Thumbnail images and description files can be written as URL inside the YAML files or added to the collections and datasets folders;
- The schemas for the collections and datasets files are defined inside the  `schema/` folder as [JSONSchema][5] files;
- Additional files and folders used by external tools can be contained inside collections and datasets folders.

## STAC Extensions

The STAC extensions adopted in the catalogue are listed below:

- [Earth Data Hub](https://raw.githubusercontent.com/bopen/earthdatahub-catalogue/main/schema/extensions/earthdatahub.json) (`schema/extensions/earthdatahub.json`)
- [Dublin Core](https://raw.githubusercontent.com/bopen/earthdatahub-catalogue/main/schema/extensions/dublincore.json) (`schema/extensions/dublincore.json`)
- [Datacube](https://github.com/stac-extensions/datacube)
- [xarray Assets](https://github.com/stac-extensions/xarray-assets)

[1]: https://earthdatahub.com/
[2]: https://destination-earth.eu/
[3]: https://github.com/radiantearth/stac-api-spec
[4]: https://github.com/radiantearth/stac-spec
[5]: https://json-schema.org/
