# Instalación propuesta de mindApp

No existe todavía una GitHub Release. Este procedimiento se documenta para `RELEASE_CANDIDATES/mindApp-v1.0.0-windows.zip`, candidato de mindApp 1.0.0 y futuro archivo principal de una Release asociada posteriormente a la etiqueta `v1.0.0`.

`ENTRADA_CODEX/mindApp.rar` es la fuente original interna. El ZIP no es una aplicación diferente: contiene la misma compilación del RAR, extraída y reempaquetada para facilitar su descarga y extracción en Windows. Codex no reconstruyó ni recompiló la aplicación y su contenido interno no fue modificado. El RAR permanecerá en almacenamiento interno y no necesita publicarse junto con el ZIP.

## Antes de instalar

1. Obtenga el archivo únicamente de una fuente autorizada por los autores.
2. Verifique el SHA-256 publicado para la descarga correspondiente.
3. Analice el ZIP con los controles de seguridad de su institución.
4. Instale y configure legalmente MindWave Mobile 2 y ThinkGear Connector desde las fuentes oficiales de NeuroSky.
5. Confirme que el equipo Windows cumple los requisitos documentados.

## Instalación

1. Extraiga todo el ZIP en una carpeta nueva; no ejecute el programa desde dentro del archivo comprimido.
2. Mantenga juntos `MindwaveUnity.exe`, `MindwaveUnity_Data/`, `MonoBleedingEdge/`, `UnityPlayer.dll` y `UnityCrashHandler64.exe`.
3. Conecte y empareje MindWave Mobile 2 conforme a la documentación oficial.
4. Inicie ThinkGear Connector.
5. Ejecute `MindwaveUnity.exe` solo después de la revisión de seguridad y con autorización.
6. Guarde cualquier exportación en una ubicación privada y autorizada.

## Limitaciones

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde al entorno Windows de 64 bits utilizado por el equipo; no constituye compatibilidad universal con todas las versiones de Windows ni una auditoría externa. Codex no ejecutó el binario. La aplicación fue desarrollada o compilada con Unity 2022.3.41f1.

La aplicación requiere hardware compatible MindWave Mobile 2 y la comunicación con el dispositivo depende de ThinkGear Connector, sujeto a los términos y condiciones de NeuroSky.

`Windows Setup Kit.zip` no forma parte del candidato ni debe incorporarse a la Release. Se recomienda obtener las dependencias de NeuroSky desde su fuente oficial.

La futura Release permitirá descargar el ZIP sin añadir los 153 archivos individualmente al historial ordinario y deberá incluir notas de versión, estas instrucciones, requisitos, SHA-256, reconocimientos y avisos de terceros. Podrá prepararse como borrador y solo publicarse después de aprobación humana. No incluirá `mindApp.rar`, `Windows Setup Kit.zip`, `neuroExV6.6.zip`, scripts privados, CSV, `scores.csv`, `resultados_entrevista.csv`, resultados, auditorías ni documentos académicos.
