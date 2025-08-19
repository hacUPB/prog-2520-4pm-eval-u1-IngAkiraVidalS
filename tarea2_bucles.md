## tarea2_bucles 
 
### ejercicio 4.8 pag 138

### analisis 

Realice el algoritmo para determinar cuánto pagará una persona que 
adquiere N artículos, los cuales están de promoción. Considere que 
si su precio es mayor o igual a $200 se le aplica un descuento de 15%, 
y si su precio es mayor a $100 pero menor a $200, el descuento es de 
12%; de lo contrario, sólo se le aplica 10%. Se debe saber cuál es el 
costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la 
solución mediante el diagrama de flujo, el pseudocódigo y el diagrama N/S.

**Se tienen N artículos en promoción.**

Según el precio de cada artículo , se aplica un descuento:
Si precio ≥ 200 → descuento 15% .Si 100 < precio < 200 → descuento 12% .Si precio ≤ 100 → descuento 10% .Para cada artículo se debe mostrar: Su precio original, el descuento aplicado. Al final, muestre el total a pagar por todos los artículos.


```
Inicio
    Escribir "Ingrese la cantidad de artículos:"
    Leer N

    totalPagar ← 0

    Para i ← 1 Hasta N Hacer
        Escribir "Ingrese el precio del artículo ", i, ":"
        Leer precio

        Si precio >= 200 Entonces
            descuento ← precio * 0.15
        Sino
            Si precio > 100 Y precio < 200 Entonces
                descuento ← precio * 0.12
            Sino
                descuento ← precio * 0.10
            FinSi
        FinSi

        precioFinal ← precio - descuento
        totalPagar ← totalPagar + precioFinal

        Escribir "Artículo ", i, ":"
        Escribir "  Precio original: $", precio
        Escribir "  Descuento: $", descuento
        Escribir "  Precio final: $", precioFinal
    FinPara

    Escribir "Total a pagar por todos los artículos: $", totalPagar
Fin
```
### diagrama 

![tareabucles](ejercicio4.8.png)




## ejercicio 2

### analisis 

Tienen una tarjeta de $10.000.000. Calcular el valor de todas las cuotas sabiendo:

Valor de la compra
Tasa de interés del 2%
Número de cuotas. Máximo 36. 

```
Inicio
    Definir VALOR_TARJETA como 10000000
    Definir tasa_interes como 0.02

    Escribir "Ingrese el valor de la compra:"
    Leer valor_compra

    Si valor_compra > VALOR_TARJETA Entonces
        Escribir "El valor de compra es mayor al límite de la tarjeta."
        Terminar
    FinSi

    Escribir "Ingrese el número de cuotas (máximo 36):"
    Leer num_cuotas

    Si num_cuotas > 36 Entonces
        Escribir "Número de cuotas no puede ser mayor a 36."
        Terminar
    FinSi

    Definir cuota_base, cuota_con_interes, i como Entero
    cuota_base = valor_compra / num_cuotas

    Para i = 1 Hasta num_cuotas Hacer
        cuota_con_interes = cuota_base + (cuota_base * tasa_interes)
        Escribir "Cuota ", i, ": ", cuota_con_interes
    FinPara
Fin
```
![tareabucles](ejercicio2tarea.png)
