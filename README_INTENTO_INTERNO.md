# OMEGLE v5 - intento de Google interno

Esta versión intenta mantener OME.TV y el login dentro de la WebView usando:

- Cookies y cookies de terceros activadas.
- DOM Storage activado.
- Cámara y micrófono.
- User-Agent parecido a Chrome móvil.
- Popups/ventanas cargadas dentro de la misma WebView.

Importante: Google puede bloquear igualmente el login con `403 disallowed_useragent`. Si eso pasa, no se puede resolver de forma estable dentro de WebView. La opción estable es Chrome/TWA.
