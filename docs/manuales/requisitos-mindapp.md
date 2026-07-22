# Requisitos de mindApp

## Hardware y conectividad

- Computador con Windows de 64 bits.
- Dispositivo MindWave Mobile 2 compatible.
- Conectividad y emparejamiento requeridos por el dispositivo.

## Software externo

- MindWave Mobile 2 y sus controladores aplicables.
- ThinkGear Connector 3.2.4.0 instalado y en ejecución.
- Herramienta confiable para extraer archivos ZIP.

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde a la plataforma Windows de 64 bits utilizada por el equipo; no constituye compatibilidad universal con todas las versiones de Windows ni una auditoría externa. Codex no ejecutó el binario. La aplicación fue desarrollada o compilada con Unity 2022.3.41f1.

La dependencia quedó documentada así: ThinkGear Connector 3.2.4.0, versión identificada mediante los metadatos del ejecutable incluido en el paquete utilizado por el equipo. La aplicación requiere hardware compatible MindWave Mobile 2 y su comunicación con el dispositivo depende de ThinkGear Connector, sujeto a las condiciones de NeuroSky. El ejecutable de ThinkGear Connector no fue ejecutado durante la inspección documental.

El repositorio público no redistribuye `Windows Setup Kit.zip`; el paquete utilizado por el equipo se conserva únicamente como respaldo interno no publicable. Las instrucciones permanecen disponibles, pero el usuario debe obtener ThinkGear Connector prioritariamente desde la fuente oficial de NeuroSky. El paquete no se incluirá en la Release de `mindApp`.

## Evidencia de la compilación

`ENTRADA_CODEX/mindApp.rar` es la fuente original interna. `RELEASE_CANDIDATES/mindApp-v1.0.0-windows.zip` contiene la misma compilación, extraída y reempaquetada para distribución sin reconstrucción, recompilación o modificación interna por Codex. El RAR permanecerá en almacenamiento interno y el ZIP será el archivo principal propuesto para la futura Release; no es necesario publicar ambos.

El candidato contiene 153 archivos, aproximadamente `MindwaveUnity.exe`, `MindwaveUnity_Data/`, bibliotecas generadas por Unity, recursos, configuración y los demás componentes necesarios de la compilación original. No contiene código fuente de Unity. La comparación archivo por archivo produjo 0 faltantes, 0 adicionales y 0 diferencias de hash. No se ejecutaron ni descompilaron binarios.

Antes de distribuir deben revisarse dependencias y avisos de terceros, metadatos, rutas internas, seguridad, privacidad y versión de Windows admitida.

La futura Release de mindApp 1.0.0 se asociará posteriormente a `v1.0.0`, ofrecerá el ZIP sin añadir los 153 archivos individualmente al historial e incluirá notas, instalación, requisitos, SHA-256, reconocimientos y avisos de terceros. Podrá crearse como borrador y publicarse solo tras aprobación humana. No incluirá `mindApp.rar`, `Windows Setup Kit.zip`, `neuroExV6.6.zip`, scripts privados, CSV, `scores.csv`, `resultados_entrevista.csv`, resultados de los anexos, auditorías ni documentos académicos.
