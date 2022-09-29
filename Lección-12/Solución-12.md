## Lección 12 - Eventos

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex12.cairo)

[Voyager](https://goerli.voyager.online/contract/0x24d15e02ddaa19d7ecd77204d35ed9bfff00a0cabc62eb3da5ba7680e44baf9)

Al llamar la función `assign_user_slot()` se emite un evento donde está el valor secreto.
Función `claim_points()`

![image](ejercicio12-0.png "ejercicio12-0")

Llamamos a la función `assign_user_slot()` y nos quedamos con el tx de la transacción para poder revisar los eventos.

![image](ejercicio12-3.png "ejercicio12-3")

![image](ejercicio12-1.png "ejercicio12-1")

Le restamos 32, ya que cuando se emitió el evento le sumaron ese valor.

![image](ejercicio12-2.png "ejercicio12-2")
