## Lección 6 - Visibilidad de funciones

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex06.cairo)

[Voyager](https://goerli.voyager.online/contract/0x718ece7af4fb1d9c82f78b7a356910d8c2a8d47d4ac357db27e2c34c2424582)

Debemos averiguar el valor secreto en `values_mapped_secret_storage`.

Función `claim_points()`

![image](ejercicio6-0.png "ejercicio6-0")

Nos asignamos un slot.

![image](ejercicio6-1.png "ejercicio6-1")

![image](ejercicio6-2.png "ejercicio6-2")

Debemos llamar a función `external_handler_for_internal_function()` para que modifique el valor de `values_mapped_secret_storage`.

![image](ejercicio6-3.png "ejercicio6-3")

Llamamos a la función `user_values()` y guardamos el valor.

![image](ejercicio6-4.png "ejercicio6-4")

Ingresamos el valor obtenido en la función anterior. De esta manera ya podemos obtener los puntos.

![image](ejercicio6-5.png "ejercicio6-5")

