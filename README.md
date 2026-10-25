# switch-parser

Pipeline de GitHub Actions para compilar juegos de Nintendo Switch (`.nsp`) a paquetes nativos de iOS (`.ipa`) utilizando [nxnative](https://github.com/seedds/nxnative) sobre runners de macOS.

## Configuración requerida

1. En el repositorio de GitHub, ir a **Settings > Secrets and variables > Actions**.
2. Agregar un secret llamado `PROD_KEYS` con el contenido de tu archivo `prod.keys`.
3. Subir el archivo `.nsp` a un servicio con enlace de descarga directa (por ejemplo, Google Drive, OneDrive, S3 o similar).

## Uso

1. Ir a la pestaña **Actions** en GitHub.
2. Seleccionar el workflow **Build IPA with nxnative**.
3. Hacer clic en **Run workflow**, ingresar la URL de descarga del `.nsp` y ejecutar.
4. Al finalizar, descargar el archivo `.ipa` generado en la sección de artifacts para instalarlo con Sideloadly.
