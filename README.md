# How the map was created

* Created orthographic.svg using the following steps:

```
$ wget https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/10m/cultural/ne_10m_admin_0_countries.zip
$ unzip ne_10m_admin_0_countries.zip
$ cpan Geo::ShapeFile
$ cpan SVG
$ for type in orthographic ; do ./perlshaper.pl ne_10m_admin_0_countries.shp -centre -171.700833,63.776111 -type $type -res 0.0001 -psize 0.04 -nolines -seacol white -bordcol black -landcol "#FF0000" > ${type}.svg;  done
```

* Opened orthographic.svg in Adobe Illustrator, saved as Illustrator file

* Opened Illustrator file in Adobe Photoshop

* Edited using Photoshop
  * Color schemes and language boundary data from:
  	* Krauss, Michael, Gary Holton, Jim Kerr, and Colin T. West. 2011. [Indigenous Peoples and Languages of Alaska.](https://www.uaf.edu/anla/map) Fairbanks and Anchorage: Alaska Native Language Center and UAA Institute of Social and Economic Research.
    * [Noahedits.](https://commons.wikimedia.org/wiki/User:Noahedits) [Map of the Chukotko-Kamchatkan languages](https://en.wikipedia.org/wiki/Chukotko-Kamchatkan_languages#/media/File:Chukotko-Kamchatkan_map.svg)
    * Krupnik, Igor and Chlenov, Michael. 2013. [Yupik Transitions: Change and Survival at Bering Strait, 1900-1960.](https://press.uchicago.edu/ucp/books/book/distributed/Y/bo16803074.html) University of Alaska Press.
    