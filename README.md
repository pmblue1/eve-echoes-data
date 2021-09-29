# eve-echoes-data
A set of files with eve echoes informational files.

Files can be found at: https://auxilus.xyz/eve-echoes-data/files


__File List__

planets.sqlite3 - sqlite database with tables of information regarding the map and its organization. Also contains PI info. Was generated a long time ago.

eve_data.sqlite3 - sqlite database with tables of information regarding various things, including some reprocessing and blueprints. Was generated a long time ago.

database substitutes - folder with alternative format versions of the sqlite databases.
   - planets.sqlite3.json - file containing all planets.sqlite3 tables in json format.
   - eve_data.sqlite3.json - file containing all eve_data.sqlite3 tables in json format.
   - planets.constellations.csv - csv version of constellations table from planets.sqlite3
   - planets.planets.csv - csv version of planets table from planets.sqlite3
   - planets.regions.csv - csv version of regions table from planets.sqlite3
   - planets.systems.csv - csv version of systems table from planets.sqlite3
   - eve_data.blueprints.csv - csv version of blueprints table from eve_data.sqlite3
   - eve_data.market.csv - csv version of market table from eve_data.sqlite3. Not live, is useless here.
   - eve_data.reprocess.csv - csv version of reprocess table from eve_data.sqlite3

all_items_info.json - file with extensive information on game items, including ships, largely parsed and translated.

attributes.json - file with attribute data. attribute names correlate to the names of attributes in all_items_info.json file.

effects.json - file with effects data. effect names correlate to the names of effects in all_items_info.json file.

ships.json - much like all_items_info.json, but only containing items whose category was ship.

systems_r.json - basic system data with name translations

constellations_r.json - basic constellation data with name translations

regions_r.json - basic region data with name translations

stargates.json - has data on all stargates, including cords. This allows you to calculate distances between gates.

new_stations.json - data on stations, including detailed translations

planet_exploit_resource.json - data on planets and their resources


__Icon API__

Want to implement item icons into your application? Whether its a Discord bot, website, or something else, I have you covered! 

Endpoint: https://auxilus.xyz/echoes/api/icon/<item_id>

If you replace the <item_id> placeholder, an icon for the item of the given id will be returned. If the item is not found, it will return a 404 error. If you want to have the endpoint redirect you to another image url in the case of there being no icon found for that item, you can use the blank_image argument, and provide that images url. Some examples of proper usage of this endpoint:
- https://auxilus.xyz/echoes/api/icon/10500000202?blank_image=https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Icon-round-Question_mark.svg/1200px-Icon-round-Question_mark.svg.png
- https://auxilus.xyz/echoes/api/icon/10100000109

This endpoint has NO RATE LIMIT! Go crazy.



__Examples__

documented_ship_item.json - this example file includes a sample ship item, in this case a Moa Guardian. It has notes next to many of the values to help explain their meaning.
