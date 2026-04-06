# Ingeniería de Sistemas Autónomos en Entornos de Incertidumbre

## Introducción

Los sistemas autónomos operan en entornos donde la incertidumbre es inevitable. Las mediciones de los sensores son ruidosas, los modelos del sistema son imperfectos y las restricciones de tiempo real limitan la precisión computacional. El desafío no es eliminar la incertidumbre, sino diseñar sistemas que sigan siendo fiables a pesar de ella.

Esta perspectiva cambia el enfoque de la optimización algorítmica a la robustez a nivel de sistema.

---

## De la Estimación a la Fiabilidad

Las técnicas de estimación de estado, como el filtrado bayesiano, proporcionan un marco matemático para inferir variables ocultas a partir de observaciones ruidosas. Sin embargo, en los sistemas del mundo real, la estimación es solo un componente de una arquitectura más amplia.

Un sistema que produce una estimación óptima bajo supuestos incorrectos aún puede fallar.

La fiabilidad no surge de una estimación perfecta, sino de cómo la estimación interactúa con el control, la toma de decisiones y las restricciones del sistema.

---

## Determinismo sobre la incertidumbre

Si bien la percepción es inherentemente probabilística, el comportamiento del sistema a menudo debe ser determinista.

Las máquinas de estados finitos, las transiciones basadas en reglas y la lógica de control estructurada proporcionan predictibilidad e inspeccionabilidad. Estos mecanismos permiten que los sistemas impongan restricciones de seguridad incluso cuando las estimaciones subyacentes son inciertas.

Esto crea una arquitectura en capas:

- Percepción probabilística
- Estructuras de decisión deterministas
- Actuación controlada

---

## Pensamiento a nivel de sistema

El diseño de sistemas autónomos requiere razonamiento en múltiples capas:

- Detección → observaciones parciales y con ruido
- Estimación → inferencia probabilística
- Control → retroalimentación y estabilidad
- Comunicación → sistemas asíncronos y distribuidos

Los fallos en una capa se propagan por todo el sistema. Diseñar sistemas fiables requiere comprender estas interacciones, no solo los componentes individuales.

---

## Fiabilidad como restricción de diseño

En entornos de alto riesgo, el objetivo no es el máximo rendimiento, sino un comportamiento predecible ante la incertidumbre.

Esto nos lleva a principios de diseño clave:

- Modelado explícito de la incertidumbre
- Validación de supuestos en condiciones reales
- Redundancia en los circuitos de detección y decisión
- Comportamiento a prueba de fallos en condiciones degradadas

---

## Conclusión

Los sistemas autónomos no se definen únicamente por sus algoritmos, sino por la arquitectura que los integra.

El objetivo no es construir sistemas que sean óptimos en teoría, sino sistemas que se mantengan estables, interpretables y fiables cuando la teoría se enfrenta a la realidad.
