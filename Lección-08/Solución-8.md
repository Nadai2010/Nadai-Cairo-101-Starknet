## Lección 8 - Recursiones nivel 1

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex08.cairo)

[Voyager](https://goerli.voyager.online/contract/0x15fa754c386aed6f0472674559b75358cde49db8b2aba8da31697c62001146c)

En este caso `user_values_storage(user_address, 10)` debe tener el valor `10` .

Función `claim_points()`

![image](assets/ejercicio8-0.png "ejercicio8-0")

Vamos a revisar de que manera escribe la función `set_user_values()`.
Utiliza recursión para escribir sobre `user_values_storage`.
El `user_address` siempre es el mismo. El slot inicia en 0, el max es len del array.
Empieza a escribir los valores del array de izquierda a derecha en `user_values_storage`.
En este caso no importa los valores que ingrese en las posiciones 0-9 contando desde la izquierda, lo unico que nos interesa es que en la posicion 10 contando de la izquierda tenga el valor 10.

![image]/ejercicio8-3.png "ejercicio8-3")

Para el array `[10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]` quedaría de la siguiente manera.

![image](ejercicio8-4.png "ejercicio8-4")

Llamamos a la función `set_user_values()` con esta solución.

![image](ejercicio8-1.png "ejercicio8-1")

De esta manera ya podemos obtener los puntos.

![image](ejercicio8-2.png "ejercicio8-2")

