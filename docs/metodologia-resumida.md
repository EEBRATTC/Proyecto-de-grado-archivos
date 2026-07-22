# Metodología resumida

## Orden metodológico confirmado

1. Validación y limpieza de cada fila.
2. Consolidación de subbandas EEG por fila.
3. Cálculo de cocientes fisiológicos por fila.
4. Estandarización de las variables correspondientes.
5. Aplicación del PCA sobre las filas válidas de cada muestra.
6. Integración y cálculo de métricas fisiológicas por fila.
7. Consolidación final por muestra mediante mediana.
8. Aplicación del criterio `SCORE >= 6`, únicamente en la primera etapa del Anexo F.
9. Normalización mediante Z-Score por participante.
10. Proyección en el modelo de Russell.
11. Evaluación de las configuraciones y selección de `Sensibilidad_Relajacion`.
12. Aplicación de la configuración seleccionada en la segunda etapa del Anexo G, sin filtro por score.
13. Integración y comparación EEG–encuesta.

La consolidación de subbandas se realiza en cada fila antes de la estandarización y el PCA. Es una operación distinta de la consolidación final por muestra mediante mediana, que ocurre después del PCA y de la integración y cálculo de las métricas fisiológicas por fila.

## Anexo F: calibración

La primera etapa recorre los pasos 1 a 11. Las etiquetas de referencia proceden de `scores.csv`, y `SCORE >= 6` se aplica solo después de la consolidación final por muestra. `Sensibilidad_Relajacion` y `Equilibrado` alcanzaron 36,26 % de coincidencia global. La selección de `Sensibilidad_Relajacion` se sustentó en una comparación secundaria por categorías, su integración híbrida de valence y la pertinencia para el interés exploratorio sobre estímulos turísticos positivos; no implica superioridad estadística general ni detección emocional directa o determinística.

## Anexo G: EEG–encuesta

La segunda etapa reutiliza la configuración seleccionada y no aplica filtro por score. Después de procesar las filas, aplicar PCA, calcular las métricas por fila y consolidar finalmente cada muestra mediante mediana, normaliza por participante, proyecta en Russell e integra la encuesta mediante claves normalizadas de usuario y vídeo para producir comparaciones por signo y correlaciones.

## Límites de interpretación

- Los cuadrantes de Russell son categorías exploratorias, no diagnósticos.
- La encuesta es una fuente subjetiva complementaria, no una verdad absoluta.
- No se recalcularon resultados durante la organización documental.
- Fórmulas, pesos, umbrales, tratamiento de ceros y reglas metodológicas permanecen sin modificaciones en el GitHub privado de scripts; los datos y resultados completos permanecen en GitLab privado.
