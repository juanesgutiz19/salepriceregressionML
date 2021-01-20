# Predicción del precio de una casa a través de técnicas de machine learning
El presente trabajo es un proyecto realizado para la materia Modelos de Sistemas 2 de la Universidad de Antioquia, fue un gran reto en la fase del data cleaning, además las condiciones del dataset no eran las más favorables debido a la gran cantidad de variables y las pocas muestras con las que se contaba. 

Todos los notebooks están distribuidos en las siguientes carpetas: 

* **Experimentos:** Contiene los notebooks relacionados a los experimentos realizados inicialmente para la selección del mejor conjunto de hiperparámetros y así seleccionar los tres mejores modelos.
* **Análisis individual de Características:** Contiene el notebook que incluye el algoritmo empleado para la selección de variables candidatas a eliminar.
* **Selección de Características:** Contiene los notebooks necesarios para el proceso de selección de características usando como criterio de selección el modelo Gradient Boosting.
* **Extracción de Características:** Contiene los notebooks necesarios para el proceso de extracción de características a través del análisis de componentes principales (PCA).

Cabe aclarar que en cada carpeta se encuentra una carpeta llamada *datasets* que contiene los datasets necesarios para la correcta ejecución de los notebooks. A continuación se explicarán los notebooks por carpeta, se presentan en el orden en que deberían ser ejecutados.

## Carpeta: Experimentos
### Notebook: ProyectoDeSemestre RL-RF
contiene las diferentes corridas para la selección del mejor conjunto de hiperparámetros de los modelos Regresión Lineal y Random Forest.
### Notebook: ProyectoDeSemestre GB, RN, SVR
Contiene las diferentes corridas para la selección del mejor conjunto de hiperparámetros de los modelos Gradient Boosting, Redes Neuronales y Maquinas de vectores de soporte.
### Notebook: ProyectoDeSemestre VP
Contiene las diferentes corridas para la selección del mejor conjunto de hiperparámetros del modelo Ventana de Parzen.

## Carpeta: Análisis individual de Características
### Notebook: ProyectoDeSemestre - Análisis individual de características
En el notebook se determina qué variables son candidatas a ser eliminadas a través de las medidas de correlación de Pearson y Point-biserial. 
## Carpeta: Selección de Características
### Subcarpeta: 250
#### Notebook: Sequential Backward Selection - Wrapper 250
Incluye la implementación de la búsqueda secuencial hacia atrás por medio de la librería mlxtend, con la función SecuentialFeatureSelector (SFS), pasando como parámetro 250, que es el número de variables que se deben quedar en el modelo.
#### Notebook: ProyectoDeSemestre Seleccion de características (250) - GB, RF, VP
En el notebook se evalúa el desempeño que tienen los modelos ganadores con las 250 características seleccionadas.
### Subcarpeta: 280
#### Notebook: Sequential Backward Selection - Wrapper
Incluye la implementación de la búsqueda secuencial hacia atrás por medio de la librería mlxtend, con la función SecuentialFeatureSelector (SFS), pasando como parámetro 280, que es el número de variables que se deben quedar en el modelo.
#### Notebook: ProyectoDeSemestre Seleccion de características (280) - GB, RF, VP
En el notebook se evalúa el desempeño que tienen los modelos ganadores con las 280 características seleccionadas.

## Carpeta: Extracción de Características
### Notebook: ProyectoDeSemestre PCA - GB
Contiene resultados del modelo Gradient Boosting tras aplicar la técnica PCA al conjunto de datos.
### Notebook: ProyectoDeSemestre PCA - RF
Contiene resultados del modelo Gradient Boosting tras aplicar la técnica PCA al conjunto de datos.
### Notebook: ProyectoDeSemestre PCA - VP
Contiene resultados del modelo Gradient Boosting tras aplicar la técnica PCA al conjunto de datos.
