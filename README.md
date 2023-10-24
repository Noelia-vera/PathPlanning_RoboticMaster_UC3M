# PathPlanning_RoboticMaster_UC3M
## _Master de Robótica y Automatización, Universidad Carlos 3 de Madrid_
### Introducción a la Planificación de Robots
</p>

***
#### ORGANIZACIÓN DE CARPETAS:
* **doc:** Instalación de la carpeta. Dado por el profesor.
* **map1-11:**  src de los mapas para probar los algoritmos. Dado por el profesor.
* **share:** openrave. Dado por el profesor.
* **src:** dentro se encuentran las parpetas con distintos lenguajes de programación. La que se ha usado en este caso es la del lenjuaje de python.
* **src->python:** Aqui encontramos el main.py hecho por el profesor, el bfs.py que es un archivo un poco más "greedy" en el que se usa el método recursivo para llamar a una función que escoje el último nodo de la lista de nodos y la recorre de manera inversa; y Astar.py que implementa un algorítmo con heurística.
* **results:** Imágenes de los resultados obtenidos y un archivo de excell con información de tiempos, distancias y nodos explorados.

***
### MAIN.PY
Este código lo da el profesor de la asignatura.

### MAIN_PLOT.PY
Este código lo da el profesor de la asignatura. Se ha implementado una parte gráfica en la que se representan los nodos explorados y el tiempo que se tarda en encontrar el nodo meta desde el nodo inical indicado en el README de cada mapa. En este caso se recorre una lista de nodos que siguen unas direcciones determinadas.

 ### BFS_PLOT.PY
Este algorítmo es muy parecido al inicial. La diferencia radica en que se elimina el bucle while y se crea una función que será llamada de manera recursiva y los nodos de la lista de nodos se recorren de manera inversa. el nodo inical y la meta está indicado en el README de cada mapa.  Se ha implementado un algoritmo visual para ver los nodos explorados y el tiempo invertido en ello

### ASTAR_PLOT.PY
En este caso, el algoritmo implementa una heurística en donde se calcula la distancia desde el nodo inicial al nodo meta indicado en el README de cada mapa. De esta forma se elige el siguiente nodo en la lista en funciñon de la distancia más cercana a esa meta. Tambien se ha implementado un algoritmo visual para ver los nodos explorados y el tiempo invertido en ello.

***

#### 1. [COMPARATIVA DE TIEMPOS DE EJECUCIÓN](https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/Comparativa%20de%20tiempos.png)

El tiempo de búsqueda más amplio es el del algoritmo de Astar en parte porque el cálculo de las distancia requiere de mayor tiempo, en el medio encontramos el tiempo del algoritmo main y el que menos tarda es el bfs.
<p algin="center">
    <img src="[https://github.com/Noelia-vera/TFG-Noelia-Fernandez-Talavera/blob/main/Im%C3%A1genes/Robot/Real/Small/niveles.PNG](https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/Comparativa%20de%20tiempos.png)">
</p>

#### 2. [COMPARATIVA DE NODOS EXPLORADOS](https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/Comparativa%20de%20nodos%20explorados.png)

En este caso, el primer algoritmo dado por el profesor es el que más nodos recorre. Esto se debe a que realmente el código recorre los nodos en todas las direcciones definidas hasta encontrar el nodo de la meta. En el caso del Astar el numero de nodos es menor ya que, al calcular la dirección, el código dirige el path al nodo de la meta. Sin embargo, el algorítmo sin heurística más "greedy" que recorre la lista de nodos en orden inverso, en ocasiones es el que menor numero de nodos explora, algo poco normal.

<p algin="center">
    <img src="[https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/Comparativa%20de%20tiempos.png](https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/Comparativa%20de%20tiempos.png)">
</p>

#### 3. [COMPARATIVA DE NODOS EXPLORADOS GRÁFICAMENTE]
##### MAP1 (MAIN-BFS-ASTAR)
<p algin="center">
    <img src="https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/small/Astar_map1.png">
    <img src="https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/small/Astar_map1.png">
    <img src="https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/small/Astar_map1.png">
</p>

#### 4. [ARCHIVO EXCELL COMPARATIVO](https://github.com/Noelia-vera/PathPlanning_RoboticMaster_UC3M/blob/main/results/Path_planning.xlsx)
