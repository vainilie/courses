---
{"dg-publish":true,"permalink":"/01-curso-fundamentos/00-archivos/practica-4-a/","title":"Practica 4A"}
---


- Nombre de la práctica: Resolución de problemas complejos utilizando algoritmos
- Unidad: 4: Resolución de problemas y desarrollo lógico

Introducción

- Se pondrá en práctica las habilidades para la solución de problemas utilizando algoritmos.
- Los ejercicios son graduales, irán poniendo en práctica conocimientos adquiridos. Entre más se avance, más se llegará a planteamientos complejos con necesidad de activar el pensamiento lógico y creatividad.
- Se usará PSeInt para codificación, con el objetivo de llegar al resultado esperado.
- Se plantearán situaciones ordinarias.
	1. Debes analizar el problema,
	2. descomponerlo en fracciones más pequeñas
	3. diseñar algoritmos que resuelvan cada sección.
	4. Es necesario usar diferentes estructuras de datos y algoritmos hasta la solución total.
- Objetivo: Adaptarse a la herramienta y su semántica.
- Desarrollo:
	1. Lee cada problema detenidamente. Irán aumentando de dificultad.
	2. Utiliza tu pensamiento crítico para idear un plan de trabajo. Debes tomar en cuenta las restricciones planteadas.
	3. Desarrolla en PSeInt cada algoritmo.
		1. Ejecútalos, siguiendo la secuencia y haz pruebas.

# Introducción

# Objetivos

# Desarrollo

## Etapa 1: Duplicados

Debes encontrar valores duplicados en un arreglo de números enteros y regresar un arreglo con los números que se repitan exactamente 2 veces.

> [!note] Note
> Prueba tu algoritmo para los siguientes casos:
>
> - [4,3,2,7,8,2,3,1] = [3,2]
> - [1,1,2] = [1]
> - \[1] = []

### Descripción del problema

### Desarrollo del algoritmo

### Código

### Resultados

## Etapa 2: Cadena a la inversa

Regresa una cadena de texto en sentido inverso.

> [!note] Note
> - El programa debe solicitar una cadena de texto al usuario.
> - Prueba tu algoritmo con las siguientes cadenas:
> 	- galleta =
> 	- procesador =
> 	- vehículo =
> - Una vez que hayas conseguido lo anterior, agrega una validación para regresar Verdadero si la palabra es un palíndromo. Prueba tu algoritmo con los valores:
> 	- rotor =
> 	- sometemos =
> 	- reconocer =

### Descripción del problema

### Desarrollo del algoritmo

### Código

### Resultados

## Etapa 3: Calculadora de edad

Trabajas en una compañía que ofrece seguros de vida y de gastos médicos. La empresa está desarrollando una herramienta tecnológica, para que los agentes puedan calcular el monto de una póliza. Para dicho cálculo, se consideran varios factores de riesgo, entre los que se encuentra la edad. Por ello, el contratante debe llenar un formulario, incluyendo su fecha de nacimiento. Como primer reto, deberás calcular la edad del cliente al momento de la cotización.

> [!note] Note
> - La captura de la fecha de nacimiento debe ser en una sola cadena de texto con formato DD-MM-AAAA
> - Debes validar que es una fecha válida; para simplificar el algoritmo tomaremos el día 29 de febrero como inválido
> - El año de nacimiento debe ser mayor a 1900
> - No olvides validar si el cliente ya cumplió años en la fecha de captura o aún no

### Descripción del problema

### Desarrollo del algoritmo

### Código

### Resultados

## Etapa 4: Dispensadora de billetes

Has sido contratado por un banco que está en un proceso de actualización de su red de cajeros automáticos. Tu trabajo es desarrollar el algoritmo con el cual va a operar la dispensadora de billetes. Para que el cajero realice esta tarea, deberás considerar las siguientes premisas:

> [!note] Note
> - Entregar siempre la menor cantidad de billetes
> - Mantener un inventario que indique, cuál es la cantidad de billetes disponible para cada denominación
> - Las denominaciones disponibles son 20, 50, 100, 200, 500 y 1000
> - Si el inventario no cuenta con una combinación de billetes, suficiente para satisfacer el importe solicitado, no dispensará ningún billete
> - Para efectos de esta práctica, siempre que inicie el algoritmo, deberá haber en inventario, 10 billetes de cada denominación

### Descripción del problema

### Desarrollo del algoritmo

### Código

### Resultados

## Etapa 5: Máquina expendedora

Eres un emprendedor entusiasta y tienes la oportunidad de instalar una máquina expendedora de botanas en un auto lavado cercano a tu casa. Te corresponde desarrollar el algoritmo para que cuente las monedas que el usuario va insertando, sumando el importe en una variable hasta que el usuario introduzca un código de algunos de los productos que están disponibles. debes validar que el importe pagado sea suficiente. Hay que tener en cuenta las siguientes restricciones:

> [!note] Note
> - El algoritmo deberá aceptar los siguientes comandos:
> 	- `[NUMERO]`. Será un valor numérico que representa la moneda que está entrando al sistema.
> 	- `[IDENTIFICADOR]`. Será una clave para identificar los productos que están disponibles con el formato `[LETRA][NÚMERO]`, por ejemplo, D4, A3, etc.
> 	- `[RETIRAR]`. Si se recibe este comando, se devolverá el importe al usuario cancelando la operación.
> 	- `[PARA]`. Este comando será para detener la ejecución
> - La máquina sólo acepta monedas de 1, 2, 5, 10 y 20 pesos. Cualquier otra moneda que entre al sistema será rechazada
> - No te preocupes por llevar el detalle de las monedas que el cliente ha introducido, solo el importe.
> - En este problema, no ocupas tomar en cuenta el inventario disponible de cada producto
> - El algoritmo debe reiniciarse cada vez que se haya dispensado un producto y deberá mantenerse corriendo hasta que sea introducido el comando para salir
> - Intenta dividir tu programa en funciones para que tu código sea más comprensible

### Descripción del problema

### Desarrollo del algoritmo

### Código

### Resultados

# Conclusiones
