# OMEGLE - APK WebView para https://ome.tv/

Este ZIP contiene un proyecto Android listo para abrir en Android Studio. La app carga `https://ome.tv/` dentro de un WebView y ya incluye permisos de internet, cámara y micrófono.

## Cómo generar el APK

1. Instala Android Studio.
2. Abre esta carpeta como proyecto.
3. Espera a que sincronice Gradle.
4. Ve a **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Android Studio generará el APK en:

`app/build/outputs/apk/debug/app-debug.apk`

## Notas importantes

- La app depende de internet.
- OME.TV puede bloquear WebView o exigir Chrome/Play Services según sus políticas internas. Si eso ocurre, la alternativa más estable es usar una PWA/TWA si el sitio lo permite.
- Para publicar en Play Store necesitarás cambiar identificadores, revisar derechos de marca/nombre y firmar la app en modo release.

## Sin Android Studio

También puedes generar el APK desde GitHub, sin instalar Android Studio. Mira el archivo:

`README_SIN_ANDROID_STUDIO.md`

El proyecto incluye `.github/workflows/build-apk.yml`, que compila automáticamente el APK y lo deja como artifact descargable.
