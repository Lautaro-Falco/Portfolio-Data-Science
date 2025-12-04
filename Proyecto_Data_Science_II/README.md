# ⏱️ Proyecto Data Science II – Predicción de Ventas mediante Series de Tiempo

Este proyecto fue desarrollado como **entrega final del curso Data Science II en CoderHouse**, aplicando modelos de predicción de series temporales sobre un dataset real de una cadena de cafeterías.

El objetivo principal fue **entender el comportamiento de la demanda** y **predecir ventas futuras**, permitiendo mejorar la planificación operativa y la toma de decisiones comerciales.

---

## 🔗 Acceso al Notebook

Podés ver y ejecutar el notebook completo en Google Colab desde el siguiente enlace:

👉 **Abrir en Google Colab**  
https://colab.research.google.com/drive/1KgvhPQ77wS1InEwpDjgCH8e4rZA10RmC#scrollTo=nF4R6653C3m9

---
## 📌 Objetivos del proyecto

- Analizar patrones temporales: **tendencias**, **estacionalidad** y **picos de consumo**.
- Trabajar con datos diarios de múltiples puntos de venta.
- Preparar el dataset para modelado (resampling, imputación, agregaciones).
- Entrenar modelos de forecasting con:
  - **Prophet**
  - **SARIMAX** (Auto-ARIMA y configuración manual)
- Comparar el rendimiento de los modelos mediante MAE y RMSE.
- Seleccionar el modelo más eficaz para **predicción de corto plazo**.

---

## 🧪 Herramientas y técnicas utilizadas

- **Python** 🐍 (Google Colab)
- Librerías:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`, `plotly`
  - `prophet`, `statsmodels`
- Ingeniería de series de tiempo
- Validación temporal (train/test split)
- Métricas de evaluación:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)

---

## 📈 Comparación Final de Modelos

| Modelo | MAE | RMSE | Resultado |
|--------|-----|------|-----------|
| **Prophet** | 116.35 | 142.89 | ⭐ Mejor rendimiento |
| SARIMAX Auto-ARIMA | 222.19 | 253.48 | ❌ Peor ajuste |
| SARIMAX Manual (1,1,1)x(1,1,1,7) | 124.54 | 147.70 | Buen rendimiento |

**📌 Conclusión:** Prophet resultó ser el modelo más adecuado para este caso, logrando un error aproximado del 6–8% respecto a las ventas típicas de la cadena.

---

## 🧾 Estructura del Proyecto

El trabajo fue desarrollado íntegramente en **Google Colab**, utilizando:

- 1 notebook principal con todo el análisis, modelado y conclusiones:
  - **Data_Science_II_Pronostico_Ventas.ipynb**

- Archivos de datos provistos por la cátedra e importados directamente en el entorno de Colab.

---

## 🔍 Principales Insights del Negocio

- La **estacionalidad semanal** es muy marcada: mayor demanda viernes y fines de semana.
- Varias sucursales presentan **picos operativos críticos** en horario mañana.
- Se identifican bebidas calientes como **top performers** consistentes.
- La tendencia general muestra **crecimiento sostenido** en las ventas.

---

## 📌 Conclusión General

Este proyecto demuestra cómo los modelos de series de tiempo permiten anticipar la demanda y optimizar decisiones comerciales clave, como:

- Gestión de inventarios 🏪
- Planificación de personal 🧑‍🍳
- Estrategias de promociones en días/horarios clave 💡

---

## 👨‍💻 Autor

**Lautaro Falco**  
Estudiante de Ciencia de Datos | Business Analytics | Machine Learning  
📫 Contacto: https://www.linkedin.com/in/lautaro-gabriel-falco/
