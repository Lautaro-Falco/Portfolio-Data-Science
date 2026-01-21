# 🚗 Proyecto Data Science III – Análisis de Sentimiento en Uber Reviews

Este proyecto fue desarrollado como **entrega final de la Diplomatura en Data Science**, aplicando técnicas avanzadas de **Procesamiento de Lenguaje Natural (NLP)** y **Deep Learning** para interpretar la experiencia de los usuarios de Uber en EE.UU.

El objetivo principal fue construir una **Red Neuronal Artificial** capaz de leer una reseña escrita y predecir automáticamente la calificación (estrellas) que dio el usuario.

---

## 🔗 Acceso al Proyecto

Puedes visualizar el notebook completo con todo el código y análisis, o acceder a los datos originales:

* 👉 **[Abrir Notebook en Google Colab](TU_LINK_DE_COLAB_AQUI)**
* 👉 **[Ver Dataset en Kaggle](https://www.kaggle.com/datasets/bwandowando/uberm-fb-waze-etc-us-apple-app-store-reviews)**
* 📂 **Archivo:** `Proyecto_Data_Science_III.ipynb`

---

## 🎯 Objetivos del Proyecto

* **Preprocesamiento de Texto:** Limpieza profunda usando **Spacy** y **NLTK** (Stopwords, Lematización, Tokenización).
* **Análisis Exploratorio (EDA):** Detección de patrones de comportamiento y "Pain Points" de los usuarios.
* **Modelado con Deep Learning:**
    1.  Crear una red neuronal base (Embedding + Pooling).
    2.  Implementar una arquitectura compleja (**LSTM**) para captar secuencias y contexto.
* **Evaluación:** Comparar el rendimiento de ambas arquitecturas mediante métricas de Accuracy y Loss.

---

## 🔍 Análisis Exploratorio (EDA)

Antes de modelar, se analizaron los patrones en los datos. Se descubrió una distribución **bimodal**: los usuarios aman u odian el servicio, con muy pocos puntos medios.

![Distribución y Wordcloud](LINK_A_LA_IMAGEN_DE_GRAFICOS_EDA.png)
*(Gráficos: Distribución de Ratings, Longitud de Reseña vs Rating y WordCloud de quejas)*

### 💡 Principales Insights:
> 1.  **Relación Longitud-Sentimiento:** Existe una correlación inversa. Las reseñas de **1 estrella** son significativamente más largas; los usuarios enojados escriben textos detallados para explicar su mala experiencia.
> 2.  **Pain Points Operativos:** La nube de palabras revela que los problemas no son de la app, sino del servicio físico: palabras clave como **"driver", "wait", "charge", "cancel"**.
> 3.  **Desbalance:** La escasez de calificaciones neutras (2-4 estrellas) desafía al modelo a distinguir matices sutiles.

---

## 🧪 Herramientas y Tecnologías

El proyecto fue desarrollado íntegramente en **Python** utilizando el siguiente stack tecnológico:

* **Procesamiento de Datos:** `Pandas`, `Numpy`
* **NLP:** `Spacy`, `NLTK`, `Re` (Expresiones Regulares)
* **Deep Learning:** `TensorFlow`, `Keras` (Sequential, LSTM, Embedding, Dropout)
* **Visualización:** `Matplotlib`, `Seaborn`, `WordCloud`

---

## 🧠 Arquitecturas de Modelado

Se entrenaron y compararon dos enfoques de Redes Neuronales:

### 🔹 Modelo 1: Arquitectura Sencilla (Baseline)
* **Enfoque:** "Bag of Words" (Bolsa de palabras).
* **Capas:** Embedding + GlobalAveragePooling1D + Dense (Softmax).
* **Características:** Rápido de entrenar, pero ignora el orden de las palabras.

### 🔹 Modelo 2: Arquitectura Recurrente (LSTM)
* **Enfoque:** Secuencial (Contexto).
* **Capas:** Embedding (128 dims) + **LSTM (64 units)** + Dense (ReLU) + Dropout (0.2).
* **Mejora:** Capaz de "recordar" palabras anteriores para entender el contexto de la frase.

---

## 📈 Resultados y Comparación

Se evaluaron ambos modelos con un set de datos de prueba desconocido (*Test Set*).

![Comparación de Modelos](LINK_A_LA_IMAGEN_DE_CURVAS_COMPARACION.png)
*(Gráfico: Comparación de Accuracy y Loss durante el entrenamiento)*

| Modelo | Accuracy (Test) | Observación |
| :--- | :--- | :--- |
| **Modelo 1 (Sencillo)** | **74.53%** | Buen rendimiento base, muy rápido. |
| **Modelo 2 (LSTM)** | **75.36%** | **Ganador ⭐**. Mejor manejo de estructura semántica. |

### 📌 Conclusión Final
El modelo **LSTM** logró una mejora neta del **1.12%**. Aunque numérica parece pequeña, cualitativamente es importante: el modelo LSTM demostró ser más robusto al inicio del entrenamiento.

Sin embargo, se observó que el modelo complejo tiende al *overfitting* más rápido (ver curva de Loss), lo que sugiere que para reseñas cortas y directas, la complejidad añadida tiene un retorno decreciente. El modelo es capaz de automatizar la lectura de miles de comentarios con una precisión de 3 de cada 4 casos.

---

## 👨‍💻 Autor

**Lautaro Falco**
*Data Science Student | Business Analytics | Machine Learning*
📫 **Contacto:** [Tu Perfil de LinkedIn]
