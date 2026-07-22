# Anexo F — resultados agregados de calibración

## Archivo público

- `matriz_Sensibilidad_Relajacion.png` — matriz agregada por categoría de estímulo, sin nombres, alias ni puntos individuales.
- SHA-256 de fuente y copia: `723A3B64730248E2955AE2EDD1CD7B086227A8CA19F14AC744B5A3CB92AE98C4`.

## Resumen de las ocho configuraciones

Valores transcritos de la hoja agregada `11_Resumen_Modelos` de la auditoría oficial; no se recalcularon. Los valores completos permanecen en los resultados fuente y el redondeo a dos decimales se aplica únicamente a esta presentación pública.

| Configuración | Registros antes de SCORE | Registros después de SCORE | Coincidencia global (%) |
|---|---:|---:|---:|
| Original | 137 | 91 | 35,16 |
| PCA_Dominante | 137 | 91 | 35,16 |
| Beta_Dominante | 137 | 91 | 31,87 |
| Equilibrado | 137 | 91 | 36,26 |
| Pura_Fisiologia | 137 | 91 | 29,67 |
| Puro_Machine_Learning | 137 | 91 | 31,87 |
| Gamma_Dominante | 137 | 91 | 35,16 |
| Sensibilidad_Relajacion | 137 | 91 | 36,26 |

La auditoría describe la coincidencia como comparación entre la etiqueta de referencia y el cuadrante exploratorio. `Sensibilidad_Relajacion` y `Equilibrado` obtuvieron 36,26 % de coincidencia global. El criterio de selección de `Sensibilidad_Relajacion` quedó cerrado mediante una comparación secundaria por categorías:

- Para estímulos alegres ubicados en Felicidad / Excitación, `Sensibilidad_Relajacion` obtuvo 60,00 % y `Equilibrado` 53,33 %.
- Para estímulos desagradables ubicados en Tensión / Disgusto, `Sensibilidad_Relajacion` obtuvo 27,27 % y `Equilibrado` 18,18 %.
- `Equilibrado` presentó porcentajes superiores en las categorías triste y relajante.

La selección también consideró la integración híbrida de valence de `Sensibilidad_Relajacion` y su pertinencia respecto al interés exploratorio del estudio sobre estímulos turísticos positivos. La configuración está marcada en el script y activa en el Anexo G. Esta decisión no se presenta como superioridad estadística general ni como detección emocional directa o determinística.
