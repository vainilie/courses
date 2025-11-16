---
{"dg-publish":true,"permalink":"/01-curso-fundamentos/01-unidades/03-algoritmos-poo/ejemplo-arreglo-multidimensional/","title":"Ejemplo. Arreglo multidimensional"}
---


# Arreglo multidimensional (Matriz 4x4)

Usando PSeInt, realizamos un programa que maneja un arreglo multidimensional (una matriz de 4x4) que captura los valores y muestra los datos.

1. Siempre declarar el nombre del algoritmo en PSeInt.

	```psc
	Algoritmo Matriz4x4
	```

2. Se declara el arreglo multidimensional, en este caso, un arreglo de dos dimensiones donde cada dimensión tiene 4 elementos. Es decir, un arreglo de 4 dentro de cada elemento del arreglo de 4.

	```pseud
		Definir matriz Como Entero
		Dimension matriz[4, 4]
	```

3. Para la captura de datos, primero se tiene un bucle de la primera dimensión. `i` controla la primera dimensión del arreglo que se recorre con la función `for/para` del índice 0 al 3, es decir, del primer elemento al cuarto elemento.

	```psc
		Para i <- 0 Hasta 3 Con Paso 1 Hacer
	```

4. El bucle de la segunda dimensión del arreglo, del índice 0 al 3, se representará con `j`. Entonces, este `for/para` recorre cada posición dentro de la primera dimensión o el primer arreglo.

	```psc
			Para j <- 0 Hasta 3 Con Paso 1 Hacer
	```

5. Solicita que se ingrese el valor para la posición `[i, j]` del arreglo bidimensional. Al estar dentro de los dos `for/para`, pedirá el valor de cada elemento (16 valores).

	```psc
				Escribir "Ingrese el valor para la posición [", i, ", ", j, "]:"
				Leer matriz[i, j]
			FinPara
		FinPara
	```

6. Para mostrar el arreglo multidimensional, se indica que debe recorrer la primera dimensión del arreglo:

```psc
	Escribir "La matriz ingresada es:"
	
	// Recorre la primera dimensión del arreglo
	
```

7. Recorre la segunda dimensión del arreglo y se indica que ha de imprimirse cada elemento. La instrucción `Sin Saltar` indica que los elementos deben imprimirse dentro de la misma línea, sin saltos.

```psc
		Para j <- 0 Hasta 3 Con Paso 1 Hacer
			// "Sin Saltar" mantiene los elementos de la misma dimensión i en una línea
			Escribir Sin Saltar matriz[i, j], " "
	
```

8. Al final de este arreglo se imprime un salto de línea para separar visualmente cada elemento de la primera dimensión.

```psc
		Escribir "" 

	FinPara
	FinAlgoritmo

```

## Código completo

```c++
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


```pseudo
\begin{algorithm} \caption{Matriz 4x4} \begin{algorithmic} \State Definir matriz Como Entero \State Dimension matriz[4,4] \For{$i \gets 0$ to $3$} \For{$j \gets 0$ to $3$} \State Escribir "Posición [", i, ",", j, "]" \State Leer matriz[i,j] \EndFor \EndFor \end{algorithmic} \end{algorithm}
```