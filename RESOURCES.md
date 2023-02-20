# Resources

## Pug

- [Tutorial Video from FreeCodeCamp](https://www.youtube.com/watch?v=kt3cEjjkCZA&ab_channel=freeCodeCamp.org)
- [Guide to restructuring a project with pug from FreeCodeCamp](https://www.freecodecamp.org/news/make-multipage-html-development-suck-less-with-pug-fb23bc8e7874/)
- [Pug cheatsheet](https://devhints.io/pug)

## Bootstrap

- [Bootstrap Cheatsheet](https://bootstrap-cheatsheet.themeselection.com/)

## Geoprocessing

You can install the OSGeoWeb shell when you install QGIS. This gives you access to many geoprocessing tools from the command line without requiring additional installs or PATH configuration.

[Viewing information from a geodatabase from the command line with ogrinfo](https://gdal.org/programs/ogrinfo#)
```bash
ogrinfo EJSCREEN_2022_with_AS_CNMI_GU_VI.gdb.zip EJSCREEN_Full_with_AS_CNMI_GU_VI -so -where "ST_ABBREV='ME'"
```

[Converting file formats with `ogr2ogr` from GDAL](https://gdal.org/programs/ogr2ogr.html#ogr2ogr)
```bash
ogr2ogr -f geojson ejscreen-2022-me.geojson EJSCREEN_2022_with_AS_CNMI_GU_VI.gdb.zip EJSCREEN_Full_with_AS_CNMI_GU_VI -where "ST_ABBREV='ME'" -t_srs EPSG:4326
```