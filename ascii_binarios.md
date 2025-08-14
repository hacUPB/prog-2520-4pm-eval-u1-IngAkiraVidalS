# Actividad2 Uni2

## 1. ¿Qué numero binario representa el caracter 'C' en ASCII?

    El código ASCII para la letra **'C'** es **67** en decimal.
    El valor binario de 67 es:  
  **01000011**

## 2. Conversion #flotante 5.75 a binario IEEE 754

### 1° paso: parte entera (5)
    5 en binario = `101`

 ### 2° paso: parte entera (.75)
    0.75 * 2 = 1.5 -> 1
    0.5 * 2 = 1.0 -> 1

    entonces:
    0.75 = `.11`

### resultado:

**5.75** en binario = `101.11`

---

### (Opcional IEEE 754 simple precisión)

    5.75 → signo: 0 (positivo) 
    Binario normalizado: `1.0111 × 2^2`
    Exponente en exceso 127: 127 + 2 = 129 → `10000001`
    Mantisa (23 bits): `01110000000000000000000`


**IEEE 754 (32 bits):**  
`0 10000001 01110000000000000000000`


