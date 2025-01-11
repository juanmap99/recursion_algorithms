# Manual de usuario
Esta herramienta está diseñada para facilitar la comprensión visual, textual y práctica de conceptos avanzados como la recursividad y la programación dinámica a través de la resolución de diversos problemas seleccionados cuidadosamente.

Cada problema aborda un desafío único, destacando diferentes estrategias y peculiaridades en su solución. La mayoría de los problemas fueron tomados de LeetCode, garantizando su relevancia y nivel adecuado de dificultad.

## Problemas Implementados
Los problemas incluidos y las razones de su selección son las siguientes:
- **Fibonacci:** Elegido por su simplicidad, ideal para introducir el concepto de programación dinámica.
- **Target Sum:** : Destacado por requerir una estructura de memorización usando un diccionario con claves compuestas por dos variables.
- **Combination Sum:**  Presenta la necesidad de utilizar un bucle dentro de cada llamada recursiva para explorar todas las posibles combinaciones.
- **House Robber:** Ilustra cómo evaluar múltiples opciones para maximizar un beneficio, diferenciándose de problemas donde los resultados de subproblemas se suman directamente.
- **Unique Paths:** Introduce un proceso recursivo que involucra la navegación a través de una matriz, ofreciendo una perspectiva diferente sobre la recursión y la programación dinámica.

## Modo de ejecución
La herramienta ofrece dos modos de ejecución adaptados a diferentes necesidades de aprendizaje:

### 1. Modo Manual
Permite al usuario avanzar paso a paso presionando un botón para cada iteración del algoritmo. Este enfoque facilita un análisis detallado de cada cambio, ideal para entornos educativos o para aquellos que deseen comprender profundamente cada etapa del proceso.

### 2. Modo Automático
El algoritmo se ejecuta de manera continua sin intervención del usuario. Antes de comenzar, el usuario puede ajustar la velocidad de ejecución según sus preferencias.

## Parámetros Modificables

### Parámetros Comunes
- **Activar memorización:** Permite activar la versión del algoritmo que utiliza programación dinámica para optimizar la solución.
- **Velocidad:** Controla el retraso entre los pasos en el modo automático. Hay diez niveles de velocidad:
  - Velocidad 1: 1000 ms
  - Velocidad 2: 500 ms
  - Velocidad 3: 250 ms
  - Velocidad 4: 100 ms
  - Velocidad 5: 60 ms
  - Velocidad 6: 30 ms
  - Velocidad 7: 10 ms
  - Velocidad 8: 5 ms
  - Velocidad 9: 2 ms
  - Velocidad 10: 0.6 ms

### Parámetros Específicos por Problema
Cada problema tiene configuraciones únicas que permiten personalizar su ejecución:
- **Fibonacci**
  - Parámetro 1: Fibonacci calcular
    - Descripción: Determina el número del cual se desea conocer el Fibonacci.
    - Restricciones
      - El número introducido debe ser un entero positivo con menos de cuatro dígitos.
    - Ejemplo: 5
- **Target Sum**
  - Parámetro 1: Array de elementos
    - Descripción: Determina el array de elementos sobre el cual se resuelve el problema.
    - Restricciones
      - El array debe estar encerrado en corchetes y los valores separados por una coma.
      - Los números introducidos deben ser enteros positivos.
    - Ejemplo: [2,3,6,5,4]
  - Parámetro 2: Target sum
    - Descripción: Número que representa la suma total a la que se desea llegar.
    - Restricciones
      - El número introducido debe ser un entero positivo con menos de seis dígitos.
    - Ejemplo: 358
- **Combination Sum**
  - Parámetro 1: Array de elementos
    - Descripción: Array que representa los números que pueden ser utilizados para la suma.
    - Restricciones
      - El array debe estar encerrado en corchetes y los valores separados por una coma.
      - Los números introducidos deben ser enteros positivos.
    - Ejemplo: [12,5,6,1,2,3]
  - Parámetro 2: Target sum
    - Descripción: Número que representa la suma total a la que se desea llegar utilizando los elementos del array.
    - Restricciones
      - El número introducido debe ser un entero positivo con menos de seis dígitos.
    - Ejemplo: 358
- **House Robber**
  - Parámetro 1: Dinero casas
    - Descripción: Array que representa el dinero de cada una de las casas.
    - Restricciones
      - El array debe estar encerrado en corchetes y los valores separados por una coma.
      - Los números introducidos deben ser enteros positivos.
    - Ejemplo: [125,36,95,20,36]
- **Unique Paths**
  - Parámetro 1: Filas
    - Descripción: Valor que representa la cantidad de filas en la matriz.
    - Restricciones
      - El número introducido debe ser un entero positivo con menos de cuatro dígitos.
    - Ejemplo: 11
  - Parámetro 2: Columnas
    - Descripción: Valor que representa la cantidad de columnas en la matriz.
    - Restricciones
      - El número introducido debe ser un entero positivo con menos de cuatro dígitos.
    - Ejemplo: 13

## Estructura del Enunciado
El botón "Enunciado" permite acceder a una descripción detallada del problema. Al hacer clic, se abre una ventana modal que sigue esta estructura:

- **Introducción al problema:** Objetivo y parámetros específicos.
- **Ejemplos:** Entradas y salidas con explicaciones.
- **Restricciones:** Detalles sobre los límites de los valores permitidos.
- **Follow-up:** Retos adicionales relacionados con el problema.

## Estructura de la Explicación
El botón "Explicación" proporciona un análisis completo del problema en dos partes:

### Página 1: Solución sin Programación Dinámica

  - Código en Python.
  - Explicación detallada del código.
  - Análisis detallado de sus limitaciones debido a la falta de programación dinámica.
  - Representación gráfica de las llamadas recursivas para un caso específico.

### Página 2: Solución con Programación Dinámica

  - Código en Python.
  - Explicación detallada del código.
  - Explicación de cómo se resuelven las limitaciones de la solución básica.
  - Gráfico comparativo que resalta la eficiencia de la solución optimizada.

## Estructura de la tabla
Durante la ejecución, se genera una tabla que registra información clave sobre las llamadas recursivas. Está ubicada debajo del código y contiene las siguientes columnas:

- **Counter:** Identifica cada llamada con un número secuencial.
- **Tree Depth:** Indica la profundidad de la llamada en el árbol recursivo.
- **Parameters:** Link que abre una ventana modal mostrando los valores recibidos por la llamada (excluyendo el parámetro memo).
- **Output:** Resultado de la llamada, o "Waiting.." si la ejecución aún no ha finalizado.

### Funcionalidades de la Tabla

- Ordenamiento ascendente y descendente en todas las columnas (excepto "Parameters").
- Resaltado en amarillo de la primera llamada al finalizar la ejecución, indicando el resultado final.
