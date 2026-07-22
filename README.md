# Esquema de trabajo para la toma de decisiones en turismo mediante EEG y minería de datos

Repositorio público de consulta del proyecto de grado **“Esquema de trabajo para la toma de decisiones en el sector turismo de la ciudad de Cartagena, combinando lectura de electroencefalogramas con técnicas de minería de datos no supervisadas”**.

Versión documental: **1.0.0**. La fecha definitiva de publicación se fijará únicamente el día real de publicación.

## Equipo académico

- **Eduardo José Ebratt Cancino**, estudiante de Ingeniería de Sistemas.
- **José Ignacio Gabriel Pardo Paternina**, estudiante de Ingeniería de Sistemas.
- **Tutor:** Juan Carlos García Ojeda.
- **Afiliación:** Universidad de Cartagena.
- **Programa:** Ingeniería de Sistemas.
- **Ciudad y año:** Cartagena de Indias, Colombia, 2026.
- **Contacto público:** [eebratt12@gmail.com](mailto:eebratt12@gmail.com).

Los autores no se presentan como ingenieros titulados. Ninguno posee un ORCID confirmado.

## Propósito público

Este repositorio prioriza documentación, manuales, arquitectura, dependencias, preparación de descargas, citación y evidencia agregada. No contiene scripts Python, CSV EEG crudos, `scores.csv`, `resultados_entrevista.csv`, auditorías completas, bases integradas, datos por participante ni resultados individualizados.

Los scripts se conservan en un repositorio privado de GitHub. El acceso puede solicitarse a los autores mediante `eebratt12@gmail.com` o concederse mediante invitación directa a una persona específica. Toda solicitud será evaluada por los autores y no garantiza acceso. La autorización estará sujeta a las condiciones académicas, institucionales, de privacidad y reutilización aplicables.

La URL del repositorio privado de scripts no se publica aquí. Los datos y resultados completos se mantienen en un repositorio privado separado.

## Resumen del proyecto

El proyecto estudia señales EEG obtenidas en un contexto turístico de Cartagena de Indias y propone un esquema de trabajo que combina su procesamiento con técnicas de minería de datos no supervisadas para apoyar análisis exploratorios orientados a la toma de decisiones. Las métricas fisiológicas y los cuadrantes de Russell no constituyen diagnósticos clínicos ni clasificaciones emocionales definitivas.

### Primera etapa — Anexo F

Se validó y limpió cada fila; se consolidaron sus subbandas EEG; se calcularon los cocientes fisiológicos; se estandarizaron las variables; y se aplicó PCA sobre las filas válidas de cada muestra. Después del PCA y del cálculo e integración de las métricas fisiológicas por fila se efectuó la consolidación final por muestra mediante mediana. Solo entonces se aplicó `SCORE >= 6`, seguido por Z-Score por participante, la proyección en Russell y la evaluación de ocho configuraciones.

`Sensibilidad_Relajacion` y `Equilibrado` alcanzaron una coincidencia global de 36,26 %. La selección de `Sensibilidad_Relajacion` se cerró mediante una comparación secundaria por categorías: obtuvo 60,00 % para estímulos alegres ubicados en Felicidad / Excitación frente a 53,33 % de `Equilibrado`, y 27,27 % para estímulos desagradables ubicados en Tensión / Disgusto frente a 18,18 %. `Equilibrado` presentó porcentajes superiores en las categorías triste y relajante. La decisión también consideró la integración híbrida de valence de `Sensibilidad_Relajacion` y su pertinencia para el interés exploratorio del estudio sobre estímulos turísticos positivos. No representa superioridad estadística general ni detección emocional directa o determinística.

### Segunda etapa — Anexo G

Se aplicó la configuración `Sensibilidad_Relajacion` a 96 CSV EEG sin filtro por score, respetando el procesamiento por fila, el PCA antes de la mediana final por muestra, la normalización Z-Score por participante y la proyección en Russell. Después se compararon los resultados con una encuesta de 96 registros. La base integrada privada contiene 93 correspondencias. Este repositorio solo conserva dos reportes globales y dos figuras agregadas que superaron revisión de nombres, identificadores y nivel de agregación.

## Arquitectura

```text
MindWave Mobile 2
        |
ThinkGear Connector 3.2.4.0 (NeuroSky, tercero)
        |
mindApp compilada con Unity 2022.3.41f1 / exportación CSV
        |
Scripts privados en GitHub
        |-- Anexo F: calibración
        `-- Anexo G: EEG y encuesta
        |
Datos, resultados completos y auditorías en GitLab privado
        |
