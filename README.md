# readmission-predictor

## Descripción 

Tiene como objetivo predecir si un paciente diabético, al que se le da el alta hospitalaria, será reingresado en el futuro. Utilizando técnicas de machine learning, el modelo analiza datos históricos de pacientes para hacer predicciones sobre su probabilidad de reingreso. Así, se permite mejorar la atención que reciben los pacientes una vez que ingresan por primera vez, evitando altas erróneas, optimizando recursos hospitalarios.

## Dataset

Los datos se pueden encontrar en [UCI ML Repository](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008). Clore, J., Cios, K., DeShazo, J., & Strack, B. (2014). *Diabetes 130-US Hospitals for Years 1999-2008* [Dataset]. UCI Machine Learning Repository. [https://doi.org/10.24432/C5230J](https://doi.org/10.24432/C5230J).

Los datos con los que estamos trabajando en este proyecto no son de la mejor calidad, pues se incluyen valores faltantes, características irrelevantes y datos inconsistentes.  Además, incluye tanto valores numéricos como categóricos. Por lo tanto, uno de los principales objetivos de este proyecto es realizar un tratamiento completo de los datos.

## Estructura

'readmpred.ipynb' 

En este notebook se desarrolla todo el proyecto. Este consta de lo siguiente:

- Procesamiento de los datos:
  -- Tratamiento de datos faltantes, conversión de datos categóricos a numéricos, representaciones one-hot.

- Selección de características mediante dos métodos:
  -- Mediante visualización gráfica: boxplots, histogramas, correlation matrix, correlación con la variable respuesta.
  -- Métodos de envoltura (RFE)

- Entrenamiento y elección del mejor modelo de entre los siguientes:

 -- Logistic Regression Multinomial
 -- Random Forest
 -- Decision Trees

 
