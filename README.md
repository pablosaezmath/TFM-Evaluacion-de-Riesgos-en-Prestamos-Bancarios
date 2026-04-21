# TFM — Scoring Crediticio para Evaluación de Riesgos Bancarios

> **Trabajo Fin de Máster · Máster en Big Data y Ciencia de Datos · VIU, 2026**  
> **Autor:** Pablo Sáez Gil · saeznovelda@gmail.com

---

## ¿Qué problema resuelve?

Las entidades financieras necesitan estimar la probabilidad de impago antes de conceder un préstamo. Este proyecto construye un **modelo de scoring crediticio end-to-end** que predice si un solicitante incurrirá en mora, combinando análisis exploratorio riguroso, ingeniería de características y comparación sistemática de modelos de clasificación y regresión sobre un dataset real de 8.399 clientes.

## Pipeline

```
Carga de datos → EDA → Preprocesamiento → Modelado → Evaluación → Conclusiones
```

1. **EDA** — distribuciones, correlaciones, análisis de morosidad por segmento
2. **Preprocesamiento** — imputación, codificación, escalado, transformaciones logarítmicas
3. **Modelado** — clasificadores y regresores con validación cruzada estratificada y RandomizedSearchCV
4. **Evaluación** — AUC-ROC, curva ROC, matriz de confusión, importancia de variables, MAE, RMSE, R²

## Modelos evaluados

**Clasificación** (predicción de mora): `Logistic Regression` · `KNN` · `SVM` · `Random Forest` · `AdaBoost` · `XGBoost`

**Regresión** (estimación numérica): `Linear Regression` · `Random Forest Regressor` · `XGBoost Regressor`

## Stack

`Python` · `pandas` · `numpy` · `scikit-learn` · `XGBoost` · `matplotlib` · `seaborn` · `Jupyter Notebook`

## Estructura

```
TFM-Evaluacion-de-Riesgos-en-Prestamos-Bancarios/
├── notebook/
│   └── TFM-Evaluacion-de-Riesgos-en-Prestamos-Bancarios.ipynb
├── data/
│   └── data.csv
└── README.md
```

## Cómo reproducir

```bash
git clone https://github.com/pablosaezmath/TFM-Evaluacion-de-Riesgos-en-Prestamos-Bancarios.git
cd TFM-Evaluacion-de-Riesgos-en-Prestamos-Bancarios
pip install pandas numpy scikit-learn xgboost matplotlib seaborn jupyter
jupyter notebook notebook/TFM-Evaluacion-de-Riesgos-en-Prestamos-Bancarios.ipynb
```

## Autor

**Pablo Sáez Gil** — Graduado en Matemáticas · Máster en Big Data y Ciencia de Datos (VIU) · saeznovelda@gmail.com
