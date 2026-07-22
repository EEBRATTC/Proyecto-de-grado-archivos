# Plan para una futura GitHub Release de mindApp

Este documento es un plan; no autoriza ni crea una Release.

## Candidato local

- Ruta fuera del repositorio: `RELEASE_CANDIDATES/mindApp-v1.0.0-windows.zip`.
- Tamaño actual: 32,515,872 bytes.
- SHA-256: `EF1F902F0DA06056A4305D3D196F1E627886936B3874F2E1ED23E1FD6C986FB3`.
- Contenido verificado: 153 archivos, 0 faltantes, 0 extras y 0 diferencias frente a la extracción del RAR original.

`ENTRADA_CODEX/mindApp.rar`, SHA-256 `02AE879941EA3DB2E466D16FDCF4BF0859344CEDA6547FBADCBA3B0607A3B8C2`, es la fuente original interna. El ZIP candidato no es una aplicación diferente, no fue reconstruido ni recompilado por Codex y contiene la misma compilación del RAR, extraída y reempaquetada en formato ZIP para facilitar su descarga y extracción en Windows. La aplicación interna no fue modificada. El RAR permanecerá en almacenamiento interno y el ZIP será el paquete propuesto para distribución; no es necesario publicar ambos.

El ZIP contiene aproximadamente `MindwaveUnity.exe`, `MindwaveUnity_Data/`, bibliotecas generadas por Unity, recursos, archivos de configuración y los demás componentes necesarios incluidos en la compilación original. No contiene el código fuente de Unity.

## Entorno funcional confirmado

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde al entorno Windows de 64 bits utilizado por el equipo, no constituye compatibilidad universal con todas las versiones de Windows ni una auditoría externa, y Codex no ejecutó el binario. La aplicación fue desarrollada o compilada con Unity 2022.3.41f1. Requiere hardware compatible MindWave Mobile 2; la comunicación depende de ThinkGear Connector y su uso permanece sujeto a las condiciones de NeuroSky.

## Estructura prevista de la futura Release

- Versión de la aplicación: **mindApp 1.0.0**.
- Etiqueta prevista para una etapa posterior: `v1.0.0`; no ha sido creada.
- Archivo principal: `mindApp-v1.0.0-windows.zip`.
- La descarga se ofrecerá mediante GitHub Release sin añadir los 153 archivos individualmente al historial ordinario del repositorio.
- La Release incluirá notas de versión, instrucciones de instalación, requisitos, SHA-256, reconocimientos y avisos de terceros.
- Podrá crearse inicialmente como borrador y solo publicarse después de aprobación humana.
- `RELEASE_CANDIDATES/mindApp-v1.0.0-windows.zip` permanecerá fuera de los repositorios hasta esa decisión.

## Controles pendientes antes de publicar

1. Realizar la revisión final de seguridad institucional sin incorporar datos reales.
2. Revisar licencias y avisos de Unity, Mono y demás bibliotecas incluidas.
3. Confirmar instrucciones oficiales para MindWave Mobile 2 y ThinkGear Connector.
4. Revisar el ZIP final y repetir inventario, detección de secretos y hashes si el archivo llegara a cambiar.
5. Obtener aprobación humana expresa de los autores y de las instancias institucionales aplicables.
6. Crear la etiqueta y la Release únicamente después de la aprobación, preferiblemente primero como borrador, y publicar el checksum del archivo definitivo.

## Exclusiones obligatorias

La futura Release no incluirá `mindApp.rar`, `Windows Setup Kit.zip`, `neuroExV6.6.zip`, scripts privados, CSV, `scores.csv`, `resultados_entrevista.csv`, resultados de los anexos, auditorías, documentos académicos, consentimientos, credenciales ni software de terceros adicional. `Windows Setup Kit.zip` fue retirado del árbol público y se conserva únicamente como respaldo interno no publicable; el repositorio público no lo redistribuye. ThinkGear Connector debe obtenerse prioritariamente desde la fuente oficial y utilizarse conforme a las condiciones de NeuroSky. No declarar el paquete como código abierto ni afirmar derechos sobre componentes externos.
