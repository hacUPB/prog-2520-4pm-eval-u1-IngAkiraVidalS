## ejercicio lapices 

### análisis

Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.


|variables de entrada|descripcion|
|--------------------|-----------|
|cant_lapices | cuantos lápices se compra |

|variables de salida | descripcion |
|--------------------|-------------|
|precio | valos que hay que pagar |

|variables intermedias | descripcion |
|----------------------|-------------|
|valor_unitario | usada dentro del codigo |

|constantes | descripcion |
|----------------------|--------------|
| 1000 | cantidad límite de lapices   |
|$85, $90 | valor individual según la cantidad |

```
Inicio
leer cant_lapices
Si cant_lapices >= 1000
    valor_unidad = 85
ai no 
    valor_unidad = 90
Fin si 
precio = valor unidad * cant_lapices
escribir "valor total: ", precio
Fin

```

## diagrama de flujo 

![actividad1](diagralgolapices.png)


## ejercicio 2

Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

## análisis

|variables de entrada|descripcion|
|--------------------|-----------|
|precio_prenda_1 | costo parcial de las prendas |
|precio_prenda_2 | costo parcial de las prendas |
|precio_prenda_3 | costo parcial de las prendas |


|variables de salida | descripcion |
|--------------------|-------------|
|precio_final | valor que hay que pagar |
| descuento   | valor del descuento |


|constantes | descripcion |
|----------------------|--------------|
| 250000 | valor a partir del cual se da el descuento   |
|15%, %8 | descuentos |

## pseudocodigo 

```
Inicio
Leer valor_compra
Si valor_compra > 250000
    descuento = valor_compra * 0.15
Si no 
    descuento = valor_compra * 0.08
Fin Si
precio_final = valor_compra - desceunto
Mostrar "valor a pagar: $", precio final
Fin 
```

## ejercicio 3 

El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

### pseudocodigo

```
Inicio
Leer alumnos
Si alumnos >= 100
    costo_alumno = 65
si no
    Si alumnos >= 50
        costo_alumno = 70
    Si no
        costo_alumno = 95
    Fin si
Fin si

```




## ejercicio inventado 
Una tienda de ropa tiene la siguiente promocion: por la compra de 3 productos, la prenda de menor valor, tiene un 70% de descuento.
CALCULAR CUAL FUE EL DESCUENTO APLICADO Y CUANTO TIENE QUE PAGAR LA PERSONA.

## análisis

|variables de entrada|descripcion|
|--------------------|-----------|
|precio_prenda | costo parcial de cada prendas |

|variables de salida | descripcion |
|--------------------|-------------|
|precio_final | valor que hay que pagar |
| descuento   | valor del descuento |

|constantes | descripcion |
|----------------------|--------------|
| 3 | valor a partir del cual se da el descuento   |
|70% | descuentos |

### pseudocodigo 

```
Inicio 
    Digite "ingrese precio_prenda_1:"
    leer precio1
    digite "ingrese precio_prenda_2:"
    leer precio2
    digite "ingrese precio_prenda_3:"
    leer precio 3

    menor ← precio1
    Si precio2 < menor Entonces
        menor ← precio2
    FinSi
    Si precio3 < menor Entonces
        menor ← precio3
    FinSi

    descuento ← menor * 0.70
    total ← (precio1 + precio2 + precio3) - descuento

    Escribir "El descuento aplicado es: ", descuento
    Escribir "El total a pagar es: ", total
Fin
```

![ejercicioinventado](ejercicioprendas.png)
