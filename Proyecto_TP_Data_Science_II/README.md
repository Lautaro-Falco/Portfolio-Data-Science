# 📊 Proyecto Trabajo Practico Data Science II – Análisis de Ventas e Insights de Negocio

Este proyecto fue desarrollado como **trabajo practico del curso Data Science II en CoderHouse**, y también presentado en clase como parte de la instancia de networking y exposición.  

El objetivo fue aplicar un **proceso completo de análisis de negocio** utilizando SQL Server, Python y Power BI para obtener **insights accionables** sobre ventas, clientes y canales de una empresa simulada.

---

## 🗄️ Base de datos utilizada

Se trabajó con la base **AdventureWorksDW2022**, modelo de datos de Microsoft orientado a retail y ventas.

---

## 🛠️ ¿Qué incluye el proyecto?

- **SQL Server**: Extracción, limpieza y preparación de los datos (se entregaron ya listos para el análisis en Python/Power BI).  
- **Python (Colab)**: Análisis de negocio con gráficos y métricas en los puntos 3 al 9 (segmentación, elasticidad, MOS, bundles, forecast, etc.).  
- **Power BI**: Dashboards de los puntos **1 (Ingresos/pedidos/ticket promedio por canal)**, **2 (Rentabilidad por categorías/subcategorías)** y **5 (Cobertura de inventario – MOS)**.  
- **Documentación en Canva** con storytelling visual del proyecto y conclusiones.

---

## 📑 Documentación del Proyecto

Incluye:
- Objetivos del análisis y metodología aplicada.
- Explicación de cada punto (10 entregables) con gráficos y conclusiones.
- Plan de acción a 90 días con KPIs definidos.
- Conclusiones ejecutivas (hallazgos clave).  

📂 Podés ver y descargar toda la documentación completa desde este enlace:  
👉 [Acceder a la carpeta de Google Drive](https://drive.google.com/drive/u/0/folders/1LT9MOvAKBs7QCaih4wtsvXq6vjncAPZ9)


## 📑 Documentación y archivos disponibles

En la carpeta de Google Drive están incluidos todos los recursos del proyecto:

- `queries.sql`: script con todas las consultas en **SQL Server** utilizadas.  
- `pbi_dashboard.pbix`: archivo de **Power BI** con los dashboards de los puntos 1, 2 y 5.  
- `csv/`: carpeta con **todos los datasets exportados** (uno por cada query de los puntos 1 al 10).  
- `consignas.pdf`: enunciado original del trabajo práctico.  
- `documentacion_final.pdf`: entrega final con la **presentación completa en Canva** (storytelling, análisis y conclusiones).  
- `colab_notebook.ipynb`: notebook con el código en **Python/Colab** para los análisis y gráficos de
---

## 📊 Principales Insights

- **Canales**: Internet aporta volumen de pedidos, Resellers lideran en ticket promedio e ingresos.  
- **Clientes**: 4 clusters RFM; el 2 (<2% de clientes) genera la mayor parte del revenue.  
- **Inventario (MOS)**: riesgo de quiebre en SKUs críticos con MOS < 1 mes (cascos, botellas, jerseys).  
- **Bundles**: asociaciones fuertes (neumáticos + cámaras + patch kit, botella + portabotella) con lift >7.  
- **Forecast Q1**: tendencia negativa → necesidad de reforzar promociones e inventario.  

---

## 🧠 Herramientas utilizadas

- SQL Server (AdventureWorksDW2022)  
- Python (Colab, Prophet, Scikit-learn, Pandas, Seaborn, Matplotlib)  
- Power BI  
- Canva  
- GitHub  
