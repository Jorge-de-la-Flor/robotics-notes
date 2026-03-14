# Control PID: La base de los sistemas de retroalimentación

El controlador Proporcional-Integral-Derivativo (PID) es el mecanismo de retroalimentación más utilizado en robótica. Calcula continuamente un valor de "error" como la diferencia entre un punto de consigna deseado y una variable medida.

## Los tres componentes

- **Proporcional (P):** Reacciona al error actual. Si el error es grande, la corrección es fuerte. Proporciona la "fuerza" de la respuesta.

- **Integral (I):** Acumula los errores pasados. Es esencial para eliminar el "error en estado estacionario", esas pequeñas desviaciones que el término proporcional por sí solo no puede corregir.

- **Derivativo (D):** Predice el error futuro analizando su tasa de cambio. Actúa como un "amortiguador", evitando que el sistema se sobrepase y oscile.

## Estabilidad y ajuste

La excelencia de un controlador no reside solo en alcanzar el objetivo, sino en cómo lo logra. Un controlador PID bien ajustado equilibra la velocidad (tiempo de subida) con la estabilidad (amortiguación), asegurando que el robot se mueva con suavidad y sin esfuerzos mecánicos.

## Aplicaciones en Robótica

Los bucles PID están presentes en todas partes: desde mantener las RPM de un motor hasta estabilizar el vuelo de un cuadricóptero o el agarre preciso de un brazo quirúrgico.
