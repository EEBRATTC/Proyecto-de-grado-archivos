# Notas preparatorias de mindApp 1.0.0 para Windows

Estado: **candidato local; no publicado**.

## Contenido propuesto

- `mindApp-v1.0.0-windows.zip` como archivo principal de la futura GitHub Release de mindApp 1.0.0, asociada posteriormente a la etiqueta `v1.0.0`.
- La misma compilación Unity existente en `ENTRADA_CODEX/mindApp.rar`, extraída y reempaquetada como ZIP sin reconstrucción, recompilación ni modificación interna por Codex.
- 153 archivos, preservados byte a byte respecto de la extracción del RAR original.
- Manuales públicos de instalación y requisitos.
- Checksum SHA-256 del candidato.
- Notas de versión, reconocimientos y avisos de terceros.

El RAR es la fuente original interna y permanecerá en almacenamiento interno; el ZIP es el paquete de distribución propuesto. No es necesario publicarlos simultáneamente. El ZIP contiene aproximadamente `MindwaveUnity.exe`, `MindwaveUnity_Data/`, bibliotecas generadas por Unity, recursos, configuración y los demás componentes necesarios de la compilación original. No contiene el código fuente de Unity.

## Validación disponible

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde a la plataforma Windows de 64 bits utilizada por el equipo, no demuestra compatibilidad universal ni constituye una auditoría externa. Codex no ejecutó el binario. La aplicación fue desarrollada o compilada con Unity 2022.3.41f1. La comparación del contenido del candidato contra la compilación original dio 0 archivos faltantes, 0 extras y 0 diferencias de hash.

## Limitaciones y dependencias

- Se requiere hardware compatible MindWave Mobile 2 y la comunicación depende de ThinkGear Connector, sujeto a las condiciones de NeuroSky.
- La comprobación del equipo no constituye validación universal ni auditoría externa.
- Permanecen pendientes revisión de seguridad, licencias y avisos de terceros.
- No se incluirán `mindApp.rar`, `Windows Setup Kit.zip`, `neuroExV6.6.zip`, scripts privados, CSV, `scores.csv`, `resultados_entrevista.csv`, resultados de los anexos, auditorías ni documentos académicos.

La Release permitirá descargar la aplicación desde GitHub sin añadir los 153 archivos individualmente al historial ordinario. Podrá prepararse inicialmente como borrador y solo se publicará después de aprobación humana. Estas notas no crean la etiqueta `v1.0.0`, no crean ni autorizan una GitHub Release y no publican el ZIP.
