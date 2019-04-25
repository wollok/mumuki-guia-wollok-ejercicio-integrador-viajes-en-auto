**Lucía** es una chofer que hace reemplazos, o sea, cubre los turnos que las otras remiseras se tienen que tomar por alguna razón.

Lucía cobra lo mismo que el chofer al que está reemplazando, y para que esto ocurra es necesario que esto se informe.

Veamos un ejemplo:

```wollok
lucia.estaReemplazandoA(roxana)
lucia.precioViaje(ludmila, 10) // => 180

lucia.estaReemplazandoA(gabriela)
lucia.precioViaje(ludmila, 10) // => 216
```

> Programá el objeto `lucia` para que se comporte como se ve en el ejemplo.