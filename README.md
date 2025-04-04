# Regresión Lineal en Emisiones de CO₂

## Objetivo  
Analizar la relación entre el consumo de combustible y las emisiones de dióxido de carbono (CO₂) mediante modelos de regresión lineal. Se busca predecir las emisiones basadas en características del vehículo, aplicando además técnicas de regularización para mejorar la generalización del modelo.

---

## Tabla de Contenidos
- [Introducción](#introducción)  
- [Fuentes de Datos](#fuentes-de-datos)  
- [Procesamiento y Análisis](#procesamiento-y-análisis)  
- [Modelado](#modelado)  
- [Regularización](#regularización)  
- [Resultados](#resultados)  
- [Requisitos](#requisitos)  
- [Uso](#uso)  
- [Contribuciones](#contribuciones)  
- [Autor](#autor)  

---

## Introducción  
Este proyecto aplica técnicas de regresión lineal sobre un conjunto de datos de consumo de combustible y emisiones de CO₂ de vehículos. El objetivo es construir modelos predictivos y evaluar su rendimiento, incluyendo técnicas de regularización para evitar el sobreajuste.

---

## Fuentes de Datos  
- **Archivo Utilizado:** `FuelConsumptionCo2.csv`  
- **Fuente:** [Environment Canada - Open Government Portal](https://open.canada.ca/data/en/dataset)  
- El conjunto de datos incluye variables como tamaño del motor, consumo de combustible en ciudad y carretera, tipo de combustible, y emisiones de CO₂.

---

## Procesamiento y Análisis  
El análisis se realiza en un notebook Jupyter, con las siguientes etapas:
- Exploración de los datos: descripción estadística y visualización.
- Limpieza de datos: eliminación de columnas innecesarias y valores atípicos.
- Selección de variables relevantes para el modelo.

---

## Modelado  
Se implementa un modelo de regresión lineal simple para predecir las emisiones de CO₂ con base en variables como:
- Tamaño del motor (ENGINESIZE)
- Consumo de combustible en ciudad y carretera (FUELCONSUMPTION_CITY, FUELCONSUMPTION_HWY)

---

## Regularización  
Para mejorar la generalización del modelo, se aplica regularización utilizando:
- **Ridge Regression:** minimiza los coeficientes excesivamente grandes, ayudando a reducir el sobreajuste.

Comparación de métricas:
- MAE (Error absoluto medio)
- MSE (Error cuadrático medio)
- R² (Coeficiente de determinación)

---

## Resultados  
- El modelo de regresión lineal logra una buena aproximación para predicciones básicas.
- Ridge Regression mejora el rendimiento al reducir la varianza en modelos más complejos.
- Se observan relaciones lineales claras entre el tamaño del motor y las emisiones de CO₂.

---

## Requisitos  
Para ejecutar el notebook, asegúrate de tener instalado:

- Python 3.x  
- Jupyter Notebook o Jupyter Lab  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  

Instalación rápida:
```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

---

## Uso  
1. Clona este repositorio:
```bash
git clone https://github.com/tu_usuario/regresion-co2.git
```
2. Abre el notebook:
```bash
jupyter notebook "Regresion Lineal-CO2.ipynb"
```
3. Ejecuta las celdas en orden para entrenar el modelo y analizar los resultados.

---

## Contribuciones  
¿Te gustaría proponer mejoras o añadir nuevos enfoques de modelado?  
¡Eres bienvenido! Puedes abrir un issue o enviar un pull request.

---

## Autor  
**José Eduardo Saucedo Martínez** 