Selección agregada autorizada en este repositorio público
```

Consulte la [arquitectura](docs/arquitectura-del-sistema.md), el [flujo](docs/flujo-de-procesamiento.md), la [metodología resumida](docs/metodologia-resumida.md), el [mapa de repositorios](REPOSITORY_MAP.md) y la [documentación de ThinkGear Connector](docs/dependencias/thinkgear-connector.md).

## Descargas y mindApp

- [`downloads/README.md`](downloads/README.md) documenta el estado de las descargas.
- [`docs/manuales/instalacion-mindapp.md`](docs/manuales/instalacion-mindapp.md) y [`docs/manuales/requisitos-mindapp.md`](docs/manuales/requisitos-mindapp.md) preparan una instalación futura.
- [`RELEASE_NOTES_MINDAPP.md`](RELEASE_NOTES_MINDAPP.md) y [`PLAN_RELEASE_MINDAPP.md`](PLAN_RELEASE_MINDAPP.md) son documentos preparatorios; no existe una GitHub Release.

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde al entorno Windows de 64 bits utilizado por el equipo; no constituye compatibilidad universal con todas las versiones de Windows ni una auditoría externa. Codex no ejecutó el binario. La aplicación fue desarrollada o compilada con Unity 2022.3.41f1, requiere hardware compatible MindWave Mobile 2 y su comunicación con el dispositivo depende de ThinkGear Connector, sujeto a las condiciones de NeuroSky.

`ENTRADA_CODEX/mindApp.rar` es la fuente original interna de la compilación. `RELEASE_CANDIDATES/mindApp-v1.0.0-windows.zip` no es una aplicación diferente ni fue reconstruida o recompilada por Codex: contiene la misma compilación extraída del RAR y reempaquetada en ZIP para facilitar su futura descarga y extracción en Windows, sin modificar la aplicación interna. El RAR se conservará en almacenamiento interno y no necesita publicarse junto con el ZIP. El ZIP permanece fuera de los tres repositorios y será el archivo principal propuesto para una futura GitHub Release de mindApp 1.0.0; todavía no fue publicado ni añadido al staging.

`Windows Setup Kit.zip` fue retirado del árbol de trabajo público y este repositorio no lo redistribuye. El paquete utilizado por el equipo se conserva únicamente como respaldo interno no publicable en `ENTRADA_CODEX/terceros_no_publicar/`. ThinkGear Connector pertenece a NeuroSky, Inc.; el equipo no lo desarrolló ni lo posee. Es una dependencia necesaria para la comunicación con MindWave Mobile 2 y debe obtenerse prioritariamente desde la fuente oficial de NeuroSky, conforme a sus términos y condiciones. ThinkGear Connector 3.2.4.0 fue identificado mediante los metadatos del ejecutable utilizado por el equipo. El paquete no se incluirá en la Release de `mindApp`.

`neuroExV6.6.zip` permanece clasificado como `TERCERO_NO_PUBLICAR / PENDIENTE_DE_CONFIRMACION` y no está en este repositorio.

## Resultados agregados seleccionados

- [Anexo F — calibración](results/calibration/README.md): matriz de `Sensibilidad_Relajacion` y resumen agregado de ocho configuraciones.
- [Anexo G — EEG y encuesta](results/eeg-survey/README.md): correlaciones globales, coincidencia global por signo, dos figuras agregadas y síntesis por video.

La figura Russell global fue rechazada porque contiene alias y puntos individualizables. No se publicaron gráficos por participante, bases individuales ni auditorías completas.

## Privacidad, disponibilidad y reproducibilidad

- [Seguridad y privacidad](SECURITY_AND_PRIVACY.md)
- [Disponibilidad de datos](docs/disponibilidad-de-datos.md)
- [Disponibilidad del software](docs/disponibilidad-del-software.md)
- [Reproducibilidad](docs/reproducibilidad.md)
- [Derechos y reutilización](RIGHTS_AND_REUSE.md)
- [Avisos de terceros](THIRD_PARTY_NOTICES.md)

## Citación

> Ebratt Cancino, E. J., & Pardo Paternina, J. I. G. (2026). *Esquema de trabajo para la toma de decisiones en el sector turismo de la ciudad de Cartagena, combinando lectura de electroencefalogramas con técnicas de minería de datos no supervisadas* (Versión 1.0.0) [Proyecto de grado]. Universidad de Cartagena. https://github.com/EEBRATTC/Proyecto-de-grado-archivos

Consulte [CITATION.md](CITATION.md) y [CITATION.cff](CITATION.cff). La disponibilidad pública no equivale a una licencia de código abierto.
