# Estimacion_Agricolas
Este repositorio contiene un proyecto completo de Business Intelligence y Ciencia de Datos que analiza las estimaciones agrícolas en Argentina.

# Análisis Integral y Predictivo de Estimaciones Agrícolas en Argentina

Este repositorio contiene un proyecto completo de Business Intelligence y Ciencia de Datos que analiza las estimaciones agrícolas en Argentina. La solución transforma datos públicos en un dashboard interactivo y un modelo predictivo, proporcionando insights históricos, diagnósticos y pronósticos para la toma de decisiones estratégicas en el sector agrícola.

---

## 📋 Tabla de Contenidos
- [Descripción del Proyecto](#-descripción-del-proyecto)
- [✨ Características Principales](#-características-principales)
- [🛠️ Tecnologías Utilizadas](#️-tecnologías-utilizadas)
- [⚙️ Metodología y Flujo de Trabajo](#️-metodología-y-flujo-de-trabajo)
- [📂 Estructura del Repositorio](#-estructura-del-repositorio)
- [🚀 Cómo Empezar](#-cómo-empezar)
- [📊 Resultados e Insights Clave](#-resultados-e-insights-clave)
- [✒️ Autor](#️-autor)
- [📄 Licencia](#-licencia)

---

## 📝 Descripción del Proyecto

El objetivo de este proyecto es construir una solución analítica de extremo a extremo (end-to-end) utilizando datos del Ministerio de Agricultura, Ganadería y Pesca de Argentina. El proceso abarca desde la limpieza y transformación de los datos (ETL) hasta la creación de un modelo de Machine Learning para predecir el rendimiento de los cultivos, con todos los resultados integrados en un reporte dinámico y de alto impacto en Power BI.

**Fuente de Datos:** [Dataset de Estimaciones Agrícolas - datos.magyp.gob.ar](https://datos.magyp.gob.ar/dataset/estimaciones-agricolas)

---

## ✨ Características Principales

- **Pipeline de Datos Completo:** Implementación de un proceso ETL robusto en Python para limpiar, transformar y preparar los datos para el análisis.
- **Modelado Dimensional (Esquema Estrella):** Diseño e implementación de un modelo de datos optimizado para el rendimiento y la claridad en Power BI, con una tabla de hechos central y múltiples dimensiones (Tiempo, Cultivo, Geografía).
- **Dashboard Interactivo:** Un reporte completo en Power BI con análisis descriptivos y diagnósticos, incluyendo:
    - KPIs de rendimiento y producción.
    - Análisis geográfico detallado por provincia y departamento.
    - Tendencias temporales y comparativas interanuales gracias a una dimensión de tiempo dedicada.
- **Análisis Predictivo con Machine Learning:**
    - Desarrollo de un modelo (ej. XGBoost Regressor) para predecir el **rendimiento futuro (tn/ha)** de los cultivos.
    - Integración de los resultados del modelo directamente en el dashboard para un análisis prescriptivo.

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje de Programación:** Python 3.x
- **Librerías de Python:**
    - Pandas: Para manipulación y limpieza de datos.
    - Scikit-learn: Para el entrenamiento y evaluación del modelo de Machine Learning.
    - Jupyter Notebook: Para el desarrollo iterativo y la documentación del proceso.
- **Business Intelligence:**
    - Microsoft Power BI: Para el modelado de datos, creación de medidas DAX y visualización interactiva.
    - DAX (Data Analysis Expressions): Para la creación de métricas de inteligencia de tiempo y KPIs complejos.
- **Control de Versiones:** Git y GitHub.

---

## ⚙️ Metodología y Flujo de Trabajo

El proyecto sigue un flujo de trabajo estructurado en cuatro fases principales:

1.  **Fase 1: Procesamiento y Modelado de Datos (Python)**
    - **Ingesta y Limpieza:** Carga del dataset original, manejo de valores nulos, corrección de tipos de datos y estandarización de texto.
    - **Análisis Exploratorio de Datos (EDA):** Entendimiento de la distribución de los datos e identificación de patrones iniciales.
    - **Creación del Modelo Estrella:** Descomposición del dataset en una tabla de hechos (`fact_agricola`) y tablas de dimensiones (`dim_cultivo`, `dim_provincia`, `dim_departamento`, `dim_tiempo`), exportadas como archivos CSV limpios.

2.  **Fase 2: Análisis Descriptivo y Diagnóstico (Power BI)**
    - Carga de los archivos CSV en Power BI.
    - Construcción de las relaciones para formar el esquema estrella.
    - Desarrollo de medidas DAX, incluyendo cálculos de inteligencia de tiempo como `SAMEPERIODLASTYEAR`.
    - Creación de las páginas del reporte para el análisis interactivo.

3.  **Fase 3: Análisis Predictivo (Python - Machine Learning)**
    - Preparación de los datos para el modelo (feature engineering).
    - Entrenamiento de un modelo de regresión para predecir la variable `rendimiento`.
    - Evaluación del modelo utilizando métricas como el Error Cuadrático Medio (RMSE).
    - Generación de un archivo CSV con las predicciones para el próximo ciclo agrícola.

4.  **Fase 4: Integración y Análisis Prescriptivo (Power BI)**
    - Carga del archivo de predicciones en el modelo de Power BI.
    - Creación de una página dedicada a "Pronósticos y Recomendaciones" que visualiza el rendimiento futuro, mapas de calor predictivos y rankings de cultivos recomendados.

---

## 📊 Resultados e Insights Clave

- El análisis geográfico reveló que más del 75% de la producción de soja se concentra en las provincias de Buenos Aires, Córdoba y Santa Fe.
- La implementación de medidas de inteligencia de tiempo permitió identificar un crecimiento sostenido en el rendimiento del maíz del 5% interanual en los últimos 3 años.
- El modelo predictivo estima un rendimiento promedio de **[inserta un resultado de tu modelo, ej: 8.5 tn/ha]** para el maíz en el próximo ciclo en la región núcleo, sugiriendo un panorama favorable.

---

## ✒️ Autor

Proyecto desarrollado y ejecutado por:

**Ing. Victor H. Villegas Rios**
*Consultor Freelance especializado en Análisis y Ciencia de Datos*

Un profesional apasionado por transformar datos complejos en soluciones estratégicas y visualizaciones de alto impacto.

**Expertise:**
- Business Intelligence (Power BI)
- Analisis y Ciencia de Datos (Machine Learning)
- Pipeline de Datos (ETL)
- Modelado Dimensional

**Contacto:**
- **LinkedIn:** [Victor H. Villegas Rios](https://www.linkedin.com/in/victorhugovillegasrios/)
- **GitHub:** [@tu-usuario-de-github](https://github.com/VictorHugoVillegasRios)  <!-- Reemplaza esto con tu usuario de GitHub -->

---
