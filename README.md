# 📊 Proyecto de Predicción de Churn en Telecomunicaciones

## 📈 Problema de Negocio
Una empresa de telecomunicaciones desea **mejorar la retención de sus clientes**, identificando aquellos que tienen más posibilidades de abandonar el servicio (Churn). Este proyecto tiene como objetivo limpiar y preparar un conjunto de datos para el entrenamiento de un modelo de Churn.

## ❓ Preguntas Clave
- **🔍 Análisis Inicial**: ¿Qué insights podemos obtener del análisis exploratorio inicial del conjunto de datos?
- **🛠️ Transformaciones**: ¿Qué transformaciones básicas son necesarias para preparar los datos?
- **🔎 Datos Duplicados**: ¿Cómo podemos identificar y tratar los datos duplicados y los valores nulos?
- **📊 Outliers**: ¿Cómo manejamos los outliers presentes en el dataset?
- **📋 Variables Categóricas**: ¿Qué técnicas aplicamos para procesar las variables categóricas?

## 🚀 Configuración del Ambiente
Asegúrate de tener las siguientes bibliotecas instaladas:
```bash
pip install numpy pandas seaborn matplotlib sklearn
```

## 📥 Obtención y Tratamiento de Datos
### 📂 Cargando la Base de Datos
El conjunto de datos se carga desde un archivo JSON.

### 🧹 Tratamiento de Datos
Durante el preprocesamiento se realizan las siguientes operaciones:
- **🧽 Reemplazo de valores nulos** en la columna `cuenta.cobros.Total`.
- **🚫 Eliminación** de duplicados y valores nulos en columnas específicas.
- **📉 Manejo de outliers** utilizando el método del rango intercuartílico (IQR).
- **🔄 Normalización** de variables categóricas mediante codificación one-hot.

## 📊 Normalización de Datos
Se eliminan columnas innecesarias y se reemplazan los valores categóricos con representaciones numéricas.

## 🔍 Modelado
Se utiliza un **modelo de Random Forest** para predecir el churn de los clientes. Se evalúa el rendimiento del modelo mediante la división de los datos en conjuntos de entrenamiento y prueba.

### 📉 Reducción de Dimensionalidad
Se aplican diversas técnicas para reducir la dimensionalidad de los datos, incluyendo:
- **🎨 Diagramas de violín y puntos** para visualización.
- **🗺️ Mapas de calor** para correlación de variables.
- **🔍 Selección de características** utilizando `SelectKBest`.

## 📝 Conclusiones
Este proyecto proporciona un marco para la limpieza y preparación de datos en un contexto de churn en telecomunicaciones, lo que permite el desarrollo de modelos predictivos más precisos.
