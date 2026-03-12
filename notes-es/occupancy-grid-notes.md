# Mapeo de Cuadrículas de Ocupación

Las cuadrículas de ocupación son un método probabilístico que utilizan los robots para representar su entorno.

El mundo se divide en una cuadrícula de celdas, y cada celda almacena la probabilidad de estar ocupada.

---

## Concepto

Cada celda de la cuadrícula representa:

- espacio libre
- espacio ocupado
- espacio desconocido

El robot actualiza estas probabilidades utilizando las mediciones de sus sensores.

---

## Por qué funciona bien

Las cuadrículas de ocupación permiten a los robots construir mapas de forma incremental mientras se mueven.

Se utilizan comúnmente con sensores como:

- lidar
- sonar
- cámaras de profundidad

---

## Aplicaciones

Las cuadrículas de ocupación se utilizan ampliamente en:

- navegación de robots móviles
- sistemas SLAM
- planificación de rutas
- evasión de obstáculos

---

## Ventaja clave

Permiten a los robots razonar sobre la incertidumbre del entorno en lugar de asumir mediciones perfectas.
