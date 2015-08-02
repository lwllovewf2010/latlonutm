# Latitude, Longitude to UTM Converter

This module converts between latitude longitude and UTM coordinates.

Geographic coordinates are entered and displayed in degrees.

Negative numbers indicate West longitudes and South latitudes.

UTM coordinates are entered and displayed in meters.

The ellipsoid model used for computations is WGS84.

Usage:

```python
import latlonutm as ll
lat = 38.889360
lon = -77.034355
print 'lat = {}, lon = {}'.format(lat, lon)
[[northing, easting], zone, hemi] = lat_lon_to_utm(lat, lon)
print 'northing = {}, easting = {}, zone = {}, hemisphere = {}'.format(northing, easting, zone, hemi)
[lat, lon] = utm_to_lat_lon(northing, easting, zone, hemi)
print 'lat = {}, lon = {}'.format(lat, lon)
```

Converted from javascript found on this page:
http://home.hiwaay.net/~taylorc/toolbox/geography/geoutm.html
