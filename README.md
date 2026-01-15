1. Šī ir programma, kas plāno maršrutus kravas automašīnām Eiropā un salīdzina variantus:
	Tikai pa sauszemi;
	Sauszeme + prāmis.
Šī programma aprēķina ETA, provizoriskās izmaksas un iekļauj dažādus faktorus, kā aizliegtās zonas (zonas kurās pastāv iespējamība traucējumiem)

2. Šo programmu var palaist, double click failu, vai arī caur visual studio code, kur to var atvērt ar 'run -> start debugging/run without debugging'

3.	Frontend:
		HTML + CSS + Vanilla JavaScript
		Leaflet (kartei un slāņiem)
	Kartes un maršruti:
		OpenStreetMap tiles (kartes pamatne)
		OSM Nominatim - vietu meklēšana/ģeokodēšana
		OSRM (router.project-osrm.org) - ceļa maršruti, atgriež distanci/ilgumu
	Prāmji (modelēti)
		Ostas ir definētas lokāli masīvā "PORTS"
		Prāmju savienojumi definēti "FERRY_EDGES"
		Maršruta atrašana prāmju tīklā tiek veikta ar Dijkstra algoritmu
		Jūras attālums tiek rēķināts ar Haversine
	Ierobežojumi (modelēti)
		"Hard constraints" zonas ir definētas "HARD_CONSTRAINTS"
