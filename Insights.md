**FECHA:** 22 de noviembre de 2025

**PARA:** Gerencia General y Junta Directiva, HabitAlpes

**DE:** Equipo de Ciencia de Datos (Juan Carlos Cepeda y Jose Daniel Molano)

**ASUNTO:** Informe Ejecutivo – Resultados y Viabilidad del Modelo de Automatización de Avalúos

Estimados miembros de la dirección:

Por medio de la presente, hacemos entrega de los resultados finales del proyecto de analítica de datos enfocado en la optimización del proceso de avalúos de inmuebles. El objetivo de este estudio fue determinar la viabilidad técnica y financiera de asistir el proceso de valoración mediante algoritmos de Machine Learning.

A continuación, detallamos los hallazgos clave y nuestra recomendación estratégica para el negocio.

**Recomendaciones**

Se recomienda a HabitAlpes **implementar el modelo de predicción (Random Forest)** bajo un esquema **híbrido de "Human-in-the-loop"**, con las siguientes consideraciones:

* **Segmentación de Lujo:** Los inmuebles con valor superior a **$2.800 millones** (aprox. 8% de la cartera) deben seguir siendo avaluados manualmente por expertos, dado su alto valor y particularidades.
* **Automatización Inteligente:** Recomendamos desplegar el modelo para el segmento estándar, donde el algoritmo demuestra alta fiabilidad. Esto nos permite automatizar aproximadamente el **63% del volumen total** de solicitudes de manera segura.
* **Gestión de Riesgo:** Aquellos casos donde el modelo detecte alta incertidumbre o diferencias críticas de precio serán derivados automáticamente a revisión humana, evitando reclamos por subestimación.
* **Gobierno de datos:** ⁠Los resultados obtenidos subrayan la necesidad de continuar fortaleciendo la gestión de los datos, ya que la presencia de valores atípicos tiene un efecto directo sobre la estabilidad del modelo y su capacidad para reducir costos operativos.

**Soporte a las recomendaciones**

La implementación de esta tecnología transforma radicalmente nuestra estructura de costos y eficiencia:

* **Eficiencia:** Reducción del tiempo de avalúo de **6 horas a 1 hora** por inmueble.
* **Ahorro Directo:** Se genera un ahorro de **$47.500 COP** por cada transacción automatizada.

**Proyección Financiera:**
El análisis de rentabilidad, asumiendo un costo de mantenimiento (salario de Científico de Datos por $6.000.000), arroja los siguientes resultados:

* **Ganancia Neta Mensual:** **$2.322.730** .
* **Retorno de Inversión (ROI):** **39.36%** proyectado a 12 meses.
* **Recuperación de Inversión:** El proyecto se paga a sí mismo en **8.6 meses**

Estos resultados estan soportados en un juicioso y riguroso analisis financiero del cúal podemos ofrecer detalles según su requerimiento.

Es importante destacar que, más allá de la ganancia neta inmediata, el valor real radica en la **escalabilidad**: HabitAlpes podrá procesar un mayor volumen de solicitudes sin aumentar linealmente su planta de peritos.


**Solidez Técnica y Modelo Seleccionado**

Tras evaluar múltiples algoritmos de predicción, hemos determinado que el modelo **Random Forest Regressor** es la herramienta óptima para HabitAlpes.

* **Precisión:** El modelo logra explicar el **81.71% (R²)** de la variabilidad en los precios del mercado, un estándar alto para el sector inmobiliario.
* **Criterio Experto:** Confirmamos que el modelo "razona" de manera similar a un perito humano (Analisis Shapley y LIME). Las variables que más pesan en su decisión son, en orden: área construida, número de baños, ubicación geoespacial y estrato, pero, adicionalmente, también logra cuantificar pequeñas variables relevantes en el precio final como son sí el inmueble es nuevo, pertenece a un conjunto cerrado, entre otras. Esto garantiza que las valoraciones automáticas sigan una lógica de mercado coherente.
* **Puntos de mejora:** Finalmente, la variable de ubicación, aunque incorporada mediante clusterización, podría beneficiarse de un tratamiento alternativo que permita capturar de manera más precisa su correlación con el estrato y el precio, lo que abre la puerta a futuros ajustes basados en zonificación geográfica, categorización socioespacial o enriquecimiento con fuentes externas.

**Conclusión**

La adopción de este modelo es **financieramente sostenible y estratégicamente necesaria** . Recomendamos proceder con el despliegue del modelo bajo el esquema híbrido propuesto. Esto posicionará a HabitAlpes como una inmobiliaria tecnológicamente avanzada, capaz de responder con agilidad a la demanda del mercado mientras optimiza sus márgenes operativos.

Quedamos a su disposición para profundizar en cualquier detalle técnico o financiero de este informe.

Cordialmente,

**Equipo de Ciencia de Datos**
*Proyecto HabitAlpes*
