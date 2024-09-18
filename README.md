# Proyecto de Análisis y Modelado de Datos

## Descripción del Proyecto

El objetivo de este proyecto es realizar un **análisis exploratorio de datos (EDA)** sobre cuatro conjuntos de datos, diagnosticar patrones clave y seleccionar una problemática específica para abordar (regresión, clasificación, clusterización, predicción). A partir del análisis, se seleccionará un conjunto de datos y se desarrollará un modelo predictivo que mejor se ajuste a la problemática encontrada.

Este repositorio contiene el dataset elegido, el análisis EDA inicial, y la descripción de la problemática seleccionada junto con los modelos aplicados.

## Datasets Utilizados

1. **Precio de casas**: Contiene características de distintos domicilios.
2. **Precio de autos**: Contiene datos de características de autos y sus precios.
3. **Lesiones**: Datos de 74 atletas, donde algunos presentan lesiones.

## Resumen del Análisis EDA

### 1. Precio de Casas
- Se observa cierta correlación entre las características de las casas y el precio.
- **Modelo sugerido**: Regresión. Se probaron varios modelos de regresión utilizando **LazyPredict** para seleccionar los más efectivos para predecir el precio de una casa en base a sus características.

### 2. Precio de Autos
- No se observa una correlación fuerte en la mayoría de las variables. Sin embargo, se decidió aplicar un modelo de regresión.
- **Modelo sugerido**: Árbol de regresión. Se aplicó **LazyPredict** para elegir el mejor modelo inicial y se acompañó de una búsqueda de hiperparámetros y optimización del modelo.

### 3. Prediccion de lesiones
- No se identifican correlaciones claras entre las variables.
- **Modelo sugerido**: Clasificación. Se apli modelo KGB para predecir lesiones en funcion a sus entrenamientos.
- El modelo fue optimizado utilizando **LazyPredict** para la selección inicial de modelos, seguido de una búsqueda de hiperparámetros.

## Problema Seleccionado

Se escogió el dataset de **Prediccion de lesiones**. Dado que no hay correlación clara entre las características, se decidió aplicar un **modelo de clasificación** para predecir lesiones. El proceso incluyó:

1. Selección inicial de modelos con **LazyPredict**.
2. Optimización mediante búsqueda de hiperparámetros.
3. Implementación final del modelo utilizando **LGB**.

## Instrucciones para Ejecutar

Sigue estos pasos para ejecutar el proyecto localmente:

1. Clona el repositorio:

    ```bash
    git clone https://github.com/Ferx096/PROYECTO2_ML.git
    ```

2. Navega a la carpeta del proyecto:

    ```bash
    cd PROYECTO2_ML
    ```

3. Instala las dependencias necesarias:

    ```bash
    pip install -r requirements.txt
    ```

4. Ejecuta los notebooks para EDA y modelado:

    ```bash
    jupyter notebook
    ```

### Estructura del Repositorio
/Proyecto2 │ ├── /datasets │ ├── dataset1.csv │ ├── dataset2.csv │ ├── dataset3.csv │ └── dataset4.csv │ ├── /EDA │
├── EDA_dataset1.ipynb │ ├── EDA_dataset2.ipynb │ ├── EDA_dataset3.ipynb │ └── EDA_dataset4.ipynb │ ├── /selected_dataset │
├── selected_dataset.csv │ └── EDA_selected_dataset.ipynb │└── README.md

## Autor

Fernando Cabrera Barranzuela

## Licencia

Este proyecto utiliza datasets de uso público.
