## Lección 10 - Composability

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex10.cairo)

[Voyager](https://goerli.voyager.online/contract/0x8415762f4b0b0f44e42ac1d103ac93c3ea94450a15bb65b99bbcc816a9388)

En este ejercicio el valor secreto está en otro contrato. Vamos a llamarlo contrato B `ex10b.cairo`. El contrato A es donde tenemos que ingresar el valor secreto.

Función `claim_points()`

![image](ejercicio10-0.png "ejercicio10-0")

Primero debemos encontrar el address del contrato B. Se obtiene del contrato A llamando a la función `ex10b_address()` .

![image](ejercicio10-1.png "ejercicio10-1")

Buscamos en el [contrato B](https://goerli.voyager.online/contract/0x070e27636818c69fb3e17451bd077c971524cb2a5a38e79b2d8a09034b7e1a9c) en Voyager. Llamamos a la función `secret_value()` y obtenemos el valor secreto.

![image](ejercicio10-2.png "ejercicio10-2")

Vamos al contrato A. Ingresamos el valor secreto y de esta manera ya podemos obtener los puntos. 

![image](ejercicio10-3.png "ejercicio10-3")