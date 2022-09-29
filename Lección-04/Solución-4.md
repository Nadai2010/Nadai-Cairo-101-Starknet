## Lección 4 - Mappings 

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex04.cairo)

[Voyager](https://goerli.voyager.online/contract/0x2cca27cae57e70721d0869327cee5cb58098af4c74c7d046ce69485cd061df1)

En este ejercicio debemos hacer que el valor `values_mapped_storage` sea igual a `expected_value + 32`.

Función `claim_points()`

![image](ejercicio4-0.png "ejercicio4-0")

Ahora iremos a `write smart` y nos asignamos un slot.

![image](ejercicio4-1.png "ejercicio4-1")

Copiamos el valor del slot y vamos a `read smart`.

![image](ejercicio4-2.png "ejercicio4-2")

Llamó a la función `values_mapped()` y me guardo el valor.

![image](ejercicio4-3.png "ejercicio4-3")

Ingreso el valor obtenido en la función anterior pero le restamos 32, ya que dentro de la función `claim_points()` le suman este valor. De esta manera ya podemos obtener los puntos.

![image](ejercicio4-4.png "ejercicio4-4")