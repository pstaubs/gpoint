# gpoint
PHP 7.0-compatible fork of the old gPoint PHP class dating from 2008, written by Brenor Brophy.

Original documentation available at: http://safe.phpclasses.net/browse/view/html/file/14315/name/readme.htm

> # About the gPoint Class

> A gPoint object is a point on the Earth's surface. Its location is defined by a Longitude and a Latitude coordinate. These coordinates define a point on the surface of a sphere. However, computer screens like paper are flat surfaces and so we face a problem if we wish to represent data whose location is defined by Lat/Longs onto a such a surface. For example, you have an array of Lat/Long points that you want to plot on an image of a map. So how do you calculate the X/Y pixel on the image to plot your point? What you need is a transformation from a Lat/Long coordinate to an X/Y coordinate. This is called a map projection. There are many different types of projection. This class provides functions for working with two of the most useful; Universal Transverse Mercator (UTM) and Lambert Conformal Conic. The class also supports a variant of UTM, that I call Local Transverse Mercator. It is very useful when you just need to plot a few points on an arbitrary image that covers a modest amount of the Earth (10x10 degrees) and you don't have to deal with UTM zones.

> At a high level converting a Long/Lat coordinate in degrees thru a projection will return an Easting/Northing coordinate in meters. That is meters measured on the 'flat' ground that you can convert to pixels and plot on an image. Broadly speaking Transverse Mercator (and UTM) is useful for modest sized areas of about 10x10degrees or less. Lambert is useful for large areas in the mid latitudes (Like the whole USA or Europe for example). Neither projection works well for areas near the poles.
