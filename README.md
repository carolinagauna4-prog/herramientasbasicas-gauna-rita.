# Análisis de catálogo de Netflix

**Autor:** Gauna Rita Carolina 
**Curso:** Herramientas básicas para el Análisis de Datos  
**Fecha:** 8/8/2026

## Objetivo del proyecto
Este proyecto analiza la evolución del catálogo de Netflix a través del tiempo, explorando la distribución de tipos de contenido (películas vs. series), los géneros más frecuentes, los países con mayor producción y la tendencia de estrenos por año.

La pregunta principal que guía el análisis es:  
**¿Cómo ha evolucionado el catálogo de Netflix en términos de tipos de contenido, géneros y países de producción?**

## Dataset

El dataset utilizado proviene de Kaggle: **Netflix Movies and TV Shows**.  
**Enlace:** [https://www.kaggle.com/datasets/shivamb/netflix-shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)

**Características:**
- **Registros:** 8,807 títulos.
- **Columnas:** 12 variables (show_id, type, title, director, cast, country, date_added, release_year, rating, duration, listed_in, description).
- **Fuente:** Kaggle (dominio público para fines educativos).

## Pasos realizados

### 1. Ingesta y limpieza de datos
- Se cargó el dataset en Python (Google Colab) con pandas.
- Se auditaron y trataron valores nulos en columnas clave (director, cast, country, rating, date_added, duration).
- Se estandarizaron formatos: fechas (date_added) y nombres de columnas (minúsculas y sin espacios).

### 2. Exploración y visualización (Python)
- Se generaron 5 gráficos con matplotlib y seaborn:
  - Distribución de películas vs. series.
  - Top 10 géneros más frecuentes.
  - Evolución de estrenos por año.
  - Top 10 países con más contenido.
  - Distribución de duración de películas.
- Cada gráfico fue acompañado de una interpretación breve.

### 3. Construcción de KPIs
Se definieron 3 indicadores clave:
- **Porcentaje de películas vs. series** (aprox. 70% películas).
- **Top 3 géneros más comunes** (Dramas, Comedias, Documentales).
- **Año con más estrenos** (2020, con más de 1,500 títulos agregados).

### 4. Dashboard en Power BI
Se construyó un dashboard interactivo con:
- **3 tarjetas de KPIs** (total de títulos, año pico, % de películas).
- **4 gráficos visuales** (películas vs. series, estrenos por año, top países, top géneros).
- **3 filtros interactivos** (año, tipo de contenido, país).

## Enlaces

- **Dataset fuente:** [Netflix Movies and TV Shows - Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **Notebook:** [Ver en GitHub](enlace-a-tu-notebook)  
- **Dashboard:**<img width="759" height="432" alt="image" src="https://github.com/user-attachments/assets/5261238e-8ad3-4331-a270-73ec69026869" />
<img width="768" height="443" alt="image" src="https://github.com/user-attachments/assets/ec488af0-7120-43c8-9ee1-7b8ea817c2d8" />

## Conclusión

El análisis confirma que el catálogo de Netflix está dominado por películas (≈70%), con un crecimiento exponencial de estrenos a partir de 2010 y un pico en 2020. Estados Unidos es el principal productor de contenido, y los géneros más frecuentes son Dramas, Comedias y Documentales. Este proyecto integra herramientas de Python (pandas, matplotlib, seaborn) y Power BI, y está publicado en GitHub para su trazabilidad y reproducibilidad.
