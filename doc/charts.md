#Location

Charts must be stored in `/srv/charts/`

For convenience a link have been added in the `/home/pi/charts` directory.



#Users
The applications that directly read charts are signalk and opencpn.

Tuktuk for it's part is retrieving the charts from the signalk server.   


#Formats

### Tuktuk & signalk
Only support tiling formats (mbtiles).

Opencpn uses zooms between 1:800 to 1:12300000 Witch is equivalent to z5 @ z20 in tuktuk.





### Opencpn

Opencpn support a wild range of charts.
You can take a look at the list on opencpn website `https://opencpn.org/wiki/dokuwiki/doku.php?id=opencpn:opencpn_user_manual:charts:chart_formats`

_NOTE: opencpn 5.0.0 have added the support for tiling formats.
But due to the low capacity of the raspberry. Sadly, It often crash ._
