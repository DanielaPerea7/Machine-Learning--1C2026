# Optimización de la Movilidad Urbana: Segmentación de Usuarios y Predicción de Churn en EcoBici

## Introducción

Este proyecto aborda la problemática de la movilidad sustentable en la Ciudad de Buenos Aires, utilizando el sistema de bicicletas públicas **EcoBici**. En un contexto de alta demanda urbana, entender el comportamiento del usuario es vital para la gestión operativa. Se aplican técnicas de **Machine Learning** para transformar registros brutos de viajes en perfiles de usuario y modelos predictivos que permitan anticipar el abandono del sistema.

## Objetivo

Desarrollar un ecosistema de modelos de Machine Learning para segmentar la base de usuarios de EcoBici según su intensidad de uso y predecir la probabilidad de **Churn** (inactividad > 60 días) para diseñar estrategias de retención.

## Integrante

- **Comisión:** 26141
- **Nombre:** Daniela Perea

## Dataset utilizado

Se utilizaron datos abiertos de la Ciudad de Buenos Aires (BA Data):

- **Fuente:** [Portal de Datos Abiertos de CABA - EcoBici](https://data.buenosaires.gob.ar/dataset/bicicletas-publicas)
- **Archivo:** `recorridos-2025.csv`

## Estructura del repositorio

- `Pre_Entrega_Proyecto_Final/`:
    - `ML_Pre_Entrega_Proyecto_Final.ipynb`: Análisis exploratorio, tratamiento de nulos y eliminación de outliers, Creación de etiquetas de Churn, segmentación de perfiles y unión de tablas.
    - `dataset/`: Carpeta (local) con los datasets originales y el dataset procesado.
- `README.md`: Descripción general del proyecto.

## Metodología

El proyecto sigue el ciclo de vida de Machine Learning:

1. **Limpieza y Preprocesamiento:** Filtrado de viajes inválidos (duraciones extremas), tratamiento de valores nulos en demografía y conversión de tipos de datos temporales.
2. **Ingeniería de Características (Feature Engineering):** Construcción de la variable **Target (Churn)** basada en ventanas de inactividad de 60 días y cálculo de métricas de comportamiento (frecuencia, duración media, distancias).
3. **Análisis Exploratorio (EDA):** Identificación de patrones de uso por género, edad y franjas horarias.
4. **Modelado No Supervisado:** Segmentación de usuarios en perfiles (Intensivos, Ocasionales, Nuevos).
5. **Modelado Supervisado:** Implementación y comparación de modelos para predecir el Churn y la demanda futura.

## Herramientas utilizadas

- **Lenguaje:** Python 3.x
- **Librerías principales:**
    - `Pandas`: Manipulación y limpieza de datos.
    - `NumPy`: Operaciones numéricas.
    - `Matplotlib` & `Seaborn`: Visualización de datos estática.
    - `Scikit-Learn`: Preprocesamiento (Escalado, Codificación) y algoritmos de ML.
    - `Google Colab`: Entorno de desarrollo en la nube.

---
