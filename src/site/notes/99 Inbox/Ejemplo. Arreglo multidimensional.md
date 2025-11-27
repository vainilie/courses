---
{"dg-publish":true,"permalink":"/99-inbox/ejemplo-arreglo-multidimensional/","title":"Ejemplo. Arreglo multidimensional","created":"2025-11-16 14:35","updated":"2025-11-26 18:34"}
---


# Arreglo multidimensional (Matriz 4x4)

Usando PSeInt, realizamos un programa que maneja un arreglo multidimensional (una matriz de 4x4) que captura los valores y muestra los datos.

> [!IMPORTANT] 1\. Siempre declarar el nombre del algoritmo en PSeInt
>
> ``` rust
> Algoritmo Matriz4x4
> ```

> [!TODO] 2\. Declaración del arreglo multidimensional
> Se declara el arreglo multidimensional, en este caso, un arreglo de dos dimensiones donde cada dimensión tiene 4 elementos. Es decir, un arreglo de 4 dentro de cada elemento del arreglo de 4.
>
> ``` rust
> 	Definir matriz Como Entero
> 	Dimension matriz[4, 4]
> ```

> [!TODO] 3\. Captura de datos
> Para la captura de datos, primero se tiene un bucle de la primera dimensión. `i` controla la primera dimensión del arreglo que se recorre con la función `for/para` del índice 0 al 3, es decir, del primer elemento al cuarto elemento.
> ``` rust
> 	Para i <- 0 Hasta 3 Con Paso 1 Hacer
> ```
>
> El bucle de la segunda dimensión del arreglo, del índice 0 al 3, se representará con `j`. Entonces, este `for/para` recorre cada posición dentro de la primera dimensión o el primer arreglo.
> ``` rust
> 		Para j <- 0 Hasta 3 Con Paso 1 Hacer
> ```
>
> Solicita que se ingrese el valor para la posición `[i, j]` del arreglo bidimensional. Al estar dentro de los dos `for/para`, pedirá el valor de cada elemento (16 valores).
> ``` rust
> 			Escribir "Ingrese el valor para la posición [", i, ", ", j, "]:"
> 			Leer matriz[i, j]
> 		FinPara
> 	FinPara
> ```

> [!TODO] 4\. Mostrar el arreglo
> Para mostrar el arreglo multidimensional, se indica que debe recorrer la primera dimensión del arreglo:
>
> ``` rust
> 	Escribir "La matriz ingresada es:"
> 	Para i <- 0 Hasta 3 Con Paso 1 Hacer
> ```
>
> Recorre la segunda dimensión del arreglo y se indica que ha de imprimirse cada elemento. La instrucción `Sin Saltar` indica que los elementos deben imprimirse dentro de la misma línea, sin saltos.
> ``` rust
> 		Para j <- 0 Hasta 3 Con Paso 1 Hacer
> 			Escribir Sin Saltar matriz[i, j], " "
>		Fin Para
> ```
>
> Al final de este arreglo se imprime un salto de línea para separar visualmente cada elemento de la primera dimensión.
> ``` rust
> 		Escribir ""
> 	FinPara
> FinAlgoritmo
> ```

> [!TIP] Output
> Al ejecutarlo, pedirá los valores para cada elemento:
> ``` rust
> Ingrese el valor para la posición [0,0]:
> >
> Ingrese el valor para la posición [0, 1]:
> …
> ```
>
> Al ingresarlos todos, mostrará:
>
> ``` rust
> La matriz ingresada es:
> 11 12 13 14
> 21 22 23 24
> 31 32 33 34
> 41 42 43 44
> ```

## Código completo

``` rust title:"Matriz 4x4"
// Programa: Matriz 4x4
// Descripción: Manejo de arreglo multidimensional (matriz de 4x4)

Algoritmo Matriz4x4
	// Declaración del arreglo multidimensional
	// Un arreglo de 2 dimensiones: 4 elementos en cada dimensión
	Definir matriz Como Entero
	Dimension matriz[4, 4]

	// SECCIÓN 1: CAPTURA DE DATOS

	// i controla la primera dimensión del arreglo (índice 0 a 3)
	Para i <- 0 Hasta 3 Con Paso 1 Hacer

		// j controla la segunda dimensión del arreglo (índice 0 a 3)
		// Este bucle recorre cada posición dentro de la dimensión i
		Para j <- 0 Hasta 3 Con Paso 1 Hacer
			// Solicita el valor para la posición [i, j] del arreglo bidimensional
			Escribir "Ingrese el valor para la posición [", i, ", ", j, "]:"
			Leer matriz[i, j]
		FinPara
	FinPara

	// SECCIÓN 2: MOSTRAR EL ARREGLO MULTIDIMENSIONAL

	Escribir "La matriz ingresada es:"

	// Recorre la primera dimensión del arreglo
	Para i <- 0 Hasta 3 Con Paso 1 Hacer

		// Recorre la segunda dimensión e imprime cada elemento
		Para j <- 0 Hasta 3 Con Paso 1 Hacer
			// "Sin Saltar" mantiene los elementos de la misma dimensión i en una línea
			Escribir Sin Saltar matriz[i, j], " "
		FinPara

		// Salto de línea al terminar de imprimir toda la segunda dimensión
		// Esto separa visualmente cada elemento de la primera dimensión
		Escribir ""

	FinPara

FinAlgoritmo
```
