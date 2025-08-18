## Ejercicio 3
Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

### Analisis
### Variables de entrada
 
| Variable       |Descripción                     |
|----------------|----------------------------------|
| cant_lapices   | Cuántos lápices se compran      |
 
### Variables intermedias
 
| Variable | Descripción                  |
|----------|-------------------------------|
| precio   | Valor que hay que pagar       |

### Variables de salida
 
| Variable | Descripción                  |
|----------|-------------------------------|
| precio   | Valor que hay que pagar       |
 
### Constantes
 
| Constante | Descripción                        |
|-----------|-------------------------------------|
| 1000      | Cantidad límite de lápices         |
| 85        | Valor individual cuando hay oferta |
| 90        | Valor individual sin oferta        |



## Pseudocódigo 



## Ejercicio 4

Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.
 
## Análisis
 
 
| Variable de entrada       | Descripción                        |
|----------------|-------------------------------------|
| valor_compra   | Costo parcial de las prendas        |
 
 
 
| Variable de salida       | Descripción                  |
|----------------|-------------------------------|
| precio_final   | Valor que hay que pagar       |
 
 
 
| Constantes  | Descripción                                      |
|-------------|--------------------------------------------------|
| 250000      | Valor a partir del cual se da el descuento
| 15%, 8%     | Descuentos
 
 
## Pseudocódigo
 
```
Inicio
Leer valor_compra
Si valor_compra > 250000
    descuento = valor_compra * 0.15
Si no
    descuento = valor_compra * 0.08
Fin Si
precio_final = valor_compra - descuento
Mostrar "Valor a pagar: $", precio_final
Fin
```

## Ejercicio 5

El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

## Análisis 

### Variables de entrada
| Variable     | Descripción                                  |
|--------------|----------------------------------------------|
| num_alumnos  | Número de alumnos que participan en el viaje |

### Variables intermedias
| Variable      | Descripción                                          |
|---------------|------------------------------------------------------|
| costo_alumno  | Costo que paga cada alumno según el rango de alumnos |
| pago_compañia | Pago total a la compañía de viajes                   |

### Variables de salida
| Variable     | Descripción                            |
|--------------|----------------------------------------|
| pago_compañia| Total a pagar a la compañía de viajes  |
| pago_alumno  | Valor que debe pagar cada alumno       |

### Constantes
| Constante | Descripción                                         |
|-----------|-----------------------------------------------------|
| 65        | Costo por alumno si son 100 o más alumnos           |
| 70        | Costo por alumno si son entre 50 y 99 alumnos       |
| 95        | Costo por alumno si son entre 30 y 49 alumnos       |
| 4000      | Costo fijo del autobús si son menos de 30 alumnos   |


## Pseudocódigo
 
```
INICIO
    LEER num_alumnos

    SI num_alumnos >= 100 ENTONCES
        costo_alumno = 65
        pago_compañia = num_alumnos * costo_alumno
        pago_alumno = costo_alumno

    SINO SI num_alumnos >= 50 Y num_alumnos <= 99 ENTONCES
        costo_alumno = 70
        pago_compañia = num_alumnos * costo_alumno
        pago_alumno = costo_alumno

    SINO SI num_alumnos >= 30 Y num_alumnos <= 49 ENTONCES
        costo_alumno = 95
        pago_compañia = num_alumnos * costo_alumno
        pago_alumno = costo_alumno

    SINO
        pago_compañia = 4000
        pago_alumno = pago_compañia / num_alumnos

    FIN SI

    ESCRIBIR "El total a pagar a la compañía es: ", pago_compañia
    ESCRIBIR "Cada alumno debe pagar: ", pago_alumno
FIN
```


## Ejercicio 6 

Una tienda de ropa tiene la siguiente promoción: por la compra de tres productos, la prenda de menor valor, tiene un 70% de descuento.
Calcular cual fue el descuento aplicado y cuanto tiene que pagar la persona.

## Analisis 
### Variables de entrada
| Variable | Descripción                          |
|----------|--------------------------------------|
| p1       | Precio del primer producto           |
| p2       | Precio del segundo producto          |
| p3       | Precio del tercer producto           |

### Variables intermedias
| Variable  | Descripción                                  |
|-----------|----------------------------------------------|
| menor     | Precio mínimo entre p1, p2 y p3              |
| subtotal  | Suma de los tres precios                     |
| descuento | Descuento aplicado sobre la prenda más barata|
| total     | Total a pagar después del descuento          |

### Variables de salida
| Variable           | Descripción                          |
|--------------------|--------------------------------------|
| descuento_aplicado | Valor del descuento otorgado         |
| total_pagar        | Monto final que debe pagar la persona|

### Constantes
| Constante            | Descripción                                  |
|----------------------|----------------------------------------------|
| 0.70                 | Porcentaje de descuento (70%)                |
| 3                    | Cantidad de productos requerida para promo   |

## Pseudocódigo
 
```
INICIO
  LEER p1
  LEER p2
  LEER p3

  subtotal = p1 + p2 + p3
  menor = p1
  SI p2 < menor ENTONCES
      menor = p2
  FIN SI
  SI p3 < menor ENTONCES
      menor = p3
  FIN SI

  descuento_aplicado = menor * 0.70
  total_pagar = subtotal - descuento_aplicado

  ESCRIBIR "Descuento aplicado: ", descuento_aplicado
  ESCRIBIR "Total a pagar: ", total_pagar
FIN
```
