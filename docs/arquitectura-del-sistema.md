# Arquitectura del sistema

Arquitectura de alto nivel confirmada por los archivos disponibles:

```text
MindWave Mobile 2 (NeuroSky, Inc.)
        |
ThinkGear Connector 3.2.4.0 (NeuroSky, tercero)
        |
mindApp compilada con Unity 2022.3.41f1 / exportación de CSV EEG
        |
Procesamiento técnico privado en Python
        |-- Anexo F: calibración
        `-- Anexo G: EEG y encuesta
        |
Evidencias y resultados agregados autorizados
```

## Componentes y versiones

- Dispositivo utilizado: MindWave Mobile 2.
- Fabricante del dispositivo: NeuroSky, Inc.
- Software de conexión: ThinkGear Connector.
- Versión del conector: **3.2.4.0**. ThinkGear Connector 3.2.4.0 es la versión identificada mediante los metadatos del ejecutable incluido en el paquete utilizado por el equipo; no se atribuye esta identificación a una verificación en la página oficial.
- Unity utilizado para desarrollar o compilar la aplicación: **2022.3.41f1**.
- Entorno principal de Python declarado por el equipo: **Python 3.12**.
- Python 3.12.13: utilizado únicamente para la comprobación posterior de sintaxis mediante `python -m py_compile`; los pipelines no fueron ejecutados nuevamente.
- Versiones exactas originales de NumPy, pandas, Matplotlib, SciPy, scikit-learn y openpyxl: no registradas.

La funcionalidad de mindApp fue comprobada por el equipo en Windows 11 Home Single Language, versión 25H2, compilación 26200.8875. La comprobación corresponde a Windows de 64 bits en el entorno del equipo, no constituye compatibilidad universal ni auditoría externa y Codex no ejecutó el binario. mindApp requiere MindWave Mobile 2 compatible y su comunicación depende de ThinkGear Connector, sujeto a las condiciones de NeuroSky.

El diagrama no implica propiedad ni derechos de redistribución sobre componentes de terceros.
