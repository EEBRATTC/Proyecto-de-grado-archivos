# Descargas

## Estado actual

- No existe una GitHub Release de `mindApp`.
- El candidato `mindApp-v1.0.0-windows.zip` está preparado fuera de este repositorio en `RELEASE_CANDIDATES/` y no está staged ni publicado.
- El SHA-256 del candidato actual se documenta en [`checksums/mindApp-v1.0.0-windows.sha256`](checksums/mindApp-v1.0.0-windows.sha256).
- El candidato contiene la misma compilación de `ENTRADA_CODEX/mindApp.rar`, extraída y reempaquetada como ZIP para facilitar su descarga y extracción en Windows; no fue reconstruida, recompilada ni modificada internamente por Codex.
- El RAR es la fuente original interna y permanecerá en almacenamiento interno. El ZIP es el paquete de distribución propuesto; no es necesario publicar ambos.
- El candidato contiene aproximadamente `MindwaveUnity.exe`, `MindwaveUnity_Data/`, bibliotecas generadas por Unity, recursos, configuración y demás componentes de la compilación original. No contiene código fuente de Unity.
- No incluye `mindApp.rar`, `Windows Setup Kit.zip`, `neuroExV6.6.zip`, scripts privados, CSV, `scores.csv`, `resultados_entrevista.csv`, resultados de los anexos, auditorías ni documentos académicos.

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde al entorno Windows de 64 bits utilizado por el equipo, no constituye compatibilidad universal ni auditoría externa y Codex no ejecutó el binario. La aplicación fue desarrollada o compilada con Unity 2022.3.41f1. Requiere MindWave Mobile 2 compatible y ThinkGear Connector, cuyo uso permanece sujeto a las condiciones de NeuroSky.

## Futura GitHub Release

La futura Release corresponderá a mindApp 1.0.0, se asociará posteriormente a la etiqueta `v1.0.0` y tendrá `mindApp-v1.0.0-windows.zip` como archivo principal. Permitirá descargar la aplicación sin incorporar los 153 archivos individualmente al historial ordinario. Incluirá notas de versión, instalación, requisitos, SHA-256, reconocimientos y avisos de terceros; podrá crearse primero como borrador y solo publicarse tras aprobación humana. No se ha creado la etiqueta ni la Release y el ZIP no se ha publicado.

## Dependencias

La aplicación requiere MindWave Mobile 2 y ThinkGear Connector. Obtenga software y controladores de NeuroSky desde fuentes oficiales y respete sus licencias. Este proyecto no afirma propiedad sobre esos componentes.

El repositorio público no redistribuye `Windows Setup Kit.zip`: fue retirado del árbol de trabajo y se conserva únicamente como respaldo interno no publicable. Las instrucciones de instalación permanecen disponibles, pero el usuario debe obtener ThinkGear Connector desde la fuente oficial de NeuroSky y utilizarlo conforme a sus condiciones. El archivo no forma parte de la futura Release de `mindApp`.

Consulte los [requisitos](../docs/manuales/requisitos-mindapp.md), la [instalación](../docs/manuales/instalacion-mindapp.md) y el [plan de Release](../PLAN_RELEASE_MINDAPP.md).
