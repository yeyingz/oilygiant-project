# Informe Final - OilyGiant: Selección de Pozos de Petróleo

**Resumen Ejecutivo:**

El objetivo principal de este proyecto era determinar la región más rentable para la perforación de nuevos pozos de petróleo. Se analizaron datos de tres regiones (Región 0, Región 1 y Región 2) y se utilizó un modelo de **regresión lineal** para predecir el volumen de reservas de petróleo. La selección final de las ubicaciones se basó en el potencial de beneficio, evaluado a través de un riguroso análisis de riesgo con la técnica de **bootstrap**.

**Análisis de Datos:**

Se cargaron y examinaron los conjuntos de datos de las tres regiones. Cada conjunto contenía 100,000 entradas sin valores nulos ni duplicados, lo que garantizó la calidad de los datos para el análisis. Las características `f0`, `f1`, `f2` y la columna `product` se utilizaron para el modelado predictivo.

**Modelado y Predicción:**

Se entrenó un modelo de regresión lineal para cada región, utilizando las características `f0`, `f1` y `f2` para predecir el `product` (volumen de reservas).

* **Región 0:** El modelo tuvo un rendimiento moderado.
* **Región 1:** El modelo mostró un rendimiento excelente, con una predicción de `product` que se correlaciona casi perfectamente con los valores reales, lo que sugiere que las características `f0`, `f1` y `f2` están altamente correlacionadas con el volumen de reservas en esta región.
* **Región 2:** El modelo tuvo un rendimiento moderado, similar al de la Región 0.

**Análisis de Riesgo y Beneficio:**

Utilizando la técnica de bootstrapping, se evaluaron 200 pozos en cada región para estimar el beneficio total y el riesgo de pérdidas. El umbral de beneficio para cada pozo se estableció en 111.1 mil barriles de petróleo, basado en los costos de perforación y desarrollo.

* **Región 0:** Presenta un beneficio potencial significativo, pero también un riesgo de pérdidas considerable.
* **Región 1:** Arroja el beneficio medio más alto de las tres regiones. Su riesgo de pérdida es el más bajo.
* **Región 2:** El beneficio medio es comparable al de la Región 0, pero con un riesgo de pérdida menor.

**Recomendación Final:**

Con base en el análisis de riesgo y el beneficio potencial, se recomienda que la compañía OilyGiant proceda con la perforación de los 200 nuevos pozos en la **Región 1**. Esta región ofrece la mayor probabilidad de éxito financiero y el menor riesgo de pérdidas.

**Áreas para Seguir Investigando:**

* Considerar modelos de aprendizaje automático más complejos como **Random Forest** o **Gradient Boosting** para ver si se pueden obtener predicciones más precisas en las regiones 0 y 2.
* Explorar técnicas de **optimización de código** para mejorar la eficiencia del proceso de simulación bootstrap.
