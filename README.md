# Predicción de Mora Bancaria mediante Machine Learning

## Descripción

Este proyecto desarrolla un modelo de Machine Learning para predecir la probabilidad de mora de clientes bancarios utilizando técnicas de aprendizaje supervisado.

El objetivo consiste en asistir al área de riesgo crediticio en la identificación temprana de clientes con elevada probabilidad de incumplimiento, mejorando así las decisiones de otorgamiento de crédito.

El modelo fue desarrollado como proyecto final del curso de Ciencia de Datos de Coderhouse.

---

## Problema de negocio

Las entidades financieras enfrentan el desafío de reducir la morosidad sin restringir excesivamente el acceso al crédito.

Los modelos tradicionales de evaluación crediticia suelen basarse principalmente en el historial financiero del cliente, pero pueden perder capacidad predictiva frente a cambios económicos bruscos.

Este proyecto propone utilizar Machine Learning para estimar el riesgo de mora considerando simultáneamente variables financieras y sociodemográficas.

---

## Objetivos

### Objetivo general

Construir un modelo de clasificación capaz de predecir la probabilidad de mora de nuevos clientes.

### Objetivos específicos

- Analizar el perfil sociodemográfico y financiero de los clientes.
- Explorar la relación entre las variables explicativas y la mora.
- Entrenar un modelo Random Forest.
- Evaluar el desempeño del modelo mediante métricas de clasificación.
- Identificar las variables con mayor importancia predictiva.

---

## Dataset

Fuente:

- Dataset de riesgo crediticio disponible en Kaggle (Perú).

Características iniciales

- 8.399 registros
- 14 variables

Luego del proceso de limpieza e ingeniería de variables:

- 6.074 registros
- 29 variables

Variable objetivo:

- **Mora**
    - 0 = Cliente al día
    - 1 = Cliente moroso

Variables utilizadas:

- Edad
- Ingreso
- Tipo de vivienda
- Zona
- Nivel educativo
- Nivel de ahorro
- Score crediticio
- Clasificación SBS
- Experiencia financiera
- Línea de crédito
- Deuda financiera
- Entre otras variables derivadas.

---

## Metodología

El proyecto se desarrolló siguiendo las siguientes etapas:

### 1. Limpieza de datos

- Eliminación de registros inconsistentes
- Tratamiento de valores faltantes
- Corrección de tipos de datos
- Ingeniería de variables

### 2. Análisis Exploratorio (EDA)

Se realizaron análisis:

- Univariado
- Bivariado
- Multivariado

Incluyendo:

- Histogramas
- Boxplots
- Barras apiladas
- Distribuciones
- Comparación entre clientes morosos y no morosos

---

### 3. Modelo de Machine Learning

Se utilizó un algoritmo de clasificación:

**Random Forest Classifier**

Motivos de selección:

- Maneja relaciones no lineales.
- Tolera variables heterogéneas.
- Es robusto frente a ruido.
- Permite calcular importancia de variables.
- Presenta buen desempeño en problemas de clasificación.

---

### 4. Evaluación del modelo

El modelo fue evaluado utilizando:

- Accuracy
- Precision
- Recall
- F1 Score
- Matriz de Confusión
- ROC AUC

---

## Principales hallazgos

El análisis exploratorio mostró que:

- Los clientes con menor score presentan mayor probabilidad de mora.
- Una menor experiencia financiera incrementa el riesgo.
- Los menores ingresos se asocian con mayor morosidad.
- Existen diferencias de riesgo según nivel educativo, tipo de vivienda y zona de residencia.

Además, el modelo permitió identificar las variables con mayor poder predictivo para la clasificación del riesgo crediticio.

---

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## Estructura del proyecto

```
Proyecto/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── images/
│
├── models/
│
├── requirements.txt
│
└── README.md
```

---

## Resultados

El modelo obtuvo un desempeño satisfactorio para la identificación de clientes con riesgo de mora, mostrando que las variables financieras tradicionales (score, clasificación y deuda) continúan siendo relevantes, aunque variables sociodemográficas y de experiencia financiera también aportan capacidad predictiva.

---

## Posibles mejoras

- Optimización de hiperparámetros mediante Grid Search.
- Comparación con XGBoost y LightGBM.
- Balanceo de clases mediante SMOTE.
- Validación cruzada.
- Implementación como API para scoring en tiempo real.

---

## Autor

**Iván Federico Montes de Oca**

Sociólogo | Ciencia de Datos | Machine Learning

Proyecto desarrollado como trabajo final del curso de Data Science de Coderhouse.
