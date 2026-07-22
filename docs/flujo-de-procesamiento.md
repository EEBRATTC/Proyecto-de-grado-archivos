# Flujo de procesamiento

La adquisición se realizó con MindWave Mobile 2 y la cadena de software asociada, que exportó los CSV EEG. El procesamiento posterior siguió este orden:

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

La consolidación del paso 2 combina subbandas dentro de cada fila y ocurre antes del PCA. La mediana del paso 7 es la consolidación final de las métricas por muestra y ocurre después del PCA y del cálculo e integración de métricas por fila. Son operaciones diferentes.

La selección de `Sensibilidad_Relajacion` responde a una comparación secundaria por categorías, su integración híbrida de valence y la pertinencia para el interés exploratorio sobre estímulos turísticos positivos. No se interpreta como superioridad estadística general ni como detección emocional directa o determinística. Antes de cualquier publicación se revisan humanamente los resultados agregados.

Los scripts que implementan este flujo permanecen en GitHub privado; los datos y resultados completos permanecen en GitLab privado. El acceso a ambos se controla por separado.
