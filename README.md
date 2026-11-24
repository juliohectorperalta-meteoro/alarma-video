# Cámara ESP32 – App Android

App para ver en vivo la ESP32-CAM (firmware `esp32cam_online.ino`).

## Compilar el APK con GitHub Actions
1. Creá un repositorio nuevo en GitHub (por ejemplo `camara-esp32`).
2. Subí todo el contenido de esta carpeta, **incluida la carpeta oculta `.github`**.
3. Entrá a la pestaña **Actions** → "Compilar APK". Se ejecuta solo con cada subida
   (o tocá "Run workflow").
4. Cuando termine (unos 5 min), abrí la ejecución y descargá **camara-esp32-apk**.
5. Descomprimí el zip e instalá `app-debug.apk` en el teléfono.

## Primer uso
- Al abrir la app aparece la configuración:
  - Dirección: la IP de la cámara (ej. `192.168.100.36`)
  - Puerto web: `80` · Puerto video: `81`
  - Clave: la `SECRET_STREAM_KEY` del `secrets.h`
- "Probar conexión" y después "Guardar y conectar".

## Uso
- Tocá el video para pantalla completa (girá el teléfono para verlo apaisado).
- Botón atrás de Android: sale de pantalla completa / cierra paneles.
- Al minimizar la app el video se corta solo (ahorra datos y la cámara descansa).
