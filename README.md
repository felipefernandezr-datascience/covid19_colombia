# 🦠 COVID-19 en Colombia: Análisis Exploratorio y Visualización de Datos

## 📝 Descripción del Proyecto
Este repositorio contiene un análisis exhaustivo del impacto del COVID-19 en Colombia, utilizando técnicas de Ciencia de Datos para procesar, limpiar y visualizar los registros oficiales de contagios y decesos. El estudio abarca desde la macrotendencia nacional hasta el comportamiento local en el departamento de Antioquia y su capital, Medellín. 

A través de tres fases de desarrollo, este proyecto responde preguntas críticas sobre la tasa de letalidad, los tiempos de atención hospitalaria y la distribución demográfica del virus, demostrando estadísticamente hitos epidemiológicos como el colapso hospitalario de 2021 y el éxito del Plan Nacional de Vacunación frente a la variante Ómicron en 2022.

---

## 📂 Estructura del Repositorio

El análisis se divide en tres Jupyter Notebooks principales, reflejando el ciclo de vida completo de un proyecto de datos:

* **`01_exploratory_analysis.ipynb`:** Validación inicial de la base de datos, perfilado (Data Profiling) y exploración univariada para comprender la estructura original de los registros de salud.
* **`02_data_cleaning.ipynb`:** Fase de preprocesamiento y Feature Engineering. Incluye la estandarización de columnas, tratamiento de valores nulos, eliminación de outliers (edades atípicas), cálculo de tasas de letalidad y análisis de las diferencias en días (retrasos) entre el inicio de síntomas, el diagnóstico y la recuperación.
* **`03_data_visualization.ipynb`:** Análisis visual profundo. Utiliza gráficos de series de tiempo, densidad (KDE), matrices de correlación (Pairplots) y cuadrículas de facetas (FacetGrids) para extraer conclusiones demográficas y epidemiológicas.

---

## 📊 Hallazgos Principales

1. **El Éxito de la Vacunación (Desacoplamiento Estadístico):** Al cruzar las curvas temporales, se evidenció que la tercera ola (mediados de 2021) fue la más letal, colapsando el sistema de salud. Sin embargo, el pico de enero de 2022 (variante Ómicron) registró el máximo histórico de contagios, pero una tasa de mortalidad mínima, demostrando visualmente la efectividad de las vacunas.
2. **Brecha de Género y Edad:** El análisis multivariado mediante FacetGrids comprobó que, aunque hombres y mujeres se contagiaron en proporciones casi idénticas, el virus tuvo una tasa de letalidad significativamente mayor en la población masculina. Así mismo, se confirmó que el riesgo de mortalidad se dispara exponencialmente a partir de los 60 años.
3. **Tiempos de Evolución y COVID Prolongado:** La ingeniería de características sobre las fechas permitió identificar una distribución bimodal en los tiempos de diagnóstico (pacientes atendidos rápidamente vs. pacientes con largas esperas) y evidenció estadísticamente la existencia de recuperaciones atípicamente largas (>100 días), asociadas a estancias en UCI y *Long COVID*.

---

## 🛠️ Tecnologías y Herramientas Utilizadas

* **Lenguaje:** Python 3
* **Manipulación y Limpieza de Datos:** Pandas
* **Visualización de Datos:** Matplotlib, Seaborn
* **Entorno de Desarrollo:** Jupyter Notebook

---
*Proyecto desarrollado como portafolio de análisis de datos y visualización avanzada.*
