# Proyecto - California Housing Prices

Este proyecto utiliza el conjunto de datos **California Housing Prices**, basado en el censo de California de 1990, para analizar y modelar los precios medianos de las viviendas en los distritos de este estado.

## Descripción del Proyecto

El objetivo principal del proyecto es explorar, limpiar y modelar los datos para predecir los precios de las viviendas medianas en función de diversas características sociodemográficas y geográficas. Incluye:

- **Análisis Exploratorio de Datos (EDA):** Visualización de las relaciones entre variables y análisis de correlaciones.
- **Preprocesamiento de Datos:** Manejo de valores nulos, transformación de variables, y codificación de datos categóricos.
- **Modelado Predictivo:** Entrenamiento de un modelo de regresión lineal para predecir los precios de las viviendas.

## 📊 Dataset

El conjunto de datos utilizado está disponible en Kaggle:  
[California Housing Prices Dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

### Columnas del Dataset

- `longitude`: Longitud geográfica.
- `latitude`: Latitud geográfica.
- `housing_median_age`: Edad media de las viviendas en la zona.
- `total_rooms`: Número total de habitaciones.
- `total_bedrooms`: Número total de dormitorios.
- `population`: Población total.
- `households`: Número de hogares.
- `median_income`: Ingreso medio en la zona.
- `median_house_value`: Valor medio de las viviendas.
- `ocean_proximity`: Proximidad al océano.

> ⚠️ **Nota:** El dataset contiene valores nulos y requiere preprocesamiento.

## Herramientas y Tecnologías

- **Lenguaje:** Python  
- **Bibliotecas:**
  - `pandas` y `numpy` para manejo de datos.
  - `matplotlib` y `seaborn` para visualización.
  - `scikit-learn` para preprocesamiento y modelado.

## Pasos Principales del Proyecto

1. **Carga y Exploración de los Datos:**  
   Se realizó una inspección inicial para entender la estructura del dataset y detectar valores nulos.

2. **Análisis Exploratorio de Datos (EDA):**  
   - Histogramas de las variables para observar distribuciones.
   - Mapa de calor para analizar correlaciones entre variables.

3. **Preprocesamiento:**  
   - Eliminación de valores nulos.
   - Transformaciones logarítmicas en variables con sesgo.
   - Codificación de la variable categórica `ocean_proximity` mediante *one-hot encoding*.

4. **Ingeniería de Características:**  
   - Creación de nuevas variables como:
     - `bedroom_ratio`: Relación entre dormitorios y habitaciones totales.
     - `household_rooms`: Promedio de habitaciones por hogar.

5. **Modelado Predictivo:**  
   Entrenamiento de un modelo de **regresión lineal** para predecir los precios medianos de las viviendas (`median_house_value`).

6. **Evaluación del Modelo:**  
   - Métricas de evaluación como el error cuadrático medio (*Mean Squared Error, MSE*).
   - Validación en datos de prueba.

## 📈 Visualizaciones

El proyecto incluye visualizaciones clave como:

- Mapas de calor para identificar correlaciones.
- Diagramas de dispersión que muestran la relación entre ubicación geográfica (`latitude`, `longitude`) y precios de vivienda.
- Histogramas de las variables transformadas.

# House_Price_Prediction-Project
