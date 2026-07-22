# Diccionario público de datos

Los CSV crudos no se publican. El esquema observado en ambas etapas contiene:

| Campo | Descripción general |
|---|---|
| `Timestamp` | Marca temporal del registro. Unidad/formato: **PENDIENTE DE CONFIRMACIÓN**. |
| `blink_strength` | Intensidad de parpadeo reportada por el sistema. |
| `PoorSignalLevel` | Indicador de calidad de señal del dispositivo. |
| `Attention` | Métrica propietaria o derivada reportada por la cadena de adquisición. |
| `Meditation` | Métrica propietaria o derivada reportada por la cadena de adquisición. |
| `Delta`, `Theta` | Valores de bandas EEG. Unidad/escala: **PENDIENTE DE CONFIRMACIÓN**. |
| `LowAlpha`, `HighAlpha` | Componentes de banda alfa. |
| `LowBeta`, `HighBeta` | Componentes de banda beta. |
| `LowGamma`, `HighGamma` | Componentes de banda gamma. |

Esta descripción no publica valores individuales ni afirma una interpretación clínica.
