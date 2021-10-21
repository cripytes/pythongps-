import android droid = android.Android () droid.startLocating () print "leyendo GPS ..." event = droid.eventWaitFor ('location', 10000) .result if event ['name'] == "location": try : lat = str (evento ['datos'] ['gps'] ['latitud']) lng = str (evento ['datos'] ['gps'] ['longitud']) excepto KeyError: lat = str ( evento ['datos'] ['red'] ['latitud']) lng = str (evento ['datos'] ['red'] ['longitud']) latlng = 'lat:' + lat + 'lng: '+ lng imprimir latlng droid.stopLocating ()  

droid.startLocating () 
event = droid.eventWaitFor ('ubicación', 10000) .result 
lat = str (evento ['datos'] ['gps'] ['latitud']) lng = str (evento ['datos'] ['gps'] ['longitud'])

droid.stopLocating ()
dirección = droid.geocode (lat, lng) .result  
print  ("resul")
 

