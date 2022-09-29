## Lección 9 - Recursiones nivel 2

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex09.cairo)

[Voyager](https://goerli.voyager.online/contract/0x2b9fcc1cfcb1ddf4663c8e7ac48fc87f84c91a8c2b99414c646900bf7ef5549)

Hay que pasar un array de 4 elementos donde la suma de estos 4 sea igual a 50, pero mientras se hace la suma se tiene que cumplir una condición.
Como el ejercicio anterior empieza a iterar de izquierda a derecha.
La condición que se tiene que cumplir es que la `suma temporal * 2` tiene que ser menor o igual que la `suma temporal + el elemento actual` .

Función `claim_points()`

![image](ejercicio9-0.png "ejercicio9-0")

Función `get_sum_internal()`

![image](ejercicio9-3.png "ejercicio9-3")

Para el array `[33, 12, 4, 1]` quedaría de la siguiente manera.

![image](ejercicio9-2.png "ejercicio9-2")

De esta manera ya podemos obtener los puntos con la solución anterior.

![image](ejercicio9-1.png "ejercicio9-1")

