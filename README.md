# 🏠 Airbnb Price Prediction – Machine Learning Project

## 📌 Descripción
Este proyecto aborda un **problema de regresión**, cuyo objetivo es **predecir el precio (`Price`) de alojamientos Airbnb** a partir de la información disponible en el dataset.  
El trabajo se ha desarrollado siguiendo un flujo completo de **Machine Learning**, desde el análisis exploratorio hasta la evaluación final de distintos modelos.

---

## 🗂️ Dataset
- Fuente: Dataset de listados de Airbnb
- Tipo de problema: **Regresión**
- Variable objetivo: `Price`

---

## 🧪 Metodología

El proyecto sigue una estructura similar a la utilizada en clase:

### 1. Preparación de datos
- Carga del dataset
- Limpieza de nombres de columnas
- División **train/test** (80/20)

### 2. Análisis Exploratorio (EDA)
- Inspección inicial (`head`, `describe`, `dtypes`)
- Detección de valores atípicos
- Análisis de correlaciones

### 3. Preprocesamiento
- Tratamiento de valores nulos
- Eliminación de variables con alta cardinalidad
- Codificación de variables categóricas (One-Hot Encoding)
- Reducción de dimensionalidad
- Selección de variables mediante **Lasso**

### 4. Modelado y Evaluación
Se entrenaron y compararon varios modelos:
- **Ridge Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

Evaluación realizada sobre el conjunto de test usando:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² (Coeficiente de determinación)

---

## 📊 Resultados
Los modelos de ensemble (**Random Forest y Gradient Boosting**) superan al modelo lineal (Ridge), lo que indica la presencia de relaciones no lineales en los datos.  
**Random Forest** obtuvo el mejor equilibrio entre error y capacidad de generalización.

---

## 🧠 Conclusión
El análisis muestra que los modelos no lineales son más adecuados para este problema.  
A pesar del ruido inherente al dataset, se consigue un modelo razonable para la predicción del precio, destacando Random Forest como la mejor opción entre los modelos evaluados.

---

## 🛠️ Tecnologías utilizadas
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

