Agregar al modelo un objeto que represente a la oficina desde donde la cooperativa despacha viajes.

En este modelo simplificado, cuando la oficina recibe un viaje, hay dos choferes que pueden tomarlo: uno que tiene prioridad (al que llamaremos _primera opción_ o _primer chofer_) y otro que es la _segunda opción_ (o _segundo chofer_).

El objeto `oficina` debe entender estos mensajes:

- `asignarChoferes(chofer1, chofer2)`: establece los choferes de primera y de segunda opción.
- `choferPrimeraOpcion()`: devuelve el chofer de primera opción.
- `choferSegundaOpcion()`: devuelve el chofer de segunda opción.
- `cambiarPrimerChoferPor(chofer)`: cambia el chofer de primera opción por el que se indica.
- `cambiarSegundoChoferPor(chofer)`: cambia el chofer de segunda opción por el que se indica.
- `intercambiarChoferes()`: intercambia los choferes de primera y segunda opción. O sea, el que era primera pasa a segunda, y viceversa.
- `choferElegidoParaViaje(cliente, kms)`: devuelve el chofer que corresponde asignar a un viaje, dados el cliente y la cantidad de kilómetros. 
  El criterio es el siguiente: si para ese viaje, el precio del segundo chofer es menor al del primero con una diferencia de más de 30 pesos, entonces se elige el segundo chofer; si no, se elige el primero.

Supongamos que en un momento dado el chofer de primera opción es Roxana, y el de segunda opción es Juana. En este caso

- para un viaje de 10 kilómetros para Ana María, el chofer elegido es Juana, porque su precio de 200 pesos, es menor al de Roxana (300 pesos), y la diferencia es de más de 30 pesos.
- si el viaje es para Teresa, entonces Roxana ofrece 220 pesos y Juana 200. El precio de Juana es menor, pero la diferencia no llega a 30 pesos. Por lo tanto, el chofer elegido es Roxana.
- si el viaje es de 4 kilómetros para Teresa, entonces Roxana cobra 88 pesos y Juana 100. El precio de Roxana es menor, por lo tanto ella es la elegida.  

> Programá a la `oficina` con todos los mensajes necesarios.