# Versión 2 - Google Login

Esta versión mantiene OME.TV en WebView, pero cuando detecta una URL de inicio de sesión de Google la abre en el navegador seguro del teléfono.

Motivo: Google bloquea el login dentro de WebView con el error 403 `disallowed_useragent`. No es un error de tu APK; es una restricción de Google.

## Qué subir a GitHub

Sube el contenido completo de esta carpeta al mismo repositorio, reemplazando los archivos existentes.

Si prefieres subir solo el cambio principal, reemplaza este archivo:

`app/src/main/java/com/lascuentasia/omegleweb/MainActivity.java`

Luego ejecuta otra vez **Actions > Build APK > Run workflow**.

## Importante

El login de Google puede abrirse en Chrome/navegador externo. Si OME.TV no comparte la sesión de vuelta con WebView, la solución más estable es usar la web en navegador seguro o una app oficial, porque no controlamos los servidores ni la autenticación de OME.TV.
