##Charts Location
On lysmarine, charts are stored in `/srv/charts/`

For convenience a link have been added in the `/home/user/charts` directory. So users can manage charts without root privileges. 

### The criteria that lead to the use of /srv/charts
 - A location that is app neutral (so app depend on another app location/existence)
 - A location that is user neutral (as many users will need to access them: User, signalk, www-data, root )
 - A location compliant to the FHS
 - A location that is historically used to store large datasets of dynamic content.
 - A location where human users could manage the dataset without root access.

## Formats and Services 
Signalk read any mbtiles format found in the folder to serve them via it's API. 
   
Opencpn can read both mbtiles and a large variety of vector charts format from the folder. 

__Note that when charts are added or removed, opencpn cache must be rebuild manually__

See the [list of supported charts](https://opencpn.org/wiki/dokuwiki/doku.php?id=opencpn:opencpn_user_manual:charts:chart_formats) by opencpn


## Side notes
* Opencpn uses zooms between 1:800 to 1:12300000 this is equivalent to z5 @ z20 mbtiles format.
* opencpn 5.0.0 have added the support for tiling formats.
But due to the low capacity of the raspberry. Sadly, It often crash .


  