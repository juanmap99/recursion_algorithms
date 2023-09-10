# Manual de usuario
Esta herramienta permite entender de manera visual, textual y experimental la manera que funciona la recursividad y programación dinámica a través de una serie de problemas con sus respectivas soluciones.

Los problemas fueron elegidos de manera que cada uno presente un desafío diferente al resto. Aunque todos tienen una naturaleza recursiva que puede dividirse en subproblemas, la estrategia de resolución de cada uno tiene sus propias peculiaridades que lo distinguen de los demás y lo hacen especialmente desafiante. La mayoría de estos problemas se tomaron de LeetCode.

Los detalles de cada problema se abordan en sus respectivas secciones, pero el motivo de elección de cada uno de ellos es el siguiente:
- **Fibonacci:** Se eligió debido a su simplicidad, ya que a menudo es el primer problema utilizado para introducir el concepto de programación dinámica.
- **Target Sum:** El motivo principal para seleccionarlo es que, a diferencia de Fibonacci, es necesario aplicar memorización usando una estructura de datos de tipo diccionario, donde se deben usar dos variables para formar la clave (Key).
- **Combination Sum:**  La motivación para elegir este problema es que requiere un bucle sobre cada llamada recursiva para explorar todas las posibles opciones de combinación.
- **House Robber:** Se eligió este problema porque, a diferencia de los problemas anteriores donde los resultados de los subproblemas se usaban de manera aditiva, aquí se necesita analizar todas las opciones posibles para maximizar las ganancias.
- **Unique Paths:** La razón principal para elegir este problema es que, a diferencia de los anteriores, el proceso recursivo implica recorrer una matriz.

## Modo de ejecución
  La herramienta proporciona a los usuarios dos modos de ejecución distintos:
- **Modo de ejecución manual:** En este modo, el usuario tiene el control total sobre la ejecución del algoritmo. El mismo puede avanzar paso a paso a través del algoritmo presionando un botón para cada paso, lo que le brinda la posibilidad de analizar detalladamente cada cambio y comprender cómo se desarrolla el proceso de ordenamiento. El hecho de que el progreso del proceso de ordenamiento se encuentre bajo el control del usuario lo transforma en el método idóneo a utilizar a la hora de buscar explicarlo en el contexto de una clase.
- **Modo de ejecución automático:** En este modo, el algoritmo se ejecuta de manera automática sin la intervención del usuario. Una vez que el usuario selecciona este modo y ajusta la velocidad deseada, la herramienta inicia el proceso de ordenamiento de forma continua hasta el final.

## Parámetros modificables

Los parámetros modificables base comunes a todos los problemas son:
- **Activar memorización:** Como su nombre lo indica, activa la solución que utiliza programación dinámica para resolver el problema.
- **Velocidad:** Este parámetro determina el tiempo de retraso entre cada paso del algoritmo durante la ejecución automática. A medida que se incrementa la velocidad, disminuye el retraso entre cada paso del algoritmo. Se cuentan con diez velocidades, en donde el retraso asociado a cada una de ellas es el siguiente:
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

En cuanto a los parámetros específicos a cada uno de los problemas, los mismos son:
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

## Estructura del enunciado
El usuario puede activar el enunciado presionando el botón "Enunciado" en la sección inferior de la configuración. Al presionarlo, se abrirá una ventana modal en el centro de la pantalla que permite al usuario interactuar con ella.

La estructura del enunciado es la misma para todos los problemas y sigue el siguiente formato:
- **Introducción al problema:** Se detallan los objetivos y parámetros proporcionados. En el caso del problema "Unique Paths", se incluye una visualización gráfica.
- **Ejemplos:** Se muestra la salida generada al ingresar cierta entrada, junto con una explicación del motivo detrás de esa salida.
- **Restricciones:** Se detallan las restricciones del problema y de los inputs.
- **Follow-up:** Se presentan desafíos adicionales propuestos para el usuario.

## Estructura de la explicación
El usuario puede activar la explicación presionando el botón "Explicación" en la sección inferior de la configuración. Al hacerlo, se abrirá una ventana modal en el centro de la pantalla que permite al usuario interactuar con ella.
La estructura de la explicación es la misma para todos los problemas y sigue el siguiente formato:
- **Página uno - Solución sin programación dinámica**
  - Imagen del código en Python que representa la solución al problema sin utilizar programación dinámica.
  - Explicación detallada del código.
  - Identificación del problema presente en la solución debido a la falta de programación dinámica.
  - Gráfico de llamadas generado a partir de cierta entrada (input).
- **Página dos- Solución con programación dinámica**
  - Imagen del código en Python que representa la solución al problema utilizando programación dinámica.
  - Explicación detallada del código.
  - Descripción de cómo se resuelve el problema que existía en la solución previa mediante la introducción de programación dinámica.
  - Gráfico de llamadas generado para el mismo ejemplo utilizado en la página anterior, pero esta vez utilizando programación dinámica. Esto se realiza para resaltar las ventajas que ofrece la programación dinámica.

## Estructura de la tabla
La tabla se activa junto con la ejecución y se utiliza para mostrar toda la información relacionada con todas las llamadas realizadas a la función. Gráficamente, se encuentra ubicada debajo del código.

La tabla consta de cuatro columnas en total, que son las siguientes:
- **Counter:** Un valor incremental secuencial que identifica cada llamada. Este contador es útil para obtener información sobre cuántas veces se ha llamado a la función hasta llegar a una solución.
- **Tree Depth:** Representa la profundidad de la llamada en el árbol de llamadas. La profundidad de una llamada se determina sumándole uno a la profundidad de la llamada que llamó a la función, en donde la primera llamada a la función tiene una profundidad igual a cero.
- **Parameters:** Link clickeable que abre una ventana modal en el centro de la pantalla, donde se muestran los valores de cada uno de los parámetros que recibió la llamada. En el contexto de la programación dinámica, el único parámetro que se excluye es el "memo", ya que es dinámico y común a todas las llamadas.
Output: Representa el resultado de una llamada cuando esta finaliza su ejecución. Mientras la llamada no haya finalizado, el valor de este campo es “Wating..”.
 
A excepción de la columna "Parameters", todos los campos se pueden ordenar tanto de manera ascendente como descendente, lo que es muy útil para realizar análisis estadísticos y también para seguir las llamadas en relación con el árbol de llamadas.

Al finalizar la ejecución del algoritmo, la fila con un Counter igual a uno, que representa la primera llamada realizada, se resalta en amarillo para indicar que la ejecución ha finalizado y se ha obtenido el resultado (Output) final.
