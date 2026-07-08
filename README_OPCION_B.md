# OMEGLE - Opción B

Esta versión mantiene OME.TV dentro de la app WebView.

Cuando OME.TV intenta iniciar sesión con Google, la app abre solo el login en el navegador externo porque Google bloquea el login dentro de WebView con `403 disallowed_useragent`.

Después de volver a la app, se recarga OME.TV dentro de la APK.

Importante: no se puede garantizar que OME.TV copie la sesión del navegador hacia la WebView, porque Chrome/navegador y WebView no siempre comparten cookies. Esta es la solución más cercana a: app interna + Google externo solo para login.

## Compilar sin Android Studio

1. Sube todo el contenido del proyecto a GitHub.
2. Ve a Actions.
3. Ejecuta `Build APK`.
4. Descarga el artifact `OMEGLE-option-b-debug-apk`.
5. Descomprime el ZIP del artifact y usa el APK.
