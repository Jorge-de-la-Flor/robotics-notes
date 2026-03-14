# El filtro de Kalman: Una intuición de la estimación óptima

El filtro de Kalman es el algoritmo definitivo para el seguimiento y la estimación en sistemas lineales. No es simplemente un filtro, sino un método matemático para encontrar el estado más probable de un sistema.

## La lógica central: Confianza vs. Verificación

El filtro opera en un ciclo continuo de predicción y actualización, mediado por un factor de "ganancia":

- Si nuestros sensores son muy precisos, el filtro confía más en la medición.

- Si nuestro modelo de movimiento es muy preciso, pero los sensores son ruidosos, el filtro confía más en la predicción.

## Por qué es "óptimo"

El filtro de Kalman está diseñado para minimizar el error cuadrático medio de la estimación. Mantiene una "matriz de covarianza" que representa la incertidumbre del sistema. Al minimizar esta incertidumbre, garantiza que la estimación resultante sea la representación estadísticamente más certera posible de la realidad.

## Aplicación en robótica

En la robótica moderna, este es el pilar de la fusión de sensores. Permite a los robots mantener una posición y una dirección estables incluso cuando los sensores individuales proporcionan información contradictoria o ruidosa.
