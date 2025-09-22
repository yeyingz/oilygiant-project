# OilyGiant: Predicción de Ubicaciones para Perforación de Pozos Petroleros

## Descripción del Proyecto

Este proyecto tiene como objetivo identificar las ubicaciones más rentables para la perforación de nuevos pozos de petróleo para la empresa OilyGiant. El análisis se llevó a cabo sobre tres regiones de exploración (Región 0, Región 1 y Región 2) para maximizar el beneficio total. Se desarrolló un modelo de **regresión lineal** para predecir el volumen de reservas de petróleo en cada pozo.

La metodología incluyó un riguroso **análisis de riesgo** utilizando la técnica de muestreo **bootstrap**, lo que permitió evaluar la variabilidad del beneficio y la probabilidad de pérdidas en cada región. Finalmente, se seleccionó la región con el mayor potencial de ganancias y el menor riesgo para recomendar la perforación de los 200 pozos más prometedores.

## Estructura del Repositorio

-   `oilygiant_project.ipynb`: Cuaderno de Jupyter que contiene todo el proceso del proyecto, desde el análisis exploratorio de datos hasta la construcción del modelo, la evaluación de beneficios y el análisis de riesgo.
-   `geo_data_0.csv`: Conjunto de datos de la Región 0.
-   `geo_data_1.csv`: Conjunto de datos de la Región 1.
-   `geo_data_2.csv`: Conjunto de datos de la Región 2.
-   `requirements.txt`: Lista de dependencias de Python para la correcta ejecución del proyecto.
-   `informe.md`: Informe final que resume la metodología, los hallazgos clave y las conclusiones del proyecto.
-   `.gitignore`: Archivo de configuración para ignorar directorios y archivos no relevantes para el control de versiones.

## Metodología y Tecnologías

El proyecto fue desarrollado en **Python** utilizando las siguientes librerías:

-   **Pandas y NumPy**: Para la manipulación, limpieza y análisis de los datos.
-   **Scikit-learn**: Para el desarrollo del modelo de regresión lineal, la división de datos y la evaluación del rendimiento del modelo.
-   **Matplotlib y Seaborn**: Para la visualización de datos y resultados.

## Conclusiones Clave

-   El modelo de **regresión lineal** demostró una alta capacidad predictiva para el volumen de reservas en la **Región 1**, con una correlación cercana a 1 entre las predicciones y los valores reales.
-   El análisis de **bootstrap** reveló que la **Región 1** ofrece el mayor beneficio medio estimado y el menor riesgo de pérdidas.
-   Se recomienda a la compañía OilyGiant priorizar la perforación en la **Región 1** para maximizar el retorno de la inversión y mitigar el riesgo financiero.

## Cómo Usar

1.  Clona este repositorio en tu máquina local.
2.  Instala las dependencias necesarias con `pip install -r requirements.txt`.
3.  Abre el cuaderno `oilygiant_project.ipynb` en tu entorno de Jupyter para revisar el código y los análisis.