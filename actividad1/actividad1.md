# Representación de Datos en el Mundo Digital

## Introducción

En la era digital, la información se procesa, almacena y transmite en forma de datos. Entender cómo se representan estos datos en una computadora es esencial para cualquier persona que aspire a programar, ya que determina la manera en que los programas manipulan números, texto, imágenes y otros tipos de información. Un conocimiento sólido de la representación digital de datos ayuda a comprender mejor el funcionamiento interno de los programas y cómo interactúan con el hardware.

En programación, especialmente en Python, es fundamental comprender cómo los datos del “mundo real” se traducen a una forma que la computadora pueda manejar eficientemente. Este tutorial te guiará a través de los conceptos clave de la representación de datos, desde los sistemas numéricos hasta el almacenamiento y codificación de información compleja.

## Contenido Temático

### 2.1. Sistema Binario

### ¿Qué son los valores booleanos?

La lógica booleana, un campo esencial en la teoría de la computación, se fundamenta en los principios introducidos por George Boole, un matemático y lógico británico del siglo XIX. Boole desarrolló un sistema algebraico que permite representar y manipular proposiciones mediante la aplicación de operadores lógicos. Este sistema, conocido como álgebra booleana, establece la base para la representación y procesamiento de información binaria en la computación moderna. La lógica booleana trabaja con valores binarios, donde cada variable puede tener solo dos estados posibles: verdadero (1) o falso (0). Estos valores booleanos son esenciales en la toma de decisiones y el diseño de circuitos lógicos en electrónica, así como en la programación, donde se utilizan para controlar el flujo de ejecución mediante condicionales y bucles.

# Bits y Bytes (representación de datos)

En el ámbito de la informática, los conceptos de bit y byte son fundamentales para comprender la representación y procesamiento de la información. Un bit, la unidad más básica de información binaria, puede adoptar uno de dos estados: 0 o 1. Estos dígitos binarios son la esencia de la codificación de la información en la computación. Por otro lado, un byte consta de ocho bits, lo que amplía significativamente las posibilidades de representación de información. Con un byte, se pueden formar 256 combinaciones únicas de estados binarios ($2^8$), proporcionando la capacidad de representar una amplia gama de datos, desde caracteres individuales hasta valores numéricos más extensos. Los bits y bytes son los bloques de construcción básicos para expresar y manipular información en el mundo digital, permiten almacenar, transmitir y representar información

### ¿Por qué las computadoras trabajan con el sistema binario?

Las computadoras están formadas por millones de pequeños interruptores electrónicos que pueden estar **encendidos (1)** o **apagados (0)**. Esta naturaleza física hace que el sistema binario sea ideal para representar y manipular información digital de manera confiable y eficiente.

### Conversión entre sistemas decimal y binario

**De decimal a binario:**

Para convertir el número decimal 13 a binario:

- 13 / 2 = 6, residuo 1
- 6 / 2 = 3, residuo 0
- 3 / 2 = 1, residuo 1
- 1 / 2 = 0, residuo 1

Escribiendo los residuos al revés: **1101**
**Esquema ASCII Art:**

```
Decimal:  13
Binario:  1101

13 ÷ 2 = 6, residuo 1
6  ÷ 2 = 3, residuo 0
3  ÷ 2 = 1, residuo 1
1  ÷ 2 = 0, residuo 1
(Residuos de abajo hacia arriba)
```

**De binario a decimal:**

Para convertir 1011 a decimal:

$1*(2^3) + 0*(2^2) + 1*(2^1) + 1*(2^0) = 8 + 0 + 2 + 1 = 11$

---

### Ejercicios

**1. Convierte el número decimal 22 a binario.**

**Paso 1:** Dividir 22 entre 2. 

22/2 = 11 residuo: 0

**Paso 2:** Dividir 11 entre 2.

11/2 = 5 residuo: 1

**Paso 3:** Dividir 5 entre 2.

5/2 = 2 residuo: 1

**Paso 4:** Dividir 2 entre 2.

2/2 = 1 residuo: 0 

**Paso 5:** dividir 1 entre 2.

1/2 = 0 residuo: 1

**Binario:** 1 0 1 1 0


**2. ¿Cuál es el resultado en decimal del número binario 10110?**

El número binario 10110 se convierte a decimal de la siguiente manera:

Descomponemos el número binario según las potencias de 2:


1    0    1    1    0  

2⁴  2³  2²  2¹  2⁰

**Calculamos:**

1 × 2⁴ = 16

0 × 2³ = 0

1 × 2² = 4

1 × 2¹ = 2

0 × 2⁰ = 0

16 + 0 + 4 + 2 + 0 = 22

Resultado: 22 en decimal. 


**3. Escribe un programa en Python que convierta un número decimal introducido por el usuario a binario.**

2.2. Representación de Diferentes Tipos de Datos en el Mundo Digital
Números enteros y decimales
Enteros: Se representan directamente en binario.
Decimales (punto flotante): Se representan usando una notación especial (IEEE 754), que usa parte de los bits para la parte entera, otra para la fracción y otra para el signo.
Diagrama conceptual:
[Signo] [Exponente] [Mantisa]
  1 bit    8 bits      23 bits   (en un float de 32 bits)

  ### Caracteres (ASCII, Unicode)

