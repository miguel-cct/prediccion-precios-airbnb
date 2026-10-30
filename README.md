# Predicción de Precios de Alojamientos en Airbnb

Proyecto de análisis exploratorio de datos (EDA) y modelado de regresión desarrollado para la materia **Introducción a la Ciencia de Datos** (Facultad de Ciencias Económicas, Universidad de Buenos Aires).

El objetivo principal es predecir la tarifa diaria (`price`) de las publicaciones de Airbnb a partir de sus características físicas, de ubicación, tipo de propiedad y reputación del anfitrión.

---

## 📊 Estructura del Proyecto

* **`TP final regresión Airbnb.ipynb`**: Notebook con el procesamiento de datos, análisis exploratorio, ingeniería de características y evaluación de modelos predictivos.
* **`.gitignore`**: Configuración para excluir archivos de gran tamaño (como el archivo de datos original) del control de versiones.

---

## 🛠️ Metodología y Flujo de Trabajo

1. **Limpieza y Preprocesamiento de Datos:**
   * Conversión y normalización de la variable objetivo `price` a formato numérico.
   * Filtro y depuración de registros sin precio, valores nulos o valores inverosímiles ($\le 0$).
   * Imputación y acondicionamiento de variables explicativas.

2. **Análisis Exploratorio de Datos (EDA):**
   * Evaluación de la distribución del precio diario y detección de sesgos y valores extremos.
   * Transformación logarítmica $\log(\text{price})$ para corregir asimetrías y estabilizar la varianza en los modelos.
   * Análisis comparativo del precio según el tipo de habitación (`room_type`) y variables clave mediante estadísticos agrupados y gráficos de dispersión/boxplots.

3. **Ingeniería de Características y Selección:**
   * Codificación de variables categóricas (tipo de alojamiento, comodidades, políticas de reserva).
   * Escalamiento de variables numéricas y análisis de correlación para evitar la multicolinealidad.

4. **Modelado y Evaluación:**
   * Entrenamiento y comparación de algoritmos de regresión para estimar el precio por noche.
   * Evaluación de métricas de desempeño (RMSE, MAE, $R^2$).

---

## 💻 Tecnologías Utilizadas

* **Lenguaje:** Python 3
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Modelado y Métricas:** Scikit-learn
* **Entorno:** Jupyter Notebook / Google Colab

---

## Dataset
https://data.insideairbnb.com/france/ile-de-france/paris/2026-06-16/data/listings.csv.gz

