
**1. Descripción del Proyecto**

Este proyecto forma parte de mi Trabajo de Fin de Máster en Ciencia de Datos e Inteligencia Artificial.
El objetivo es desarrollar un modelo de inteligencia artificial capaz de predecir la ocupación diaria de un Bed & Breakfast de 9 habitaciones en Cataluña.

El modelo se entrena a partir del histórico de reservas y se complementa con variables externas que influyen en la demanda, tales como:

Datos climáticos (temperatura, precipitaciones, etc.).

Festivos nacionales y autonómicos.

Vacaciones escolares.

Eventos culturales y deportivos de gran impacto en la zona.

Métricas derivadas como la antelación media de reserva o la duración media de las estancias.

El objetivo final es anticipar la demanda para optimizar la gestión de precios, personal y recursos, mejorando así la rentabilidad del negocio.


**2. Contenidos del Repositorio**

- web_scraping_aemet (1).ipynb: 
Contiene los notebooks y scripts utilizados para la extracción de datos climáticos históricos desde la AEMET.

- Preprocesamiento_B&B.ipynb" 
Incluye el código donde se limpian y transforman los datos, generando nuevas variables y un dataset final listo para entrenar modelos.

- Predicción_ocupación_B&B.ipynb" 
Incluye el código que construye el modelo de aprendizaje automático con el objetivo de predecir la ocupación diaria del establecimiento turístico en función de una serie de variables.

- PowerBI.pbix: Dashboard interactivo en PowerBI.

- clima_completo.csv: dataframe extraido mediante el código de "web_scraping_aemet (1).ipynb". Contiene la temperatura media y la precipitación diaria de la estación de vilassar de dalt desde el 31/03/2021 hasta el 19/04/2025.
  
- df_final.csv: dataframe resultado de el código "Preprocesamiento_B&B.ipynb". Contiene la información necesaria para realizar el estudio de predicción.

- df_final_con_resultados: dataframe resultado de el código "Predicción_ocupación_B&B.ipynb". Contiene el dataframe a estudiar con sus predicciones y error.




**3. Consideraciones importantes**

Protección de datos: La base de datos en bruto del establecimiento no se publica en este repositorio, ya que contiene información personal de los clientes. Compartirla iría en contra de la normativa vigente en materia de protección de datos (RGPD). Por este motivo, únicamente se incluyen los datasets procesados que permiten la reproducción parcial del análisis sin comprometer datos sensibles.

Scraping de AEMET: El script desarrollado para recolectar datos meteorológicos desde la web de AEMET ya no funciona actualmente, dado que el histórico de datos ha dejado de estar disponible en dicha página. Sin embargo, en este repositorio se incluye el dataset ya descargado y depurado en su momento, que contiene la información climática utilizada en el proyecto.


**4. Tecnologías utilizadas**

Lenguaje principal: Python (Google Colab como entorno de desarrollo).

Librerías de análisis de datos: pandas, numpy.

Visualización: matplotlib, seaborn, Power BI.

Machine Learning: scikit-learn, XGBoost, SHAP.

Obtención de datos: BeautifulSoup, requests (para web scraping).

Control de versiones: Git + GitHub
📁 /modelado
Notebooks dedicados al entrenamiento, comparación y optimización de modelos de Machine Learning, junto con análisis
