# Ejercicios finales de repaso

---

## 1. ¿por qué las computadoras usan binario?
    Las computadoras utilizan componente electronicos que funcionan con dos estados: 
    encendido y apagado.
    El sistema binario (1 y 0)reprenta estos estados físicos. Por eso, es eficiente y confiable para alamcenar y procesar información.

---

## 2. conversión de `10011011`

### a decimal:

    Se descompone el # binario:
1×2⁷ + 0×2⁶ + 0×2⁵ + 1×2⁴ + 1×2³ + 0×2² + 1×2¹ + 1×2⁰
= 128 + 0 + 0 + 16 + 8 + 0 + 2 + 1 = **155**


### a hexadecimal:

    Agrupamos en bloques de 4 bits:
1001  1011 -> 9B
**resultado: 0x9B**

---

## 3. ¿cómo se representa una imagen PNG en el disco?

Una imagen en formato PNG se guarda en el disco como una **secuencia binaria estructurada**. Está compuesta por:

*Firma PNG:** 8 bytes al inicio (`89 50 4E 47 0D 0A 1A 0A`)
**Chunks o bloques:** Cada uno con datos específicos. Por ejemplo:
`IHDR`: ancho, alto, profundidad de color
`IDAT`: los datos de la imagen (comprimidos con zlib)
`IEND`: marca el fin del archivo

Cada byte representa parte de la información visual. PNG es un formato **sin pérdida**, ideal para gráficos nítidos como logotipos o ilustraciones.

---

## 4. ¿qué pasa si ntento alamcenr un # mayor que 255 en un byte?

Un byte puede representar hasta 255 (en decimal). Si se intenta almacenar 300, se produce un **desbordamiento** o error si el lenguaje no lo permite.

### en PYTHON:

    Python no limita enteros a 8 bits.
    ``` python
     x = 300
     print(x) # imprime 300 sin error.

     pero si se intenta convertirlo manualmente a un byte, así
     bytes([300])
 python enviará un **ValueError** 

    Ya que python maneja esto con seguridad, evitando errores al trabajar con datos binarios.