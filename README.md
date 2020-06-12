# EJERCICIO UNSUPERVISED LEARNING
# Carlos Alfonsel (carlos.alfonsel@mbitschool.com)

## 1. Análisis Exploratorio del Dataset (EDA)

- Importación de Librerías y Conjunto de Datos.
- Limpieza Dataset: Estudio Missing Values, Outliers y Correlación.
- Repaso Aprendizaje Supervisado: Comparativa Modelos.

## 2. Clustering y Reducción de Dimensionalidad

- Dendrograma: aplicando PCA, se obtienen 5 clústers.
- K-Means: se realiza una clasificación primero con 5 clústers, y después con 3, comparando los resultados. Se aplica previamente una reducción de dimensionalidad PCA.
- K-Medoids: al igual que en los casos anteriores, se aplica PCA y luego el algoritmo de clasificación.
- EM (Expectation-Maximization).
- DBSCAN (Density-Based Spatial Clustering of Applications with Noise).

**Conclusión**: los mejores resultados se obtienen con un clasificador K-Means o DBSCAN con 5 clústers y reducción de dimensionalidad PCA. Estas 5 agrupaciones se representan en un gráfico 3D para poder apreciarlas mejor.

## 3. SOMs (Self-Organizing Maps)

Se realiza una prueba con esta técnica vista durante las clases.

## 4. Futuras Mejoras

A la hora de interpretar correctamente los clasificadores, y asignarles la etiqueta adecuada, sería interesante realizar lo siguiente:

- Análisis de los centroides: añadiendo la línea de código **kmeans.cluster_centers_**. Da como resultado un *array* con los valores del centroide del clúster.
- Dibujar en los plots los centroides: por comparación se puede asignar de esta manera una etiqueta al clúster (en nuestro caso concreto: A, B, C, D o E).
