## Lección 5 - Visibilidad de variables <a name="ej5"></a>

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex05.cairo)

[Voyager](https://goerli.voyager.online/contract/0x399a3fdd57cad7ed2193bdbb00d84553cd449abbdfb62ccd4119eae96f827ad)

En este ejercicio debemos hacer que el valor `values_mapped_secret_storage` sea igual a `expected_value + 23` .

Función `claim_points()`

![image](ejercicio5-0.png "ejercicio5-0")

Ahora iremos a `write smart` y nos asignamos un slot.

![image](ejercicio5-1.png "ejercicio5-1")

Nos fijamos en el valor del slot.

![image](ejercicio5-2.png "ejercicio5-2")

Llamamos a la función `users_values()` y nos guardamos el valor.

![image](ejercicio5-3.png "ejercicio5-3")

Como verán es 0. Debemos llamar a la función `copy_secret_value_yo_readable_mapping()` para que modifique el valor.

![image](ejercicio5-4.png "ejercicio5-4")

Llamamos a la función `users_values()` y guardamos el valor.

![image](ejercicio5-5.png "ejercicio5-5")

Ingresamos el valor obtenido en la función anterior pero le restamos 23, ya que dentro de la función `claim_points()` le suman este valor. De esta manera ya puedo obtener los puntos.

![image](ejercicio5-6.png "ejercicio5-6")

