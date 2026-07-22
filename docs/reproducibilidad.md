# Reproducibilidad

Los elementos se conservan en repositorios separados: código en GitHub privado; datos, scores, encuesta, resultados completos y auditorías en GitLab privado; documentación y resultados agregados seleccionados en este GitHub público.

El entorno principal declarado por el equipo es Python 3.12. Las dependencias detectadas son NumPy, pandas, Matplotlib, SciPy, scikit-learn y openpyxl, pero sus versiones exactas originales no fueron registradas. `tkinter` se usa opcionalmente y normalmente forma parte de Python. Python 3.12.13 corresponde únicamente a la comprobación posterior de sintaxis de los dos scripts mediante `python -m py_compile`; esa comprobación no ejecutó nuevamente los pipelines.

El código privado puede solicitarse mediante `eebratt12@gmail.com` o concederse por invitación directa a una persona específica. Cada solicitud será evaluada por los autores y no garantiza acceso; cualquier autorización queda sujeta a las condiciones académicas, institucionales, de privacidad y reutilización aplicables. La URL privada no se publica.

La reorganización no ejecutó pipelines, no modificó CSV y no recalculó resultados. Una reproducción futura requiere acceso autorizado, verificación de hashes, configuración metodológica aprobada, registro del entorno y una carpeta de salida nueva. La validación con `py_compile` no equivale a reproducibilidad numérica.
