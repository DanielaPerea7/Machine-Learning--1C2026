# Optimización de la Movilidad Urbana: Segmentación de Usuarios y Predicción de Churn en EcoBici 🚲

## 📌 Introducción

La movilidad sustentable se ha convertido en uno de los principales desafíos de las grandes ciudades. En este contexto, el sistema de bicicletas públicas **EcoBici** de la Ciudad de Buenos Aires genera una gran cantidad de datos que permiten analizar patrones de uso, hábitos de movilidad y niveles de retención de usuarios.

Este proyecto utiliza técnicas de **Machine Learning** y análisis de datos para transformar registros de viajes en información estratégica, permitiendo identificar perfiles de usuarios y predecir posibles casos de abandono del sistema (*Churn*).

---

## 🎯 Objetivo del Proyecto

Desarrollar un ecosistema de modelos de Machine Learning capaz de:

- Segmentar usuarios de EcoBici según su comportamiento e intensidad de uso.
- Detectar patrones de movilidad urbana.
- Predecir la probabilidad de **Churn** (usuarios con más de 60 días de inactividad).
- Generar insights que permitan diseñar estrategias de retención y optimización del servicio.

---

## 👩‍💻 Integrante

- **Nombre:** Daniela Perea  
- **Comisión:** 26141  

---

## 📂 Dataset Utilizado

Se trabajó con datos abiertos publicados por el Gobierno de la Ciudad de Buenos Aires.

- **Fuente:** [Portal de Datos Abiertos de Buenos Aires - EcoBici](https://data.buenosaires.gob.ar/dataset/bicicletas-publicas)
- **Archivo utilizado:** `recorridos-2025.csv`

El dataset contiene información sobre:

- Fecha y horario de inicio/fin de viaje
- Estaciones de origen y destino
- Duración del recorrido
- Datos demográficos de usuarios
- Tipo de usuario y comportamiento de uso

---

## 🗂️ Estructura del Repositorio

```bash
📦 Proyecto
├── 📁 Pre_Entrega_Proyecto_Final
│   ├── 📓 ML_Pre_Entrega_Proyecto_Final.ipynb
│   └── 📁 dataset
├── 📄 README.md
```

### Contenido principal

- **ML_Pre_Entrega_Proyecto_Final.ipynb**
  - Limpieza y preprocesamiento de datos
  - Tratamiento de valores nulos
  - Detección y eliminación de outliers
  - Feature Engineering
  - Creación de la variable objetivo (*Churn*)
  - Análisis exploratorio de datos (EDA)
  - Segmentación de usuarios
  - Integración y preparación final de datasets

- **dataset/**
  - Datasets originales
  - Dataset procesado para modelado

---

## ⚙️ Metodología

El proyecto sigue las principales etapas del ciclo de vida de un proyecto de Machine Learning:

### 1️⃣ Limpieza y Preprocesamiento

- Eliminación de viajes inválidos o inconsistentes
- Tratamiento de datos faltantes
- Conversión y normalización de variables temporales
- Filtrado de duraciones extremas (*outliers*)

### 2️⃣ Ingeniería de Características (*Feature Engineering*)

- Construcción de la variable objetivo **Churn**
- Generación de métricas de comportamiento:
  - Frecuencia de uso
  - Duración promedio de viajes
  - Cantidad de recorridos
  - Distancias recorridas
  - Antigüedad del usuario

### 3️⃣ Análisis Exploratorio de Datos (EDA)

Se analizaron patrones relacionados con:

- Franjas horarias de uso
- Distribución por género y edad
- Intensidad de uso
- Comportamiento temporal
- Tendencias de movilidad urbana

### 4️⃣ Modelado No Supervisado

Aplicación de técnicas de segmentación para identificar perfiles de usuarios, como:

- Usuarios intensivos
- Usuarios ocasionales
- Usuarios nuevos o de baja actividad

### 5️⃣ Modelado Supervisado

Desarrollo y comparación de modelos predictivos para:

- Predicción de Churn
- Análisis de retención
- Proyección de demanda futura

---

## 🛠️ Herramientas y Tecnologías

### Lenguaje

- Python 3.x

### Librerías principales

- `Pandas` → Manipulación y análisis de datos
- `NumPy` → Operaciones numéricas
- `Matplotlib` y `Seaborn` → Visualización de datos
- `Scikit-Learn` → Modelado y preprocesamiento
- `Google Colab` → Desarrollo y ejecución en la nube

---

## 📈 Resultados Esperados

A través de este proyecto se busca:

- Comprender el comportamiento de los usuarios de EcoBici.
- Detectar posibles casos de abandono del sistema.
- Mejorar la toma de decisiones basada en datos.
- Contribuir al análisis de movilidad sustentable en entornos urbanos.

---

## 🚀 Próximos Pasos

- Entrenamiento y evaluación de modelos predictivos.
- Optimización de hiperparámetros.
- Visualización avanzada de métricas.
- Implementación de dashboards interactivos.
- Generación de recomendaciones estratégicas para retención de usuarios.

---
