Análisis de Ventas en Retail: Identificando Factores Clave
Descripción del Proyecto:
El objetivo de este proyecto es analizar los datos de ventas de retail para identificar los factores que influyen en el comportamiento de los clientes. El análisis busca ofrecer insights útiles para optimizar las estrategias comerciales y mejorar la toma de decisiones en la empresa. A través de un análisis profundo de las transacciones, se pretende entender mejor las relaciones entre categorías de productos, métodos de pago, satisfacción del cliente y métodos de envío.

El dataset utilizado contiene información de más de 300,000 transacciones de retail, incluyendo detalles sobre clientes, productos, métodos de pago y feedback de clientes.

Hipótesis Principales:
Las categorías relacionadas con electrónica y ropa tienen un valor promedio de compra más alto que otras categorías.
Las transacciones realizadas con tarjeta de crédito tienden a ser de un monto mayor en comparación con otros métodos de pago.
Los métodos de envío más rápidos resultan en mejores calificaciones de satisfacción por parte del cliente.
El género influye en las preferencias de productos, con una mayor preferencia por ciertas categorías dependiendo del género.
Pasos del Análisis:
1. Exploración y Limpieza de los Datos:
Se realizaron varias transformaciones para preparar los datos, eliminando columnas irrelevantes como Name, Email, Phone, que no aportaban al análisis principal.
Se manejaron valores faltantes mediante eliminación o imputación de valores, dependiendo de su importancia para el análisis.
2. Análisis Exploratorio de Datos (EDA):
Visualizaciones de datos para explorar las relaciones entre distintas variables:
Ventas por categoría y método de pago: Electrónica y ropa mostraron montos más altos, mientras que los métodos de pago con tarjeta de crédito tendieron a asociarse con compras de mayor valor.
Distribución de monto de compra por género: No se observó una diferencia significativa en el valor total de compra entre géneros.
Métodos de envío y satisfacción del cliente: Los métodos de envío más rápidos, como Same-Day, estuvieron relacionados con una mayor satisfacción del cliente.
3. Reducción de Dimensionalidad:
Se aplicaron técnicas de feature selection utilizando la importancia de las características mediante un modelo de Random Forest.
Las variables más importantes fueron el número total de compras (Total_Purchases) y el monto parcial (Amount).
4. Modelado:
Random Forest y Regresión Lineal fueron los algoritmos elegidos para predecir el monto total de las transacciones.
Random Forest demostró ser el modelo superior, con un R² cercano a 1 y errores significativamente bajos en comparación con la Regresión Lineal.
5. Validación y Evaluación:
Se utilizó validación cruzada (5 folds) para asegurar la robustez del modelo, mostrando un R² promedio de 0.9999 para Random Forest.
El conjunto de prueba confirmó que el modelo de Random Forest capturó mejor la complejidad del problema, con un MSE de 186.45 y un R² de 0.9998, mientras que la regresión lineal tuvo un MSE significativamente mayor.
Conclusiones:
Random Forest superó significativamente a la Regresión Lineal en la predicción del monto total de las compras. Esto sugiere que el modelo Random Forest puede capturar de manera más efectiva las interacciones complejas entre las diferentes características del dataset.

Las categorías de productos como electrónica y ropa muestran un valor de compra promedio más alto, lo que confirma la hipótesis inicial. Estos resultados pueden guiar estrategias de marketing y promociones dirigidas a estas categorías.

Los métodos de envío rápidos, como Same-Day, se correlacionan con mayores calificaciones de satisfacción, lo que sugiere que la empresa podría beneficiarse al optimizar y promover estas opciones de envío para mejorar la experiencia del cliente.

A pesar de las expectativas, no se observó una diferencia significativa en el monto de compra por género. Ambos géneros presentaron comportamientos de compra similares en cuanto al valor total de sus transacciones.

Recomendaciones:
Optimizar las opciones de envío: Dado que el envío más rápido está relacionado con una mayor satisfacción del cliente, sería recomendable mejorar la logística para ofrecer más opciones rápidas como Same-Day.

Enfocar campañas de marketing: Las categorías de productos con un ticket promedio más alto, como electrónica y ropa, podrían ser el objetivo de campañas de marketing específicas para aumentar las ventas.

Seguir monitoreando el comportamiento de los métodos de pago: El hecho de que las compras realizadas con tarjeta de crédito tiendan a ser de mayor valor puede ayudar a diseñar estrategias de fidelización que incentiven el uso de este método.

Este proyecto mostró cómo el análisis de datos y la implementación de modelos de machine learning pueden ayudar a entender mejor el comportamiento del cliente en el sector retail. Las recomendaciones obtenidas podrían ayudar a optimizar las estrategias comerciales y mejorar la experiencia del cliente, basadas en el análisis de datos históricos.
