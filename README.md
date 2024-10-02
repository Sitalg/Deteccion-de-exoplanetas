# Clasificación de Exoplanetas usando Bósque Aleatorio

Este proyecto implementa un modelo de aprendizaje automático para la clasificación de exoplanetas en exoplanetas confirmados y falsos positivos utilizando el algoritmo de **Bósque Aleatorio (Random Forest)**. Los datos utilizados provienen del archivo público de exoplanetas de la NASA.

## Contenido del Proyecto

- `bosque_aleatorio.ipynb`: Contiene el código completo del análisis, preprocesamiento de datos y la implementación del modelo de Bósque Aleatorio para la clasificación.
- `matriz_confusion.png`: Imagen que representa la matriz de confusión del modelo entrenado.
- `README.md`: Este archivo, que describe el proyecto y proporciona instrucciones para la instalación y ejecución del código.

## Datos

Los datos utilizados en este proyecto fueron obtenidos del archivo público de exoplanetas de la NASA:

- URL de los datos: [Archivo de exoplanetas de la NASA](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/nstedAPI/nph-nstedAPI?table=cumulative&select=kepid,kepoi_name,koi_disposition,koi_period,koi_impact,koi_duration,koi_depth,koi_prad,koi_teq,koi_insol,koi_model_snr&format=csv)

El dataset contiene información clave sobre los exoplanetas, como:
- Disposición planetaria (confirmado, falso positivo)
- Periodo orbital
- Radio planetario
- Temperatura de equilibrio
- Insolación, entre otros.

## Requisitos

Para ejecutar el proyecto, se requiere tener instaladas las siguientes dependencias de Python:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow`

## Bibliotecas utilizadas
- pandas: Para la manipulación y limpieza de datos.
- numpy: Para operaciones numéricas y manejo de arrays.
- matplotlib y seaborn: Para visualización de datos, incluyendo gráficos y la matriz de confusión.
- scikit-learn: Para el preprocesamiento de datos y la implementación del modelo de Bósque Aleatorio.
- tensorflow: (Opcional) para futuros desarrollos con redes neuronales.

## Instrucciones de Uso
1. Clona el repositorio a tu máquina local: git clone https://github.com/usuario/repo_clasificacion_exoplanetas.git
2. Navega a la carpeta del proyecto: cd repo_clasificacion_exoplanetas
3. Instala las dependencias necesarias: pip install -r requirements.txt
4. Ejecuta el notebook: Puedes abrir y ejecutar el notebook bosque_aleatorio.ipynb en Jupyter Notebook o cualquier entorno compatible.

## Resultados
El modelo de Bósque Aleatorio entrenado mostró un rendimiento excelente para la clasificación de exoplanetas confirmados y falsos positivos, con los siguientes resultados:

- Exactitud: 90.81%
- Precisión: 92.83%
- Sensibilidad: 92.29%

La matriz de confusión muestra el rendimiento del modelo con respecto a las predicciones correctas e incorrectas.

## Futuras Mejoras
- Explorar otros algoritmos de clasificación como Gradient Boosting o Redes Neuronales.
- Incluir más características astronómicas en el análisis, como la metalicidad estelar y la excentricidad de la órbita.
- Optimización de hiperparámetros del modelo para mejorar su rendimiento.
