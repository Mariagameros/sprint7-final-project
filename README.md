# sprint7-final-project

# Análisis de Clientes – ConnectaTel

## 🎯 Objetivo del Proyecto

Como analista de datos, el objetivo de este proyecto es evaluar el comportamiento de los clientes de una empresa de telecomunicaciones en Latinoamérica, ConnectaTel, utilizando información registrada hasta el año 2024.

A través de este análisis se busca:

- Explorar, limpiar y analizar los datos disponibles.
- Construir un perfil estadístico de los clientes.
- Detectar comportamientos atípicos (outliers).
- Crear segmentos de clientes basados en edad y nivel de uso.
- Identificar patrones de consumo.
- Diseñar estrategias de retención.
- Proponer mejoras en los planes actuales.

💡 El proyecto sigue un enfoque programático, definiendo:

- Qué métricas analizar.
- En qué orden ejecutar los pasos.
- Qué decisiones de negocio se pueden derivar de cada hallazgo.

---

## 📁 Datasets Utilizados

Se trabajó con tres datasets principales:

### 1️⃣ plans.csv

Contiene información sobre los planes ofrecidos por ConnectaTel:

- Precio mensual
- Minutos incluidos
- GB incluidos
- Costo por consumo adicional

### 2️⃣ users.csv

Información demográfica y contractual de los clientes:

- Edad
- Ciudad
- Fecha de registro
- Plan contratado
- Fecha de cancelación (churn)

### 3️⃣ usage.csv

Detalle del uso real de los servicios:

- Llamadas realizadas
- Minutos consumidos
- Mensajes enviados
- Tipo de servicio
- Fecha de uso

---

## 🔎 Etapas del Análisis

### Paso 1: Carga y Exploración Inicial

- Importación de librerías.
- Carga de los tres datasets.
- Revisión de estructura (.info(), .head(), .describe()).
- Identificación preliminar de inconsistencias.

### Paso 2: Identificación de Problemas de Calidad de Datos

- Detección de valores nulos.
- Análisis del porcentaje de datos faltantes.
- Evaluación del impacto potencial en el análisis.

### Paso 3: Detección de Valores Inválidos y Sentinels

- Revisión de fechas incorrectas o incoherentes.
- Validación de rangos lógicos en variables numéricas.
- Identificación de valores artificiales o placeholders.

### Paso 4: Limpieza y Mejora de Calidad de Datos

- Tratamiento de valores nulos (eliminación o transformación).
- Conversión de tipos de datos.
- Creación de variables derivadas (segmentos por edad y nivel de uso).
- Transformación de churn a variable binaria.

### Paso 5: Análisis Estadístico

- Estadísticas descriptivas (media, mediana, percentiles).
- Detección de outliers mediante IQR.
- Análisis de distribución de consumo.
- Cálculo de métricas clave (ej. ARPU).

### Paso 6: Visualización

- Distribución por grupos de edad.
- Segmentación por nivel de uso.
- Análisis de outliers.
- Cruce entre edad y consumo.
- Visualización de patrones de comportamiento.

### Paso 7: Insights y Recomendaciones

- Identificación de segmentos más valiosos.
- Detección de usuarios intensivos.
- Evaluación de riesgo de churn.
- Propuestas de mejora en la estructura de planes.
- Estrategias de retención y upselling.

  ## Ejecutar el Proyecto en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](URL_DEL_NOTEBOOK_EN_GITHUB)

O:

1. Abre el archivo `.ipynb` en GitHub.
2. Haz clic en **Open in Colab**.
3. Ejecuta todas las celdas en orden.

---

## 📘 Cómo reproducir el análisis

1. Abre el notebook principal: `notebooks/connectatel_analysis.ipynb`
2. Asegúrate de que los archivos:
   - `plans.csv`
   - `users.csv`
   - `usage.csv`
   estén en la carpeta `/data/` o súbelos manualmente al entorno.
3. Ejecuta las celdas en orden secuencial.
4. Verifica que se creen correctamente las variables derivadas:
   - `grupo_edad`
   - `grupo_uso`
   - `is_churn`
5. Revisa las visualizaciones y conclusiones al final del notebook.

---

## 🧠 Objetivo del análisis

- Identificar problemas de calidad de datos.
- Construir un pipeline de limpieza reproducible.
- Detectar valores inválidos y comportamientos atípicos (outliers).
- Analizar patrones de consumo en llamadas y mensajes.
- Crear segmentos de clientes por edad y nivel de uso.
- Evaluar riesgo de churn.
- Generar insights estratégicos para mejorar la oferta de planes de ConnectaTel.
