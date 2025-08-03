# 📡 Challenge TelecomX LATAM Parte 2

Este proyecto forma parte del **Challenge de la Formación: Estadísticas y Machine Learning G8 - ONE**, y tiene como objetivo aplicar técnicas de **Machine Learning** para investigar la **evasión de clientes** en TelecomX, una empresa de telecomunicaciones.

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1p5NQkiSJm47ZPxECKqzDyjiwPcaPo4BO?usp=sharing)

## Descripción

El objetivo principal es **predecir la cancelación (churn)** de clientes con base en sus características demográficas, de contrato y uso de servicios. A partir de esto, se busca **identificar los factores clave que explican la baja fidelización de los clientes** y **proporcionar recomendaciones estratégicas** para mejorar la retención.

## Modelos Aplicados

- **Árbol de Decisión**
- **Random Forest**
- **K-Nearest Neighbors (KNN)**
- **Regresión Logística**

Los modelos fueron comparados en términos de: **accuracy**, **precision**, **recall** y **F1-score**.

## Análisis Realizados

### 📊 Análisis exploratorio

- **Distribución de la variable objetivo (`has_churned`)** y su relación con otras variables.
- **Análisis de variables numéricas y categóricas** mediante boxplots y gráficos de barras.
- **Correlaciones con `has_churned`:**

### 🔎 Selección e interpretación de variables

- **Random Forest:**

  - Se evaluó la importancia de cada variable usando `.feature_importances_`.
  - Se identificaron las 15 variables más relevantes para la predicción.

- **Regresión Logística:**
  - Se analizaron los coeficientes del modelo optimizado para identificar variables protectoras y de riesgo.

### 🤖 Comparación de modelos

- **Modelos Evaluados:**

  - Decision Tree
  - Random Forest
  - Optimized Random Forest
  - KNN
  - Logistic Regression
  - Optimized Logistic Regression

- **Métrica Principal:** F1-score

- **Mejor Modelo:** Optimized Logistic Regression (F1 = 0.6223), balanceando precisión y sensibilidad.

### 💡 Insights generados

- Contratos mes a mes, cargos elevados y ausencia de servicios como seguridad online son factores de **alto riesgo de churn**.
- Contratos de largo plazo, métodos de pago automáticos y antigüedad protegen contra la cancelación.

### 🪝 Estrategias de retención

- Incentivar contratos largos.
- Implementar programas de fidelización temprana.
- Optimizar servicios y ajustar percepción de precio.
- Promover pagos automáticos y servicios de valor agregado.
- Usar el modelo predictivo como sistema de alerta temprana.

## Uso

**1. Clonar el repositorio:**

```bash
git clone https://github.com/dano796/challenge-telecomx-latam-parte-2.git
```

**2. Abrir el archivo .ipynb en Google Colab.**

**3. Cargar el dataset procesado (data/datos_procesados.csv)**

---

### Challenge de la Formación: Estadisticas y Machine Learning G8 - ONE

### Daniel Ortiz Aristizábal
