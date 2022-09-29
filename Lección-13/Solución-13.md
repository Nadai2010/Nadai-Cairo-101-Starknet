## Lección 13 - Privacidad en StarkNet

[Código](https://github.com/starknet-edu/starknet-cairo-101/blob/main/contracts/ex13.cairo)

[Voyager](https://goerli.voyager.online/contract/0x2bae9190076c4252289b8a8671277cef57318192cff20c736808b0c71095895)

Función `claim_points()`

![image](ejercicio13-0.png "ejercicio13-0")

Nos asiganmos un slot.

![image](ejercicio13-1.png "ejercicio13-1")

Nos fijamos en el valor del slot.

![image](ejercicio13-2.png "ejercicio13-2")

Revisamos la [transacción](https://goerli.voyager.online/tx/0x6c2eafb7708f38a81c5a772d8d76ebf5a28fd27939df273a6650147e662c838) donde se creó el contrato y DONDE ENCONTRAREMOS los datos. Si vemos la transacción se ve el array por lo tanto los valores secretos. Al igual que los ejercicios anteriores al array lo iteran de izquierda a derecha. Por lo tanto el último elemento del array se guarda en la posición 0.
Haciendo la siguiente resta podemos obtener el valor secreto:

valor secreto = len_array - user_slot 
valor secreto = 106 - 55 = posicion 51

Definimos 106 como len_array dado que son los totales creados al hacer el deploy del Smart.

Tx cuando se creo el contrato 

![image](ejercicio13-5.png "ejercicio13-5")

Tenemos que revisar *CONSTRUCTOR CALLDATA*

![image](ejercicio13-6.png "ejercicio13-6")

Buscamos la posicion y guardamos el valor.

![image](ejercicio13-3.png "ejercicio13-3")

De esta manera ya podemos obtener los puntos.

![image](ejercicio13-4.png "ejercicio13-4")