- **ASCII:** Cada carácter se representa por un número entre 0 y 127. Ejemplo: `A` = 65 = 01000001 en binario.
- **Unicode:** Permite representar miles de caracteres de distintos alfabetos y símbolos.

**Tabla ASCII simplificada:**

| Carácter | Decimal | Binario |
| --- | --- | --- |
| A | 65 | 01000001 |
| a | 97 | 01100001 |
| 0 | 48 | 00110000 |

### Imágenes, sonidos y otros datos

- **Imágenes:** Son matrices de píxeles, cada uno representado por valores numéricos (colores RGB).
- **Sonidos:** Son muestras numéricas de la señal de audio en intervalos de tiempo (muestreo digital).

**Ejemplo de imagen:**

```
Matriz de píxeles (3x3):
[ [255,0,0], [0,255,0], [0,0,255] ]
(Rojo, Verde, Azul)
```

---

### **Ejercicios**

**1. Qué número binario representa el carácter 'C' en ASCII?**

Para convertir 67 a binario:

67 ÷ 2 = 33, residuo 1

33 ÷ 2 = 16, residuo 1

16 ÷ 2 = 8, residuo 0

8 ÷ 2 = 4, residuo 0

4 ÷ 2 = 2, residuo 0

2 ÷ 2 = 1, residuo 0

1 ÷ 2 = 0, residuo 1

Leyendo los residuos de abajo hacia arriba: 1000011

 El número binario que representa el carácter 'C' en ASCII es 1000011 


**2. Convierte el número flotante 5.75 a binario (explica los pasos)**

Parte entera: 
Convertimos 5 a binario dividiendo por 2 y guardando los residuos:

5 ÷ 2 = 2, residuo 1

2 ÷ 2 = 1, residuo 0

1 ÷ 2 = 0, residuo 1

Leyendo de abajo hacia arriba:
5 = 101 (en binario)

Parte fraccionaria: 0.75
Multiplicamos por 2 y extraemos la parte entera en cada paso:

0.75 × 2 = 1.5  parte entera: 1, fracción: 0.5

0.5 × 2 = 1.0  parte entera: 1, fracción: 0.0

Entonces:
0.75 = .11 (en binario)

 Resultado: 
Juntamos las dos partes:
5.75 = 101.11 




---
### 2.3. Almacenamiento Digital de Datos

### ¿Cómo se almacenan los datos?

Los datos se almacenan en la memoria y en dispositivos de almacenamiento como secuencias de bits. La unidad básica es el **bit**, pero normalmente se agrupan en **bytes** (8 bits).

- **Palabra:** Unidad de datos que maneja el procesador (puede ser 16, 32 o 64 bits).
- **Unidades de almacenamiento:** 1 byte = 8 bits, 1 KB = 1024 bytes, 1 MB = 1024 KB, etc.

**Diagrama de almacenamiento:**

|--bit--|--bit--|--bit--|--bit--|--bit--|--bit--|--bit--|--bit--|
|------------------------- 1 byte ------------------------------|
​

**Ejemplo:**

Guardar la letra 'A' en memoria:
'A' = 65 = 01000001 (en binario) → almacenado en 1 byte.
Ejercicios
¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?
¿Cuántos bits hay en 5 KB?
2.4. Otras Temáticas Relevantes
Sistema hexadecimal
El sistema hexadecimal (base 16) es usado frecuentemente para representar datos binarios de forma más compacta.
Conversión:
1111 1111 (binario) = FF (hexadecimal)
1010 1100 (binario) = AC (hexadecimal)

**Tabla:**

| Decimal | Hexadecimal | Binario |
| --- | --- | --- |
| 10 | A | 1010 |
| 15 | F | 1111 |

### Errores de redondeo y precisión

En los números de punto flotante, no todos los números decimales pueden representarse exactamente, lo que provoca errores de redondeo.

### Codificación de colores

Colores en computadoras suelen representarse en formato RGB, usando valores hexadecimales:

- Rojo: #FF0000
- Verde: #00FF00
- Azul: #0000FF

### Ejercicios

**1. Convierte el número decimal 255 a hexadecimal.**

**Paso 1:** Divide entre 16

255 ÷ 16 = 15, residuo 15

 
**Paso 2:** Representa los valores en hexadecimal.
El cociente 15 en hexadecimal es F

En hexadecimal, los números del 10 al 15 se representan con letras:

Decimal	Hexadecimal

10  A

11 	B

12  C

13 	D

14 	E

15 	F

El cociente 15 en hexadecimal es F

El residuo 15 también es F




---

## 3. Resumen Visual
[Representación de datos]
     |
     |-- Sistema binario
     |-- Sistema hexadecimal
     |-- Tipos de datos (números, caracteres, imágenes, sonidos)
     |-- Almacenamiento (bits, bytes, palabras)
     |-- Codificación (ASCII, Unicode, RGB)
     
     
 **4. Ejercicios Finales de Repaso**

**1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.**



**2. Convierte el número binario 10011011 a decimal y a hexadecimal.**



**3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.**



**4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?**