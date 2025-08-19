## tarea pregunta al usuario

### analisis

Preguntar al usuario la fecha de nacimiento, con tre variables: día, mes y año y cuál es la fecha actual, día actual, mes actual, año actual y con eso calcular cuántos años tiene la persona?

| variables de entrada | descripción |
|----------------------|-------------|
|cumple_feliz          |día de nacimiento |
|mes_de_cumple         |mes de nacimiento |
|fecha_nacimiento      |fecha de nacimiento|
|año_nacim             | año de nacimiento |
|dia_act               | día actual   |
|mes_act               | mes actual   |
|año_act               | año actual   |

|variables de salida | descripcion |
|--------------------|-------------|
| edad | edad calculada en años |


```
Inicio
    escriba "ingrese el día de nacimiento:"
    leer cumple_feliz
    escriba "ingrese el mes de nacimiento:"
    leer mes_de_cumple
    escriba "ingrese el año de nacimiento:"
    leer año_nacim 

    escriba "ingrese el día actual:"
    leer dia_act 
    escriba "ingrese el mes actual:"
    leer mes_act
    escriba "ingrese el año actual:"
    leer año_act

    edad ← año_act - año_nacim

    Si (mes_act < mes_de_cumple) o (mes_act = mes_de_cumple y dia_act < cumple_feliz) Entonces
        edad ← edad - 1 
    FinSi

    Escribir "La edad es: ", edad, " años"
Fin
```

![pregunta_al_usuario](datos_usuario.png)