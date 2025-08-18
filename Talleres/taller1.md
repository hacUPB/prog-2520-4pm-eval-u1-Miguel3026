# **TALLER DE ALGORITMOS**
**Introducción**

En el ámbito de la ingeniería, la resolución de problemas requiere no solo un análisis preciso de la situación, sino también la capacidad de transformar ese análisis en una solución práctica y eficiente. En este taller, los estudiantes deberán demostrar sus competencias para:

- Analizar problemas relacionados con la ingeniería.
- Diseñar un algoritmo que solucione el problema planteado.
- Representar la solución utilizando pseudocódigo y diagramas de flujo.

Cada problema deberá resolverse empleando estructuras de control como condicionales y bucles, asegurando la correcta interpretación de requisitos y el diseño lógico del flujo de ejecución.

**Ejercicios con condicionales:**




# Ejercicio
 
**Control de temperatura del motor**:
 
- Durante una inspección de rutina, se mide la temperatura de un motor de turbina. Si la temperatura es mayor a un valor crítico, se debe indicar "Peligro: sobrecalentamiento". Si está dentro del rango seguro, indicar "Operación normal". Si es demasiado baja, indicar "Motor frío – Calentar antes de operar".
 
| Tipo                   | Nombre               | Descripción                                                                 |
|------------------------|----------------------|----------------------------------------------------------------------------|
| Variable de entrada    | temperatura_motor    | Temperatura medida del motor durante la inspección (°C)                    |
| Variable intermedia    | Ninguna              | No se realizan cálculos intermedios, solo comparaciones                    |
| Variable de salida     | estado_motor         | Mensaje que indica la condición del motor (Texto)                          |
| Constante              | temp_critica         | Límite superior de temperatura segura antes de sobrecalentamiento (°C)     |
| Constante              | temp_minima_segura   | Límite inferior de temperatura para operación segura (°C)                  |
 
## Pseudocódigo
```
Inicio
    temp_critica = 700
    temp_minima_segura = 200
 
    Leer temperatura_motor
 
    Si temperatura_motor > temp_critica Entonces
        estado_motor = "Peligro: sobrecalentamiento"
    Si no
        Si temperatura_motor >= temp_minima_segura Entonces
            estado_motor = "Operación normal"
        Si no
            estado_motor = "Motor frío – Calentar antes de operar"
        Fin Si
    Fin Si
 
    Mostrar estado_motor
Fin
```

**Ejercicios con bucles:**



# Ejercicio
 
**Registro de altitudes de vuelo**
   
   -  Un sistema debe registrar la altitud de vuelo cada 10 minutos durante una hora y mostrar todas las mediciones al final.
 
| Tipo                   | Nombre             | Descripción                                                    |
|------------------------|--------------------|----------------------------------------------------------------|
| Variable de entrada    | altitud            | Altitud de vuelo registrada en cada medición (pies)            |
| Variable intermedia    | contador           | Número de mediciones realizadas                                |
| Variable de salida     | lista_altitudes    | Lista con todas las altitudes registradas                      |
| Constante              | intervalo_medicion | Intervalo de tiempo entre mediciones (minutos)                 |
| Constante              | tiempo_total       | Duración total de la medición (minutos)                        |
 
 
## Pseudocódigo
```
Inicio
    intervalo_medicion = 10
    tiempo_total = 60
    i=0
 
    Mientras i <= (tiempo_total / intervalo_medicion) Hacer
        Leer altitud
        lista_altitudes[i]=altitud
        i = i + 1
    Fin Mientras
 
    Mostrar lista_altitudes
Fin
```
 

**Ejercicios con bucle y condicionales:**
# Ejercicio
**Simulación de conteo de pasajeros:**
    
- Durante el abordaje, un sistema cuenta a los pasajeros que ingresan. Si el número total supera la capacidad máxima, el sistema debe detener el conteo y mostrar un mensaje de alerta.

| Tipo                   | Nombre             | Descripción                                                                 |
|------------------------|--------------------|-----------------------------------------------------------------------------|
| Variable de entrada    | pasajeros_ingreso  | Número de pasajeros que ingresan en cada evento de abordaje                 |
| Variable intermedia    | total_pasajeros    | Contador acumulado de pasajeros que han ingresado                           |
| Variable de salida     | mensaje_alerta     | Mensaje mostrado cuando se supera la capacidad máxima permitida             |
| Constante              | capacidad_maxima   | Número máximo de pasajeros permitido en el sistema                          |
| Constante              | estado_sistema     | Indica si el conteo continúa o se detiene según la capacidad alcanzada      |


## Pseudocódigo
```
i=0 
mientras i<180
Leer dato 
cantidad_pasajeros[i] = dato 
i=i+1
Fin mientras 
```
 


