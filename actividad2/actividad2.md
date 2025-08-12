# Algoritmos

## Introducción

Un algoritmo es un conjunto de pasos o instrucciones secuenciales que permiten resolver un problema.
Existen dos tipos principales:

1. **Cualitativos**: Describen pasos a través de palabras. Por ejemplo, las instrucciones para preparar una receta de cocina, como "mezclar los ingredientes" u "hornear durante 30 minutos", constituyen un algoritmo cualitativo.
2. **Cuantitativos**: Incluyen cálculos numéricos. Por ejemplo, un algoritmo para calcular el volumen de una caja: `Volumen = Largo * Ancho * Alto`.

## Características de los Algoritmos

Un buen algoritmo debe cumplir las siguientes características:

- **Precisión**: Los pasos deben ser claros y concisos. Te voy a poner un ejemplo de lo que no se debe hacer: un algoritmo que diga `Suma los números ingresados y muestra el resultado` sin especificar cómo ingresarlos, cómo procesarlos ni cómo mostrarlos. Este nivel de ambigüedad genera confusión y dificulta su implementación correcta.
- **Determinismo**: Dados los mismos datos de entrada, siempre produce el mismo resultado. Por ejemplo, si mi algoritmo calcula el factorial de un número entero, cada vez que yo le ingrese 5, el resultado será 120, no importa cuántas veces ejecute el programa.
- **Finitud**: Debe terminar en un tiempo razonable y no caer en ciclos infinitos. Aquí te voy a dar otro ejemplo de lo que no se debe hacer: Un algoritmo que incluye una condición mal diseñada:

Mientras (x != 10) { x = x - 2 }


Si x empieza siendo impar, nunca alcanzará el valor 10 y el ciclo será infinito. 
Un bucle sin límite de iteraciones: 
Para i desde 0 hasta infinito { imprimir(i) }
​
Este bucle no tiene fin y puede colapsar el sistema.
Estos ejemplos ilustran problemas comunes a evitar en el diseño de algoritmos.


## Ejercicio 1.

Investiga cuáles son los símbolos que se utilizan para representar cada operación de un algorimo con un diagrama de flujo. Asegúrate de que la fuente es confiable, discute lo que encontraste con tus compañeros y con el profe. Cuando estés seguro/a de tener los símbolos correctos, consigna la información en la bitácora.

**R/**
 | Símbolo               | Forma               | Uso principal                            |
|-----------------------|---------------------|-------------------------------------------|
| Terminal              | Óvalo    | Inicio o fin del algoritmo                |
| Proceso               | Rectángulo          | Acción u operación                        |
| Decisión              | Diamante (rombo)    | Punto de bifurcación (condición)          |
| Entrada/Salida        | Paralelogramo       | Input u output de datos                   |
| Línea de flujo        | Flechas             | Indicar secuencia del flujo               |
| Proceso predefinido   | Rectángulo doble    | Subproceso definido en otro lugar         |
| Conectores            | Círculo / Pentágono | Conexión dentro o fuera de la página      |
| Comentario  | Rectángulo abierto  | Información adicional                     |


