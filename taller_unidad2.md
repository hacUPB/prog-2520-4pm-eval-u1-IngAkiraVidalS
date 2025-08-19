## taller unidad 2

### verificacion de pego de despegue 

1. **Verificación de peso de despegue**
    
    En una pista de pruebas de aeronaves, el sistema debe verificar si el peso total de la aeronave, incluyendo combustible y carga, supera el límite máximo permitido para el despegue. Dependiendo del resultado, el sistema deberá indicar si la aeronave está lista para despegar o si debe reducir carga o combustible.


## analisis 

| variables de entrada | descripción |
|----------------------|-------------|
| peso _max             |peso maximo de la aeronave a analizar |
| peso_combustible      | peso combustible estimada |
| peso_carga            | peso de la carga estimad (pasajeros, equipaje y carga paga)
| peso_vacio            |peso de la aeronave vacía |


|variables intermedia  | descripcion |
|----------------------|-------------|
| peso estimado        | la suma del peso del combustible, de la carga y del peso vacío |

|variables de salida | descripcion |
|--------------------|-------------|
| limite_max | si sobre pasa el límite de peso max o no |




## diagrama de flujo 

![verificacion](Verificación_de_peso_de_despegue.png)








### **Ejercicios con bucles**

1. **Registro de altitudes de vuelo**
    
    Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.


## analisis 

| variables de entrada | descripción |
|----------------------|-------------|
|altitud               |altitud registrada |


|variable de control   | descripcion |
|----------------------|-------------|
| i                    | ----------- |

|variables de salida | descripcion |
|--------------------|-------------|
| alt_tiempo         | altitudes en el tiempo |

## pseudocodigo 

```
Inicio
 Escribir "   REGISTRO DE ALTITUDES CADA 10 MINUTOS"
    Escribir "   Intervalo: ", INTERVALO_MIN, " min | Duración: ",
             DURACION_MIN, " min | Mediciones: ", NUM_MEDICIONES

  Para i ← 0 Hasta (NUM_MEDICIONES - 1) Hacer
       minuto ← i * INTERVALO_MIN

        Repetir
            Escribir "Ingrese la ALTITUD (en pies) para el minuto ", minuto, ":"
            Leer altitud

            Si (altitud < 0) Entonces
                Escribir "  ** Error: la altitud no puede ser negativa. Intente de nuevo."
                valido ← FALSO
            Sino
                valido ← VERDADERO
            FinSi
        HastaQue (valido = VERDADERO)

        alt_tiempo[i] ← altitud
        Escribir "  > Medición ", (i + 1), " registrada: ",
                 alt_tiempo[i], " pies en el minuto ", minuto, "."

  FinPara

     Escribir "========= RESUMEN DE ALTITUDES REGISTRADAS ========="
    Para i ← 0 Hasta (NUM_MEDICIONES - 1) Hacer
        minuto ← i * INTERVALO_MIN
        Escribir "Minuto ", minuto, "  →  ", alt_tiempo[i], " pies"
    FinPara

Fin
```


 ### **Ejercicios con bucle y condicionales**

  3. **Simulación de conteo de pasajeros**
    
    Durante el abordaje, un sistema cuenta a los pasajeros que ingresan. Si el número total supera la capacidad máxima, el sistema debe detener el conteo y mostrar un mensaje de alerta.

    
| variables de entrada | descripción |
|----------------------|-------------|
|Capacidad_max         |capacidad máxima del avión
|pasajero              |cantidad de pasajeros que entran (simulado por el sistema o ingresado manualmente)|


|variable de control   | descripcion |
|----------------------|-------------|
|total_pasajeros       |acumulador de pasajeros |
| i                    | contador de iteraciones (opcional si se simula con bucle) |

|variables de salida | descripcion |
|--------------------|-------------|
| total_pasajeros    | cantidad final de pasajeros registrados |

![verificacion](CONTEOPASAJEROS.png)