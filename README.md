# Análisis y Predicción de Cancelación de Clientes en Telecom X

## Objetivo del Proyecto

El objetivo de este proyecto es desarrollar modelos predictivos para identificar a los clientes con mayor probabilidad de cancelar sus servicios en Telecom X. La empresa busca anticiparse a la cancelación de clientes y tomar acciones proactivas de retención.

## Metodología

El proyecto siguió los siguientes pasos:

1.  **Carga y Exploración de Datos:** Se cargó el conjunto de datos `telecomx_data_processed.csv` y se realizó una exploración inicial para entender su estructura y características.
2.  **Preprocesamiento de Datos:** Los datos fueron preparados para el modelado, incluyendo la codificación de variables categóricas (One-Hot Encoding) y la escalación de variables numéricas (StandardScaler). La variable objetivo 'Abandono' fue codificada numéricamente.
3.  **Análisis de Correlación y Selección de Variables:** Se analizó la correlación entre variables numéricas y se utilizó la Información Mutua para evaluar la importancia de las características categóricas y numéricas. Se seleccionaron las top 20 características basadas en Información Mutua para el modelado.
4.  **División de Datos:** El conjunto de datos preprocesado fue dividido en conjuntos de entrenamiento (80%) y prueba (20%) para evaluar el rendimiento de los modelos en datos no vistos.
5.  **Entrenamiento de Modelos:** Se entrenaron dos modelos de clasificación: Regresión Logística y Bosque Aleatorio.
6.  **Evaluación de Modelos:** Se evaluó el rendimiento de ambos modelos utilizando métricas como Precisión, Recall, F1-score y Área bajo la Curva (AUC).
7.  **Interpretación de Resultados:** Se interpretaron los resultados de los modelos, incluyendo la importancia de las características para el Bosque Aleatorio y los coeficientes para la Regresión Logística, para identificar los factores clave que influyen en la cancelación.
8.  **Conclusión Estratégica:** Se resumieron los hallazgos clave y se proporcionaron recomendaciones estratégicas basadas en el análisis.

## Hallazgos Clave

*   Los clientes con **contratos mes a mes** tienen una mayor probabilidad de cancelar.
*   La **antigüedad** del cliente es un factor importante, con clientes de menor antigüedad más propensos a cancelar.
*   Los **cargos mensuales y totales** elevados están asociados con una mayor probabilidad de cancelación.
*   Los clientes con servicio de **fibra óptica** muestran una mayor tendencia a cancelar.
*   La **falta de servicios adicionales** (Soporte Técnico, Seguridad Online) se relaciona con una mayor probabilidad de cancelación.
*   El uso de **cheque electrónico** como método de pago también está asociado con una mayor probabilidad de cancelación.

## Rendimiento de los Modelos

Ambos modelos (Regresión Logística y Bosque Aleatorio) mostraron un rendimiento razonable en la predicción de cancelación, con valores de AUC superiores a 0.80. La Regresión Logística tuvo métricas de precisión y recall ligeramente superiores en este caso particular.

## Recomendaciones Estratégicas

1.  Incentivar contratos a largo plazo.
2.  Mejorar la experiencia del cliente durante los primeros meses.
3.  Revisar la estructura de precios y ofrecer opciones más flexibles.
4.  Investigar las causas de cancelación en clientes con fibra óptica.
5.  Promocionar y destacar el valor de los servicios adicionales.
6.  Optimizar la experiencia con el método de pago de cheque electrónico.
7.  Utilizar los modelos predictivos para identificar clientes de alto riesgo y aplicar campañas de retención personalizadas.

## Próximos Pasos

*   Desplegar el modelo predictivo en un entorno de producción.
*   Monitorear continuamente el rendimiento del modelo y actualizarlo periódicamente.
*   Implementar las recomendaciones estratégicas y medir su impacto en la tasa de cancelación.
*   Explorar otros modelos y técnicas de modelado para mejorar la precisión predictiva.
