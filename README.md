# readmission-predictor

Predicción de reingreso hospitalario para pacientes diabéticos usando machine learning.

## Descripción 

Este proyecto tiene como objetivo predecir si un paciente diabético, al que se le da el alta hospitalaria, será reingresado en el futuro. Utilizando técnicas de machine learning, el modelo analiza datos históricos de pacientes para hacer predicciones sobre su probabilidad de reingreso. Así, se permite mejorar la atención que reciben los pacientes una vez que ingresan por primera vez, evitando altas erróneas, optimizando recursos hospitalarios. 

## Dataset

Los datos se pueden encontrar en [UCI ML Repository](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008). Clore, J., Cios, K., DeShazo, J., & Strack, B. (2014). *Diabetes 130-US Hospitals for Years 1999-2008* [Dataset]. UCI Machine Learning Repository. [https://doi.org/10.24432/C5230J](https://doi.org/10.24432/C5230J).

El dataset contiene información de pacientes, incluyendo características demográficas, condiciones médicas previas, datos de tratamientos, diagnósticos, medicación y resultados de exámenes médicos, así como la variable objetivo que indica si un paciente fue reingresado antes de 30 días, después o no lo fue. Por tanto, es un problema de clasificación multiclase.

Estos datos, con los que estamos trabajando en este proyecto, no son de la mejor calidad, pues se incluyen valores faltantes, características irrelevantes, datos inconsistentes y desbalance de clases. Además, incluye tanto valores numéricos como categóricos. Esto es así pues el tratamiento de datos complejos también forma parte del desarrollo del proyecto. 
## Estructura

`readmpred.ipynb`

En este notebook se desarrolla todo el proyecto, el cual está organizado en las siguientes secciones:

- **Carga de Datos**
  
- **Procesamiento de los datos**:
  - Tratamiento de los datos faltantes (Imputación)
  - Conversión de datos categóricos a numéricos con Label encoder y one-hot.

- **Selección de características mediante dos métodos**:
  - **Visualización gráfica**: Se utilizan técnicas como boxplots, histogramas, la matriz de correlación y análisis de correlación con la variable respuesta.
  - **Métodos de envoltura (RFE)**: Selección de características basada en la importancia y rendimiento de cada una en los modelos.

- **Entrenamiento y elección del mejor modelo**:

  - **Desbalance de clases**: Primero usaremos diversas técnicas para tratar este problema.
  - **Búsqueda de hiperparámetros**: Usamos GridSearchCV para encontrar los mejores hiperparámetros.
  - **XGBoost**: Entrenamos el modelo final

## Conclusión

Este proyecto ha sido un ejercicio valioso de procesamiento de datos. Se han optimizado modelos para maximizar métricas específicas como el recall. Pasamos de una precisión del 56% y un recall de un 39% en media en el modelo base, a una precisión del 61,4% y un recall del 61,33% una vez aplicadas diversas técnicas de balanceo de clases, de búsqueda de hiperparámetros y de selección de características.

## Contacto

daviddelgadobejarano@gmail.com 

[Portfolio](https://daviddb11.github.io/)


 
