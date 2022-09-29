## Lección 3 - Leyendo y escribiendo variables de almacenamiento 

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex03.cairo)

[Voyager](https://goerli.voyager.online/contract/0x79275e734d50d7122ef37bb939220a44d0b1ad5d8e92be9cdb043d85ec85e24)

En este ejercicio debemos modificar la variable `user_counters_storage` con las funciones `incremen_counter()`(suma 2) y `decrement_counter()`(resta 1) para que sea igual a 7 y poder obtener los puntos.

Función `claim_points()`

![image](ejercicio3-0.png "ejercicio3-0")

Como vemos la variable `user_counters_storage` tiene el valor de 0.

![image](ejercicio3-1.png "ejercicio3-1")

Llamamos a la función 4 veces para que `user_counters_storage()` tenga el valor de 8.

![image](ejercicio3-2.png "ejercicio3-2")

Llamamos a la función 1 vez para que `user_counters_storage()` tenga el valor de 7.

![image](ejercicio3-3.png "ejercicio3-3")

De esta manera ya podemos obtener los puntos.

![image](ejercicio3-4.png "ejercicio3-4")
