# Anexo G — resultados globales EEG–encuesta

## Archivos públicos

| Archivo | Contenido | SHA-256 |
|---|---|---|
| `Reporte_Correlaciones_EEG_Encuesta.csv` | Cuatro correlaciones globales sobre 93 registros integrados | `FAF876673C2CBD5A3F4625B7F1008C159FAFCA747A7939FB3177DFFF3F9B7DC1` |
| `Reporte_Coincidencia_Por_Signo.csv` | Coincidencia global de valence y arousal | `B5A5AF3AB10E1379A536B801A86BF27BB7FA64289C67E992645D72133C918D1A` |
| `grafica_coincidencia_por_signo.png` | Figura global sin identificadores | `6D99558093013C04738628D6633D321B0C1D8ED73025F765F02384F9D803F9C6` |
| `grafica_distribucion_cuadrantes.png` | Conteo global por cuadrante | `78B9362390ED1967F2138D7B7B1D859952EBA8ABE62077E3980A1EDC35983245` |

Los hashes coinciden con las fuentes privadas. Ningún archivo contiene nombres, alias, claves de muestra ni filas individuales.

## Síntesis agregada por video

Valores transcritos de `18_Analisis_Por_Video` de la auditoría oficial; no se recalcularon. Los promedios se muestran con tres decimales y los porcentajes con dos únicamente para la presentación pública; los valores completos permanecen en los resultados fuente.

| Video | Registros | Promedio Valence_Z | Promedio Arousal_Z | Coincidencia valence (%) | Coincidencia arousal (%) |
|---|---:|---:|---:|---:|---:|
| video_1 | 11 | 0,541 | -0,139 | 66,67 | 0,00 |
| video_2 | 12 | -0,120 | 0,898 | 40,00 | 75,00 |
| video_3 | 12 | -0,450 | -0,129 | 10,00 | 55,56 |
| video_4 | 12 | -0,705 | -0,141 | 18,18 | 54,55 |
| video_5 | 12 | 0,596 | -0,284 | 100,00 | 14,29 |
| video_6 | 11 | 0,751 | 0,227 | 87,50 | 62,50 |
| video_7 | 12 | -0,268 | 0,197 | 37,50 | 57,14 |
| video_8 | 11 | -0,258 | -0,679 | 42,86 | 33,33 |

## Correlaciones globales

Coeficientes transcritos del reporte global de 93 registros integrados y redondeados a tres decimales solo para esta presentación. La precisión completa permanece en `Reporte_Correlaciones_EEG_Encuesta.csv`.

| Comparación | Pearson | Spearman |
|---|---:|---:|
| Valence EEG vs. valence encuesta | -0,076 | -0,112 |
| Arousal EEG vs. arousal encuesta | -0,106 | -0,086 |
| Valence EEG vs. ranking encuesta | 0,112 | 0,123 |
| Arousal EEG vs. ranking encuesta | 0,142 | 0,156 |

## Coincidencia global por signo

Porcentajes transcritos del reporte global y redondeados a dos decimales solo para esta presentación. La precisión completa permanece en `Reporte_Coincidencia_Por_Signo.csv`.

| Dimensión | Registros no neutrales | Coincidencias | Porcentaje de coincidencia (%) |
|---|---:|---:|---:|
| Valence | 68 | 31 | 45,59 |
| Arousal | 59 | 29 | 49,15 |

Las correlaciones y coincidencias son exploratorias y no constituyen medición directa ni diagnóstico emocional. `grafica_russell_global.png` no se publicó: pese al nombre “global”, muestra alias en la leyenda y observaciones individualizables. Las 12 figuras por participante, la base integrada, el reporte por registro y la auditoría completa también fueron rechazados para publicación.
