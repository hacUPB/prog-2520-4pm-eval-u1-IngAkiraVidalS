## bucles 
### problemas propuestos

Un profesor tiene un salario inicial de $1500, y recibe un incremento de 10 % anual durante 6 años. ¿Cuál es su salario al cabo de 6 
años? ¿Qué salario ha recibido en cada uno de los 6 años? Realice el algoritmo y represente la solución mediante el diagrama de flujo, el 
pseudocódigo y el diagrama N/S, utilizando el ciclo apropiado

## pseudocódigo

```
Inicio
año = 1
salario = 1500
total = 0
mientras año <= 6:
    anual = salario * 1.1
    total = total + anual
    salario = anual
    año = año + 1
    Mostrar anual
Fin mientras 
Mostrar total
Fin 
```
## diagrama de flujo 
![bucles](salario.png)


## ejercicio 2

Se requiere un algoritmo para determinar, de N cantidades, cuántas 
son cero, cuántas son menores a cero, y cuántas son mayores a cero. 
Realice el diagrama de flujo, el pseudocódigo y el diagrama N/S para 
representarlo, utilizando el ciclo apropiado.

## pseudocodigo

```
Inicio
    leer N
    ceros <= 0
    menores <= 0
    mayores <= 0

    para i < 1 hasta N hacer
        leer número
        si numero = 0 entonces
            ceros < ceros + 1
         Sino
            Si numero < 0 Entonces
                menores ← menores + 1
            Sino
                mayores ← mayores + 1
            FinSi
        FinSi
    FinPara

    Escribir "Cantidad de ceros: ", ceros
    Escribir "Cantidad de menores que cero: ", menores
    Escribir "Cantidad de mayores que cero: ", mayores
Fin
```

## diagrama de flujo 
![bucles](ejercicio2bucles.png)

    
