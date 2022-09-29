## Lección 11 - Importando funciones
[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex11.cairo)

[Voyager](https://goerli.voyager.online/contract/0xab5577b9be8948d89dbdba63370a3de92e72a23c4cacaea38b3a74eec3a872)

Debemos chequear los import para saber donde se encuentra la función `validate_answers()` y ver su lógica.

Función `claim_points()`

![image](ejercicio11-0.png "ejercicio11-0")

Función `secret_value()`

![image](ejercicio11-4.png "ejercicio11-4")

Función `validate_answers()`

![image](ejercicio11-3.png "ejercicio11-3")

Llamamos a la función `secret_value()` y ontenemos el valor secreto.

![image](ejercicio11-1.png "ejercicio11-1")

Le restamos `42069`, ya que dentro de la función `secret_value()` suma ese valor y de esta manera ya puedo obtener los puntos.

![image](ejercicio11-2.png "ejercicio11-2")
