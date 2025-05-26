
# 🎯 Social Network Ads – Clasificación de Usuarios

Este proyecto tiene como objetivo predecir si un usuario comprará un producto anunciado en redes sociales, utilizando diversos modelos de Machine Learning. El análisis fue realizado con la herramienta visual **Orange**.

## 📁 Dataset

El dataset contiene 3 columnas relevantes:
- `Age`: Edad del individuo
- `EstimatedSalary`: Salario estimado
- `Purchased`: Objetivo binario (1 = compró, 0 = no compró)

Fuente: [Social_Network_Ads.csv]

## 🧠 Modelos Evaluados

Se entrenaron y compararon 5 algoritmos de clasificación utilizando validación cruzada estratificada con 5 folds. Las métricas evaluadas fueron AUC, Accuracy, F1, Precisión, Recall y MCC.

| Modelo                | AUC   | Accuracy | F1    | Precisión | Recall | MCC   |
|-----------------------|-------|----------|-------|-----------|--------|--------|
| **Random Forest**     | 0.996 | 0.957    | 0.957 | 0.957     | 0.957  | 0.907 |
| **SVM**               | 0.962 | 0.920    | 0.920 | 0.921     | 0.920  | 0.831 |
| **Árbol de Decisión** | 0.903 | 0.917    | 0.916 | 0.917     | 0.917  | 0.821 |
| **Regresión Logística** | 0.937 | 0.853  | 0.850 | 0.854     | 0.853  | 0.682 |
| **K-NN**              | 0.831 | 0.783    | 0.781 | 0.781     | 0.783  | 0.529 |

## ✅ Conclusiones

- 🔝 **Random Forest** fue el modelo más preciso, con un AUC de 0.996 y una exactitud del 95.7%. Ideal para problemas con relaciones no lineales y alta variabilidad.
- 🧠 **SVM** y **Árbol de Decisión** también ofrecieron muy buen rendimiento, siendo buenas opciones según el contexto del negocio.
- 📊 **Regresión Logística** es simple e interpretable, pero menos precisa.
- ⚠️ **KNN** tuvo el rendimiento más bajo y es sensible a la escala y dimensionalidad.

## 📌 Herramientas Utilizadas

- Orange 3 (análisis visual y evaluación de modelos)
- Python (para análisis de datos y limpieza inicial)
- Pandas / CSV
