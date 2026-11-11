# GeoUrbano sin permisos de administrador (Windows)

## Opción recomendada: Google Colab

No ejecutes `run_windows.bat` en esta computadora. Ese archivo instala dependencias locales y puede requerir permisos que no tienes.

1. Abre https://colab.research.google.com/ desde Chrome o Edge.
2. Inicia sesión con tu cuenta Google.
3. Selecciona **Archivo > Subir cuaderno**.
4. Dentro de esta carpeta, sube `notebooks/mancha_urbana_sentinel2_v08_GEE_integrado.ipynb`.
5. En Colab, selecciona **Entorno de ejecución > Cambiar tipo de entorno de ejecución** y deja Python 3.
6. Ejecuta las celdas en orden.
7. En la celda **GEE: autenticación...**, reemplaza `REEMPLAZA_CON_TU_GOOGLE_CLOUD_PROJECT_ID` por el ID de un proyecto de Google Cloud que tenga Earth Engine habilitado.
8. Cuando Colab lo solicite, autoriza Earth Engine con la cuenta Google correspondiente.
9. Las tareas exportadas a Drive aparecerán en la pestaña Tasks de Earth Engine y en la carpeta `GeoUrbano_Exportaciones` de Google Drive.

## Importante

- No necesitas instalar Python, Git, Node ni paquetes en Windows.
- Los comandos `!pip install` se ejecutan en la máquina virtual temporal de Google Colab, no en tu PC.
- No introduzcas tu contraseña en el notebook, en GitHub ni en archivos `.env`.
- Google Earth Engine requiere un Google Cloud Project ID habilitado y permisos de acceso a Earth Engine.
- El notebook contiene dos flujos: el análisis original basado en STAC/Overture y el bloque complementario de compuestos/exportación GEE. El bloque GEE no reemplaza automáticamente el entrenamiento Random Forest del flujo original.
- Las sesiones gratuitas de Colab son temporales; guarda el notebook en Drive y descarga los resultados importantes.
