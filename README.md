# Telecom_x_2
📊 Telecom X - Modelo Predictivo de Cancelación de Clientes (Churn)

Este proyecto corresponde a la segunda etapa del Desafío Telecom X, en la cual se desarrolla un modelo de predicción para identificar clientes con alta probabilidad de cancelar el servicio (churn).

Partiendo de los datos previamente depurados y estructurados en la primera fase del proyecto, se implementaron diversas técnicas de preprocesamiento de datos, análisis exploratorio, modelado predictivo y evaluación de desempeño, con el objetivo de comprender los factores que influyen en la cancelación y anticipar este comportamiento mediante algoritmos de Machine Learning.

🎯 Objetivos

El desarrollo del proyecto tuvo como propósito principal construir un modelo que permita anticipar la cancelación de clientes. Para ello se plantearon los siguientes objetivos específicos:

Preparar y transformar los datos mediante procesos de limpieza, codificación de variables y eliminación de atributos irrelevantes.

Analizar la relación entre las variables del conjunto de datos y el fenómeno de cancelación.

Entrenar y comparar al menos dos modelos de predicción utilizando algoritmos diferentes.

Identificar las variables que tienen mayor impacto en la predicción del churn.

Proponer estrategias orientadas a mejorar la retención de clientes a partir de los resultados obtenidos.

🛠️ Tecnologías utilizadas

Para el desarrollo del análisis y la construcción de los modelos se emplearon las siguientes herramientas:

Python como lenguaje principal de programación.

Pandas y NumPy para la manipulación y procesamiento de datos.

Matplotlib y Seaborn para la visualización de información y análisis gráfico.

Scikit-Learn para el entrenamiento, validación y evaluación de modelos de aprendizaje automático.

Imbalanced-learn (SMOTE) para el tratamiento del desbalance en las clases del conjunto de datos.

📂 Flujo de trabajo

El proceso de desarrollo del modelo predictivo se llevó a cabo mediante las siguientes etapas:

Carga del conjunto de datos limpio, correspondiente al archivo datos_clientes_limpio.csv, generado en la primera fase del proyecto.

Preprocesamiento de los datos, que incluyó:

Eliminación de columnas sin relevancia para el modelo, como customerID.

Transformación de variables categóricas mediante técnicas de codificación como One-Hot Encoding.

Evaluación del balance entre clases y aplicación de SMOTE cuando fue necesario.

Análisis exploratorio de datos, donde se realizaron:

Matrices de correlación entre variables numéricas.

Análisis de relaciones específicas entre variables relevantes, como:

Tipo de contrato y cancelación.

Total de cargos y probabilidad de cancelación.

Construcción de modelos predictivos, considerando dos algoritmos principales:

Regresión Logística, que requiere normalización previa de los datos.

Random Forest, que permite trabajar con datos sin necesidad de normalización.

El conjunto de datos se dividió en 80 % para entrenamiento y 20 % para prueba.

Evaluación del desempeño de los modelos, utilizando métricas como:

Exactitud (Accuracy)

Precisión (Precision)

Sensibilidad (Recall)

Puntaje F1 (F1-score)

Matriz de confusión

Interpretación de resultados, mediante:

Análisis de coeficientes en la Regresión Logística.

Evaluación de la importancia de variables en el modelo Random Forest.

📊 Resultados principales

Los resultados obtenidos indican que el modelo de Random Forest presentó el mejor desempeño general, logrando un equilibrio adecuado entre precisión y capacidad de detección de clientes que cancelan el servicio.

Entre las variables con mayor influencia en la predicción de churn se identificaron:

Tipo de contrato: los clientes con contrato month-to-month presentan mayor tendencia a cancelar el servicio.

Método de pago: el uso de electronic check se relaciona con una mayor tasa de cancelación.

Tenure (antigüedad del cliente): los clientes con menor tiempo en la empresa muestran mayor probabilidad de abandono.

Cargos mensuales (Monthly Charges): valores elevados incrementan la probabilidad de cancelación.

Servicios adicionales: la ausencia de servicios como seguridad en línea o soporte técnico se asocia con mayores niveles de churn.

📝 Conclusiones y recomendaciones

El análisis realizado permite concluir que la cancelación de clientes está fuertemente relacionada con condiciones contractuales, métodos de pago y características del servicio ofrecido.

A partir de estos hallazgos, se proponen las siguientes estrategias para mejorar la retención de clientes:

Incentivar la migración hacia contratos de mayor duración, ofreciendo descuentos o beneficios adicionales.

Fomentar el uso de métodos de pago automáticos, como débito o tarjeta de crédito, que suelen estar asociados a menor churn.

Implementar programas de fidelización durante los primeros meses de servicio, periodo donde se observa mayor riesgo de cancelación.

Diseñar paquetes de servicios que incluyan valor agregado, como seguridad en línea y soporte técnico especializado
