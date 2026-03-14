# Cuadrículas de Ocupación Probabilísticas: Mapeando lo Desconocido

El mapeo robótico es el proceso de transformar flujos de datos de sensores en una representación espacial del mundo. Las cuadrículas de ocupación proporcionan un marco probabilístico robusto para esta tarea.

## Representación de la Incertidumbre

El entorno se divide en una cuadrícula de celdas. Cada celda almacena la probabilidad de estar ocupada. Esto permite:

- **Actualizaciones Eficientes:** Las nuevas mediciones (de Lidar o Sonar) se suman a la probabilidad existente.

- **Gestión de lo Desconocido:** Las celdas pueden representar espacio "desconocido" cuando aún no lo hemos explorado, generalmente con una probabilidad inicial del 50 %.

## Mapeo como Ganancia de Información

Desde la perspectiva de la detección, el mapeo consiste en reducir la incertidumbre en el dominio espacial.

- **Espacio Desconocido:** Alta incertidumbre.

- **Espacio Mapeado:** Ganancia de información (sabemos si está libre u ocupado).

A medida que el robot explora, convierte los datos de alcance brutos y ruidosos en un mapa estructurado que puede utilizarse para planificar rutas y evitar obstáculos.
