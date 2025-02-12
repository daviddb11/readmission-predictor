# readmission-predictor

Predicción de reingreso hospitalario para pacientes diabéticos usando machine learning.

## Descripción 

Este proyecto tiene como objetivo predecir si un paciente diabético, al que se le da el alta hospitalaria, será reingresado en el futuro. Utilizando técnicas de machine learning, el modelo analiza datos históricos de pacientes para hacer predicciones sobre su probabilidad de reingreso. Así, se permite mejorar la atención que reciben los pacientes una vez que ingresan por primera vez, evitando altas erróneas, optimizando recursos hospitalarios.

## Dataset

Los datos se pueden encontrar en [UCI ML Repository](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008). Clore, J., Cios, K., DeShazo, J., & Strack, B. (2014). *Diabetes 130-US Hospitals for Years 1999-2008* [Dataset]. UCI Machine Learning Repository. [https://doi.org/10.24432/C5230J](https://doi.org/10.24432/C5230J).

Los datos con los que estamos trabajando en este proyecto no son de la mejor calidad, pues se incluyen valores faltantes, características irrelevantes y datos inconsistentes. Esto es así pues el tratamiento de datos complejos también forma parte del desarrollo del proyecyo. Además, incluye tanto valores numéricos como categóricos. Por lo tanto, uno de los principales objetivos de este proyecto es realizar un tratamiento completo de los datos.

## Estructura

**'readmpred.ipynb'**

En este notebook se desarrolla todo el proyecto, el cual está organizado en las siguientes secciones:

- **Procesamiento de los datos**:
  - Tratamiento de los datos faltantes.
  - Conversión de datos categóricos a numéricos.
  - Representaciones one-hot para variables categóricas.

- **Selección de características mediante dos métodos**:
  - **Visualización gráfica**: Se utilizan técnicas como boxplots, histogramas, la matriz de correlación y análisis de correlación con la variable respuesta.
  - **Métodos de envoltura (RFE)**: Selección de características basada en la importancia y rendimiento de cada una en los modelos.

- **Entrenamiento y elección del mejor modelo**:
  - Se entrenan y comparan los siguientes modelos:
    - **Logistic Regression Multinomial**.
    - **Random Forest**.
    - **Decision Trees**.

Cada sección sigue un enfoque estructurado para asegurar una correcta preparación, análisis y modelado de los datos, con el objetivo final de predecir los reingresos de pacientes.


 
