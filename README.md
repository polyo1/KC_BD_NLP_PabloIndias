# Análisis de Sentimientos en Reviews de Instrumentos Musicales

Este proyecto se centra en el análisis de sentimientos de un conjunto de datos de reviews de instrumentos musicales obtenidos de Amazon. El objetivo es desarrollar un modelo que pueda predecir si una review es positiva o negativa.

## Dataset

El dataset utilizado es "reviews_Musical_Instruments_5.json.gz", que contiene más de 10.000 reviews de instrumentos musicales. Cada review incluye información como el ID del usuario, el ID del producto, la puntuación (de 1 a 5 estrellas), el texto de la review, etc.

## Exploración de Datos

Se realizó un análisis exploratorio de los datos para obtener información relevante, incluyendo:

* **Cardinalidad del vocabulario:** Se calculó el número de palabras únicas en el dataset.
* **Distribución de reviews por número de estrellas:** Se analizó la frecuencia de cada puntuación.
* **Nº de reviews positivas y negativas:** Se clasificaron las reviews en positivas (4 o 5 estrellas) y negativas (1, 2 o 3 estrellas) y se contabilizó la cantidad de cada una.
* **N-grams más frecuentes:** Se identificaron los conjuntos de palabras más comunes en las reviews.
* **Nubes de palabras:** Se generaron nubes de palabras para visualizar las palabras más relevantes.

## Preprocesamiento de Texto

Se realizó un preprocesamiento del texto de las reviews para preparar los datos para el modelado, incluyendo:

* **Tokenización:** Se dividió el texto en palabras individuales (tokens).
* **Eliminación de stop words:** Se eliminaron palabras comunes que no aportan información relevante (como "el", "la", "un", etc.).
* **Lematización:** Se redujeron las palabras a su forma base (lema).

## Modelado

Se utilizaron diferentes algoritmos de aprendizaje automático para entrenar modelos de clasificación, incluyendo:

* **Regresión Logística**
* **Máquinas de Vectores de Soporte (SVM)**

Se evaluó el rendimiento de los modelos utilizando métricas como la precisión, la exhaustividad y la puntuación F1.

## Resultados

Se obtuvieron resultados prometedores en la clasificación de reviews, con una precisión superior al 90%. Se observó que el modelo Random Forest tuvo el mejor rendimiento en general.

