# Programacion Competitiva Handbook
Este es un libro publico en español en el cual encontraras tips, metodologias y teoria referente a las ciencias de la computación con el fin de brindarte las herramientas para resolver problemas de programación competitiva.

### Acerca de este libro.

### indice
- Como son las competencias.
- Preparacion.
- El lenguaje de programacion. 
- Principales temas:
  - Busquedas.
  - Ordencion.
  - Teoría de grafos.
  - Algoritmos constructivos.
  - Programación Dinámica .
  - Manipulación de bits.
- Ejercicios.
- Mocks de preparacion.



#### ¿ Que es la programacion Competitiva ? 
La programación competitiva combina dos temas: (1) el diseño de algoritmos y (2) la implementación de algoritmos.
El diseño de algoritmos consiste en resolución de problemas y el pensamiento matemática. 
Se necesitan habilidades para analizar problemas y resolverlos creativamente.
Un algoritmo para resolver un problema tiene que ser correcto y eficiente, y el
El núcleo del problema es a menudo inventar un algoritmo eficiente.
El conocimiento teórico de los algoritmos es importante para los programadores competitivos.
Típicamente, una solución a un problema es una combinación de técnicas bien conocidas y
Nuevas ideas Las técnicas que aparecen en la programación competitiva también forman
La base para la investigación científica de algoritmos.
La implementación de algoritmos requiere buenas habilidades de programación. En
programación competitiva, las soluciones se califican probando un implementado
algoritmo utilizando un conjunto de casos de prueba. Por lo tanto, no es suficiente que la idea de la
El algoritmo es correcto, pero la implementación también tiene que ser correcta.
Un buen estilo de codificación en los concursos es sencillo y conciso. Programas
debe escribirse rápidamente, porque no hay mucho tiempo disponible. A diferencia de en
ingeniería de software tradicional, los programas son cortos (generalmente a lo sumo algunos
cien líneas de código), y no es necesario mantenerlas después del concurso.

#### El lenguaje de programación

Por el momento, los lenguajes de programación más populares utilizados en concursos son
C ++, Python y Java. Por ejemplo, en Google Code Jam 2017, entre los mejores
3.000 participantes, el 79% usaban C ++, el 16% usaban Python y el 8% usaban Java [29].
Algunos participantes también usaron varios idiomas.
Mucha gente piensa que C ++ es la mejor opción para un programador competitivo,
y C ++ casi siempre está disponible en sistemas de concurso. Los beneficios de usar C ++
es que es un lenguaje muy eficiente y su biblioteca estándar contiene un gran
colección de estructuras de datos y algoritmos.
Por otro lado, es bueno dominar varios idiomas y comprender
sus puntos fuertes Por ejemplo, si se necesitan enteros grandes en el problema, Python
puede ser una buena opción, ya que contiene operaciones integradas para calcular con enteros grandes. Aún así, la mayoría de los problemas en los concursos de programación se establecen de manera
Un lenguaje de programación específico no es una ventaja injusta.
Todos los programas de ejemplo en este libro están escritos en C ++, y el estándar
Las estructuras de datos y algoritmos de la biblioteca a menudo se utilizan. Los programas siguen el
C ++ 11 estándar, que se puede utilizar en la mayoría de los concursos de hoy en día. Si tu no puedes
programa en C ++ todavía, ahora es un buen momento para comenzar a aprender.

#### Complejidad del tiempo y el espacio.


Complejidad de tiempo


 Introducción

 La complejidad del tiempo algorítmico está relacionada con la rapidez o lentitud de un algoritmo particular.  Definimos la complejidad como una función numérica T (n): tiempo versus el tamaño de entrada n.  Un algoritmo dado tomará diferentes cantidades de tiempo en las mismas entradas dependiendo de factores tales como: velocidad del procesador;  conjunto de instrucciones, velocidad del disco, marca del compilador, etc.

 La solución consiste en estimar la eficiencia de cada algoritmo de forma asintótica.  Mediremos el tiempo T (n) como el número de "pasos" elementales (definidos de cualquier forma), siempre que cada uno de estos pasos lleve un tiempo constante.

 Notaciones asintóticas

 El objetivo de la complejidad computacional es clasificar los algoritmos de acuerdo con sus desempeños.  Representaremos la función de tiempo T (n) usando la notación "big-O" para expresar la complejidad del tiempo de ejecución de un algoritmo.  Por ejemplo, la declaración T (n) = O (n2) dice que un algoritmo tiene una complejidad de tiempo cuadrática.

 Definición de "big Oh"

 Big O describe específicamente el peor de los casos, y puede usarse para describir el tiempo de ejecución requerido o el espacio utilizado (por ejemplo, en la memoria o en el disco) por un algoritmo.

 Ejemplos:

 1 = O (n)

 n = O (n2)

 log (n) = O (n)

 2 n + 1 = O (n)



#### Tiempo constante: O (1)

 Se dice que un algoritmo se ejecuta en tiempo constante si requiere la misma cantidad de tiempo, independientemente del tamaño de entrada.

 Ejemplos:

 matriz: acceder a cualquier elemento

 pila de tamaño fijo: métodos push y pop

 cola de tamaño fijo: métodos en cola y en cola


#### Tiempo lineal: O (n)

 Se dice que un algoritmo se ejecuta en tiempo lineal si su ejecución de tiempo es directamente proporcional al tamaño de entrada, es decir, el tiempo crece linealmente a medida que aumenta el tamaño de entrada.

 En el siguiente ejemplo, se podría encontrar una cadena coincidente durante cualquier iteración del bucle for y la función volvería antes, pero la notación Big O siempre asumirá el límite superior donde el algoritmo realizará el número máximo de iteraciones.


#### Tiempo lineal: O (n)
#### Tiempo lineal: O (log n)

```

```

Ejemplos:

 matriz: búsqueda lineal, recorrido, encontrar mínimo

 ArrayList: contiene el método

 cola: contiene el método


#### Tiempo logarítmico: O (log n)

 Se dice que un algoritmo se ejecuta en tiempo logarítmico si su ejecución de tiempo es proporcional al logaritmo del tamaño de entrada.

```

```

Ejemplo:

 búsqueda binaria

#### Tiempo cuadrático: O (n2)

 Se dice que un algoritmo se ejecuta en tiempo logarítmico si su ejecución de tiempo es proporcional al cuadrado del tamaño de entrada.

 Esto es común con algoritmos que involucran iteraciones anidadas sobre el conjunto de datos.  Las iteraciones anidadas más profundas darán como resultado O (N3), O (N4), etc.

```Java

```
#### Recursion

La recursion es uno de los temas mas importantes dentro de las ciencias de la computacion.Forma parte de los fundamentos de muchos algoritmos y estructuras de datos. Sin embargo, el concepto de recursividad puede ser complicado y tedioso para los programadores que van empezando. 

**¿Que es la recursion?**
La recursividad es una forma de resolver un problema usando una funcion que se llama a si misma.
Puede parecer magico una funcion que se ejecute a si misma. Lo mas interesante es que cada vez que la funcion se llama a si misma, el problema se reduce en sub problemas. La recursion continua de forma indefinida hasta que la funcion llega a un estado en el que ya no puede seguir llamando asi misma.

Una funcion recursiva debe contar con los siguientes elementos:
  *  Un caso base simple
  *  Un conjunto de reglas, tambien conocidas como relacion de recurrencia.
  


```Java

```

#### Listas

```Java

```

#### Strings

```Java

```

#### Arboles

```Java

```

#### Busqueda


```Java

```
#### Ordenamiento 



#### Algoritmos 
