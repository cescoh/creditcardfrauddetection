# Deteccion de Fraudes de tarjetas de credito
Es importante que las empresas de tarjetas de credito puedan reconocer transacciones fraudulentas para que a los clientes no se les cobre por articulos que no compraron. 

El conjunto de datos contiene transacciones realizadas con tarjetas de crédito en septiembre de 2013 por titulares de tarjetas europeos.
Este conjunto de datos presenta transacciones que ocurrieron en dos días, donde tenemos 492 fraudes de 284.807 transacciones. El conjunto de datos está altamente desbalanceado, la clase positiva (fraudes) representa el 0,172% de todas las transacciones.

Contiene solo variables de entrada numéricas que son el resultado de una transformación de PCA. Desafortunadamente, debido a problemas de confidencialidad, no se proporcionan las características originales y más información de fondo sobre los datos. Las características V1, V2, … V28 son los componentes principales obtenidos con PCA, las únicas características que no se han transformado con PCA son 'Tiempo' y 'Monto'. La característica 'Tiempo' contiene los segundos transcurridos entre cada transacción y la primera transacción en el conjunto de datos. La característica 'Monto' es el Monto de la transacción, esta característica se puede utilizar para el aprendizaje sensible al costo dependiente del ejemplo. La característica 'Clase' es la variable de respuesta y toma el valor 1 en caso de fraude y 0 en caso contrario.

Se exploraron y procesaron los datos, se aplicaron varios modelos de machine learning para predecir operaciones fraudulentas incluidos Logistic Regression, Isolation Forest y Local Outlier Factor.
Se evaluaron los rendimientos de estos modelos utilizando metricas de clasificacion comunes y se midió la precisión utilizando el área bajo la curva de precisión-recuperación (AUPRC) ya que la precisión de la matriz de confusión no es significativa para la clasificación no balanceada.

Link del dataset: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
