# Diseño de Máquinas de Estados

Las máquinas de estados finitos se utilizan ampliamente en sistemas embebidos para estructurar el comportamiento.

Permiten representar comportamientos complejos como transiciones entre estados bien definidos.

---

## Estructura básica

Una máquina de estados generalmente incluye:

- Un conjunto de estados
- Transiciones entre estados
- Eventos que desencadenan transiciones

---

## Por qué son útiles

Las máquinas de estados hacen que el comportamiento del sistema sea:

- Predecible
- Modular
- Más fácil de depurar

---

## Ejemplo en robótica

Los robots suelen implementar comportamientos como:

BUSCAR → ACERCAR → AGARRAR → RETORNO

Cada etapa puede representarse como un estado en el sistema.

---

## Relevancia en sistemas embebidos

Las máquinas de estados son especialmente útiles en sistemas embebidos donde el comportamiento determinista es importante.
