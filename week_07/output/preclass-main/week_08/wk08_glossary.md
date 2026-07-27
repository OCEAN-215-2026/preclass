# Week 8 glossary

## Online resources

Documentation for cartopy can be found at [https://scitools.org.uk/cartopy/docs/latest/reference/index.html](https://scitools.org.uk/cartopy/docs/latest/reference/index.html). In particular, the collection of map projections supported by cartopy can be found at [https://scitools.org.uk/cartopy/docs/latest/reference/projections.html](https://scitools.org.uk/cartopy/docs/latest/reference/projections.html).

ArcGIS provides some useful information about the map projection *it* supports. Their landing page is at [https://pro.arcgis.com/en/pro-app/latest/help/mapping/properties/list-of-supported-map-projections.htm](https://pro.arcgis.com/en/pro-app/latest/help/mapping/properties/list-of-supported-map-projections.htm). Note that the name of the same projection may differ between cartopy and ArcGIS.

The cartopy geographical features comes from Natural Earth. You can find more information and browse available features at [https://www.naturalearthdata.com/features/](https://www.naturalearthdata.com/features/)

## Cartopy

### Cartopy submodules

+ `cartopy.crs` (`ccrs`): submodule providing map projection utilities
+ `cartopy.features` (`cfeature`): submodule providing geographical features utilities
+ `cartopy.mpl.gridliner`: submodule providing gridline customizations

### Cartopy functions

+ `ccrs.PlateCarree()`, `ccrs.Robinson()`, etc.: map projections. To be used as `projection` argument in `<Figure>.add_subplot()` and `transform` argument in `<GeoAxes>.pcolormesh()`, etc.

### Cartopy GeoAxes methods

_Note_: a GeoAxes instance is created by `<Figure>.add_subplot()` when the `projection` argument uses a cartopy map projection.

+ `<GeoAxes>.coastline()`: add coastline to the GeoAxes instance
+ `<GeoAxes>.add_feature()`: add a geographical feature to the GeoAxes instance
+ `<GeoAxes>.gridlines()`: adding gridlines to the GeoAxes instance
+ `<GeoAxes>.set_extent()`: limit the geographical extent of the plot

### Cartopy attributes

+ `cfeatures.BORDERS`, `cfeatures.STATES`, `cfeature.COASTLINE`, `cfeature.LAKES`, `cfeatures.LAND`, `cfeature.OCEAN`, `cfature.RIVERS`: built-in geographical features that can be added to a GeoAxes instance.

+ `cartopy.mpl.gridliner.LONGITUDE_FORMATTER` and `cartopy.mpl.gridliner.LATITUDE_FORMATTER`: formatter for longitude and latitude display

### Cartopy gridliner attributes

_Note_: the object returned by `<GeoAxes>.gridlines()` is a Gridliner instance

+ `<Gridliner>.xlocator` and `<Gridliner>.ylocator`: set the locations of gridlines
+ `<Gridliner>.xformatter` and `<Gridliner>.xformatter`: set the formatting of the gridline labels
+ `<Gridliner>.xlabel_style` and `<Gridliner>.xlabel_style`: set the gridline labels styles

## matplotlib functions

+ `matploltib.ticker.FixedLocator()`: generate tick locations based on the input array