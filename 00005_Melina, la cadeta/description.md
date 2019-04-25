**Melina** es una cadeta que trabaja para los otros clientes de la remisería. Parecido al caso de **Lucía**, en cada momento trabaja para un cliente - se debe informar para quién. 

Por ser cadeta, la agencia le otorga un descuento especial: el precio por kilómetro pactado con Melina es 3 pesos menos que lo que se le cobraría a su cliente. Si por ejemplo trabaja Ludmila, su precio por kilómetro será de 15; si en cambio trabaja para Teresa, la agencia le cobrará 19 por kilómetro.

Veamos cómo quedaría esto en un REPL de Wollok:

```wollok
melina.estaTrabajandoPara(ludmila)
melina.precioPactadoPorKm() // => 15

melina.estaTrabajandoPara(teresa)
melina.precioPactadoPorKm() // => 19
```

> Agregá al objeto `melina`, con los mensajes necesarios para que sea polimórfico con las demás clientas.
