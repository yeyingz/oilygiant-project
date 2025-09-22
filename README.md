# OilyGiant Extracción de Petróleo

**Descripción del proyecto:**

Este proyecto se centra en encontrar los lugares más rentables para perforar nuevos pozos de petróleo para la compañía OilyGiant. El objetivo es identificar las 200 mejores ubicaciones en tres regiones diferentes (Región 0, Región 1 y Región 2) para maximizar el beneficio total. Para ello, se ha desarrollado un modelo de regresión lineal para predecir el volumen de reservas en nuevos pozos. El análisis de riesgo y el cálculo del beneficio potencial se realizaron mediante la técnica de muestreo **bootstrap**, para asegurar la solidez de las conclusiones.

**Archivos del proyecto:**

* `oilygiant_project.ipynb`: El cuaderno de Jupyter que contiene todo el código, el análisis de datos, la construcción del modelo, la evaluación de beneficios y el análisis de riesgos.
* `geo_data_0.csv`: Datos de la Región 0.
* `geo_data_1.csv`: Datos de la Región 1.
* `geo_data_2.csv`: Datos de la Región 2.
* `README.md`: Descripción general del proyecto.
* `requirements.txt`: Lista de las librerías de Python necesarias para ejecutar el proyecto.
* `.gitignore`: Archivo para excluir directorios y archivos no deseados de Git.
* `informe.md`: Un informe final que resume los hallazgos y conclusiones clave.

**Tecnologías y librerías utilizadas:**

* **Python**
* **pandas**: Para la manipulación y análisis de datos.
* **numpy**: Para operaciones numéricas, especialmente en el muestreo bootstrap.
* **matplotlib.pyplot** y **seaborn**: Para la visualización de datos.
* **sklearn.linear_model.LinearRegression**: Para la creación del modelo predictivo.
* **sklearn.model_selection.train_test_split**: Para dividir los datos en conjuntos de entrenamiento y prueba.
* **sklearn.metrics.mean_squared_error**: Para evaluar el rendimiento del modelo.

**Conclusión:**

El proyecto concluye que la **Región 1** es la más prometedora para la perforación, con el mayor beneficio potencial y un riesgo de pérdidas bajo, validado por un análisis de riesgo y variabilidad por **bootstrapping**.