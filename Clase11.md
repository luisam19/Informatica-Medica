# Fecha: 08/03/2022 

## Arboles de decisión

RF es un tipo de Algoritmo de Ensamble en Machine Learning en donde se combinan diferentes árboles y la salida de cada uno se contará como “un voto” y la opción más votada será la respuesta del _Bosque Aleatorio_ (RF).

El RF, al igual que el árbol de decisión, es un modelo de aprendizaje supervisado para clasificación (aunque también puede usarse para problemas de regresión).

Documentación de Sci-Kit Learn: <a href="https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html" target="_blank">RandomForestClassifier</a>

* Es uno de los algoritmos de Ml más potentes y usados en el mundo
* Toma lo mejor de los árboles de decisión
* Ataca la debilidad de los árboles de decisión
* Tiene un sesgo bajo, por tanto tiene errores muy pequeños

Cuándo se realiza pruebas de producción, es difícil ajustar, el algoritmo tiende a overfitting.

Se traza una línea media, para empezar hallar las distancia y encuentra los MSE. Después empieza a iterar. 

## Gran problema de los DT
**Bias vs varianza**

En entrenamiento se comporta muy bien, tiene un bias bajo.
En los datos sde prueba, la varianza es alta. 

Los DT son sensibles a los datos de entrenamiento 
**PROBLEMA**: `Overfitting`

## Solución al problema

Introduciendo dos variables adicionales
1. Agregación:No trabajando con un solo árbol, sino que se trabaja con muchos (cientos árboles)
2. Aleatorización de las muestras. A cada árbol se le pasa un conjunto de muestras, con la finalidad de enriquecer la eficiencia estadística. 
3. A cada árbol se mezcla de forma aleatoria el uso de las características.

### ¿Cómo funciona Random Forest?
1. Se seleccionan las $k$ características (_features_) del total de características del conjunto de datos y se crea un árbol de decisión con esas $k$ características.
2. Se Crean $n$ árboles variando siempre la cantidad de las $k$ características. También se podría variar la cantidad de muestras que pasan a esos árboles (esto es conocido como “bootstrap sample”)
3. Se Toman cada uno de los $n$ árboles y se hace la misma clasificación. Se Guardan el resultado de cada árbol obteniendo $n$ salidas.
4. Se Calculan los votos obtenidos para cada “clase” seleccionada y se considera a la más votada como la clasificación final del “bosque”.


#### Ventajas:
* Tiene buen desempeño -aún- sin ajustar los hiperparámetros.
* Funciona bien para problemas de clasificación y regresión.
* Al utilizar múltiples árboles se reduce el riesgo de overfiting.
* Se mantiene estable con nuevas muestras puesto que al utilizar cientos de árboles sigue prevaleciendo el promedio de sus votaciones.

#### Desjeventajas:
* Si bien tiene menos riesgo de _overfitting_, no es infalible.
* Tiene “costo” computacional alto. Se deben crear y ejecutar cientos de árbol de decisión.
* Requerir más tiempo de entrenamiento (varía según el problema)
* RF no funciona bien con datasets pequeños.
* Difícil poder interpretar los ¿cientos? de árboles creados en el bosque. 


## $Overfitting$ en Machine Learning
Es muy común que en los inicios del aprendizaje en machine learning se caiga en el problema del $Overfitting$. Lo que ocurrirá es que la máquina sólo se ajustará a aprender los casos particulares que le enseñó en el entrenamiento (train) y será incapaz de reconocer nuevos datos de entrada (test).

<img src="img/aprendizaje.png" width="500px">

