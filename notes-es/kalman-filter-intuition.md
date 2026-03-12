# Intuición del Filtro de Kalman

El filtro de Kalman es un algoritmo que se utiliza para estimar el estado de un sistema dinámico a partir de mediciones con ruido.

Se utiliza ampliamente en robótica, sistemas de navegación y aplicaciones de detección integrada.

---

## Idea central

Un sistema normalmente tiene:

- un **modelo de predicción**
- **mediciones con ruido**

El filtro de Kalman combina ambas fuentes de información para estimar el estado más probable.

---

## Dos fases

### Predicción

El modelo del sistema predice el siguiente estado:

- posición
- velocidad
- variables del sistema

Esta predicción se basa en estimaciones previas y en la dinámica del sistema.

---

### Actualización

Cuando se recibe una medición, el filtro actualiza la estimación combinando:

- estado predicho
- medición del sensor

El algoritmo asigna un peso en función de la **incertidumbre** de cada fuente.

---

## Por qué funciona

El filtro funciona porque modela:

- Incertidumbre del proceso
- Incertidumbre de la medición

Mediante matrices de covarianza, determina el grado de confianza en la predicción frente a la medición.

---

## Por qué es importante en robótica

Los robots rara vez observan el mundo a la perfección.

Los sensores son ruidosos, tienen retrasos y, a veces, poco fiables.

Los filtros de Kalman permiten a los robots mantener estimaciones estables de:

- Posición
- Velocidad
- Orientación
- Estado del sistema
