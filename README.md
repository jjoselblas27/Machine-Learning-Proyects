# Machine-Learning-Proyects
Recopilatorio de Proyectos realizados en el transcurso del curso Machine learning en UTEC.

## Clasificacion
objetivo la aplicación de los algoritmos de SVM (Support vector machine), KNN (K-nearest neighbors), regresión logística y árboles de decisión para clasificar un dataset de imágenes de mariposas.

Se separo un 70 % de datos para el entrenamiento, un 15 % para la validación usando K-Fold Cross Validation o Bootstrap y un 15 % para el testeo de los modelos.

Se concluye que una parte crucial al momento de realizar el experimento fue trabajar con un conjunto de vectores característicos que provengan de imágenes con la menor cantidad de ruido. El eliminar el fondo y redimensionarlas influyó enormemente en la precisión de los modelos.

Los modelos de KNN y regresión logística fueron los que tuvieron una eficiencia y resultados superiores al promedio, y parecen ser los más óptimos para la clasificación de imágenes.

Sin embargo, se establece la necesidad de generar modelos que reconozcan el ruido y en los cuales su aporte y significancia sea mínima, con el objetivo de aumentar la precisión. Todos los modelos implementados carecen de esta propiedad, lo que condujo a una investigación acerca de la forma de generar los vectores de tal manera que no se pierda la información.

## Clustering

En este estudio, empleamos técnicas avanzadas para explorar y analizar nuestros datos de manera exhaustiva. Comenzamos aplicando la técnica de reducción de dimensionalidad SVD para transformar nuestros datos complejos en un espacio dimensional más manejable. Luego, implementamos tres algoritmos de clustering ampliamente reconocidos: K-Means, DBSCAN y GMM. Utilizamos métricas objetivas como el coeficiente de Silhouette, Rand Index y Mutual Information Score para evaluar y comparar la calidad de los clusters generados por cada algoritmo. Los resultados revelaron patrones y estructuras clave en nuestros datos, proporcionando información esencial para la toma de decisiones informadas.

Con respecto a los resultados de las métricas de clustering, el mejor método para el conjunto de datos utilizados fue el K-Means. Si bien en los resultados de NMI las tres técnicas lograron resultados superiores al 0.8, se necesita un análisis más amplio para mejorar su aplicación.

## Multilayer Perceptron

En este proyecto, hemos explorado la aplicación del Perceptrón Multicapa (MLP) para la clasificación de tumores mamarios utilizando un conjunto de datos que comprende información detallada de 569 pacientes. Nuestra investigación se ha centrado en la diferenciación entre tumores benignos y malignos, una tarea crucial para la detección temprana y el tratamiento efectivo del cáncer de mama.

Los experimentos realizados han demostrado la eficacia de MLP en la clasificación de tumores, alcanzando un 98 por ciento de precisión. La capacidad del modelo para aprender patrones complejos a partir de características de los pacientes destaca su utilidad en el ámbito médico.

Se puede notar que existen redes neuronales de mayor profundidad que son más complejas que la MLP. Para esto sería una buena opción probar con LSTM o CNNs, las cuales funcionan mejor para las imágenes médicas. Además, cuando se utilizan muchas capas ocultas, el modelo MLP muestra una tendencia al sobreajuste. Para esto existen técnicas para regularizar, como por ejemplo, Weight Decay.

La comparación de diferentes funciones de activación, ajuste de parámetros, hiperparámetros y análisis de resultados ha proporcionado valiosos insights sobre la influencia de estos aspectos en el rendimiento del modelo. La robustez del MLP para adaptarse a la complejidad de los datos de tumores mamarios subraya su potencial para mejorar los sistemas de diagnóstico existentes.

Para finalizar, se realizaron diversos ajustes a los hiperparámetros del modelo con el objetivo de mejorar el performance, lo cual brindó una visión de mayor alcance sobre el funcionamiento de este tipo de redes neuronales. Cabe resaltar que es importante realizar un análisis previo de posibles sesgos en el conjunto de datos, ya que este puede presentar existencia de sesgos que afectarían el rendimiento de nuestro modelo.
