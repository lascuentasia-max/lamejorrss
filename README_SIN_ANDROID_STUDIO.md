# Generar el APK sin Android Studio

Este proyecto incluye una compilación automática con GitHub Actions. Puedes hacerlo desde el móvil o desde un navegador.

## Pasos

1. Entra en https://github.com y crea una cuenta o inicia sesión.
2. Pulsa **New repository**.
3. Pon un nombre, por ejemplo: `omegle-apk`.
4. Sube todos los archivos de este ZIP al repositorio.
   - Importante: sube el contenido de la carpeta, no el ZIP cerrado.
5. Ve a la pestaña **Actions**.
6. Abre **Build APK**.
7. Pulsa **Run workflow**.
8. Espera a que termine la compilación.
9. En la ejecución finalizada, baja a **Artifacts** y descarga `OMEGLE-debug-apk`.
10. Dentro estará `app-debug.apk`.

## Instalar en Android

1. Copia `app-debug.apk` al móvil.
2. Ábrelo.
3. Android puede pedir activar **Instalar apps desconocidas** para tu navegador o gestor de archivos.
4. Acepta e instala.

## Notas

- Este APK es de prueba/debug. Funciona para instalar manualmente, pero no es ideal para publicar en Google Play.
- La app carga `https://ome.tv/` dentro de un WebView.
- Si OME.TV bloquea WebView, cámara/micrófono o login por sus propias políticas, no se puede garantizar desde la APK.
- Revisa derechos de marca y términos de OME.TV si vas a distribuir esta app a otras personas.
