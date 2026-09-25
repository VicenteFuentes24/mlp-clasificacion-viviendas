# Evaluación 1 - Fundamentos de Deep Learning

## Integrantes

- Vicente Alonso Fuentes Lagos
- Marlon Gabriel Abreu Galviz

## Descripción

Este proyecto corresponde a la Evaluación 1 de Fundamentos de Deep Learning.

El objetivo es desarrollar una red neuronal artificial multicapa capaz de clasificar viviendas según su rango de valor utilizando seis variables relacionadas con ubicación, antigüedad y entorno.

El precio original de las viviendas es una variable numérica continua. Para trabajar el problema como clasificación, los datos se dividen en tres categorías:

- Bajo
- Medio
- Alto

Posteriormente se implementa una red neuronal MLP utilizando TensorFlow/Keras y se comparan diferentes configuraciones para analizar su rendimiento.

## Archivos del proyecto

- `Deep_Learning_Clasificación_de_viviendas_EV1.ipynb`: cuaderno principal con el desarrollo completo.
- `Real_estate_valuation_USD.xlsx`: dataset utilizado para el entrenamiento y evaluación del modelo.

## Tecnologías utilizadas

- Python
- Google Colab
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Ejecución

Para ejecutar el proyecto:

1. Abrir el archivo `.ipynb` en Google Colab.
2. Subir el archivo `Real_estate_valuation_USD.xlsx` al entorno de Colab.
3. Ejecutar las celdas del cuaderno en orden desde el inicio.
4. Esperar a que finalicen los entrenamientos y experimentos.
5. Revisar las métricas, tablas y gráficos obtenidos.

## Modelo utilizado

Se implementó una red neuronal multicapa o MLP.

La configuración principal utiliza:

- 6 variables de entrada.
- 2 capas ocultas.
- Función de activación ReLU.
- Función de salida Softmax.
- Optimizador SGD.
- Sparse Categorical Crossentropy como función de pérdida.

Durante el desarrollo se realizaron experimentos modificando distintos hiperparámetros, como:

- Cantidad de épocas.
- Learning rate.
- Batch size.
- Funciones de activación.
- Arquitectura de la red.
- Dropout.
- Función de pérdida.

## Evaluación

El rendimiento del modelo se analiza mediante las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-Score
- Matriz de confusión

El modelo obtuvo un rendimiento cercano al 80 % de Accuracy en la evaluación realizada.

## Dataset

Se utilizó el dataset **Real Estate Valuation**, que contiene información relacionada con viviendas, incluyendo variables como antigüedad, distancia a estaciones MRT, cantidad de tiendas cercanas y ubicación geográfica.

Fuente:

UCI Machine Learning Repository - Real Estate Valuation Dataset.

## Conclusión

El proyecto permitió implementar y evaluar una red neuronal MLP para un problema de clasificación multiclase.

Los experimentos permitieron observar cómo diferentes configuraciones e hiperparámetros afectan el rendimiento del modelo y seleccionar una configuración adecuada para clasificar las viviendas en las categorías Bajo, Medio y Alto.