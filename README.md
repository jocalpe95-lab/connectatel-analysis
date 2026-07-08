# ConnectaTel - Análisis Exploratorio de Datos

##  Objetivo del proyecto
Analizar el comportamiento de uso y las características demográficas de los usuarios de ConnectaTel, integrando datos de planes, perfiles de usuario y consumo (llamadas y mensajes), con el fin de identificar segmentos de clientes, detectar problemas de calidad de datos y generar recomendaciones accionables para el negocio.

##  Datasets utilizados
- `plans.csv`: información sobre los planes ofrecidos (Básico, Premium).
- `users_latam.csv`: datos demográficos de los usuarios (edad, ciudad, plan, fechas de registro/baja).
- `usage.csv`: registros de uso individual (mensajes y llamadas) por usuario.

##  Etapas del análisis
1. **Carga y exploración inicial** de los tres datasets.
2. **Combinación de datasets**: agregación de `usage` por usuario y merge con `users`.
3. **Estadística descriptiva** de variables numéricas (edad, mensajes, llamadas, minutos) y categóricas (plan).
4. **Visualización de distribuciones**: histogramas por variable, segmentados por tipo de plan.
5. **Detección de outliers**: boxplots y método IQR para identificar valores extremos.
6. **Detección de un valor sentinela (`-999`)** en la columna `age`, tratado como dato faltante.
7. **Segmentación de clientes**: por nivel de uso (`grupo_uso`) y por edad (`grupo_edad`).
8. **Visualización de segmentos** y análisis ejecutivo con hallazgos y recomendaciones.

##  Cómo ejecutar el notebook
1. Clona este repositorio o descarga el archivo `.ipynb`.
2. Abre el notebook en [Google Colab](https://colab.research.google.com/) o en Jupyter local.
3. Asegúrate de tener instaladas las librerías: `pandas`, `numpy`, `matplotlib`, `seaborn`.
4. Sube los archivos `plans.csv`, `users_latam.csv` y `usage.csv` al mismo entorno (o ajusta las rutas de carga según corresponda).
5. Ejecuta las celdas en orden, de arriba hacia abajo.

##  Guía de reproducción
El notebook está organizado en pasos secuenciales (Paso 1 a Paso 8). Cada sección incluye:
- Instrucciones del ejercicio en celdas de markdown.
- Código de análisis en celdas ejecutables.
- Insights escritos tras cada visualización o resumen relevante.

## Autor
Camilo Alvarez — Proyecto desarrollado como parte del bootcamp de Análisis de Datos en TripleTen (Sprint 7).
