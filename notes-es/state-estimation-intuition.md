# Estimación de estado: Inferir la realidad a partir del ruido

En robótica, el "estado" representa el conjunto de variables ocultas —como la posición, la velocidad y la orientación— que definen la condición de un sistema. El desafío fundamental de la robótica radica en que el estado nunca es directamente observable; debe inferirse a partir de datos incompletos y ruidosos.

## La realidad de la observabilidad parcial

Los sensores físicos no proporcionan la "verdad"; proporcionan evidencia ruidosa con limitaciones inherentes:

- **Sensores externos (GPS/Lidar):** Proporcionan referencias absolutas, pero sufren interferencias, oclusiones y bajas tasas de muestreo.

- **Sensores internos (IMU/Codificadores):** Esenciales para actualizaciones de alta frecuencia, pero propensos a la deriva de integración con el tiempo.

## El marco bayesiano recursivo

La estimación de estado se trata como un proceso recursivo. Mantenemos una distribución de probabilidad (creencia) sobre el estado y la refinamos a medida que llega información:

1. **Predicción:** Utilizamos un modelo de movimiento para proyectar dónde debería estar el robot. Este paso aumenta naturalmente la incertidumbre a medida que el sistema se mueve.

2. **Corrección:** Integramos nuevas observaciones de sensores para ajustar la estimación a la realidad, reduciendo así la incertidumbre del sistema.

## Importancia en la Autonomía

Una estimación de estado robusta es un requisito previo para la autonomía de alto nivel. Ya sea una herramienta quirúrgica o un vehículo autónomo, la capacidad de integrar datos inconsistentes en una única y fiable "Fuente de Verdad" es lo que define un sistema robótico de misión crítica.
