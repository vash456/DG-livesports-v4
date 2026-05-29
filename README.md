# DG LiveSports

Aplicación Android nativa de deportes en vivo que proporciona acceso a noticias, resultados, tablas, videos, social y notificaciones. El proyecto incluye autenticación de usuarios con Firebase y Facebook, mapas con Google Maps y una interfaz basada en navegación lateral + pestañas.

## Descripción

DG LiveSports es una aplicación de deportes que centraliza información deportiva en un solo lugar. El proyecto está escrito en Java y usa Android SDK 24, además de integrar servicios de Firebase, Facebook y Google Play Services.

## Funcionalidades principales

- Pantalla de bienvenida con splash.
- Autenticación mediante login y registro.
- Navegación lateral con secciones:
  - Principal
  - Resultados
  - Partidos y tablas
  - Noticias
  - Videos
  - Social
  - Notificaciones
  - Configuración
- Visualización de tablas de equipos y detalles de equipos.
- Mapa integrado con Google Maps.
- Detección de conexión de red.
- Gestión de sesión y cierre de sesión.

## Estructura del proyecto

- `app/build.gradle`: configuración del módulo Android.
- `build.gradle`: configuración de Gradle a nivel de proyecto.
- `settings.gradle`: incluye el módulo `:app`.
- `app/src/main/AndroidManifest.xml`: manifiesto de aplicación, permisos y actividades.
- `app/src/main/java/com/dg_livesports/dg_livesports/`: código fuente Java.
- `app/src/main/res/`: recursos de layouts, valores, drawables y menús.

## Requisitos

- Android Studio (o un IDE compatible con Gradle).
- JDK 8 o compatible.
- SDK de Android 24.
- Conexión a Internet para descargar dependencias y usar servicios en tiempo de ejecución.

## Dependencias importantes

- Android Support Libraries: `appcompat-v7`, `support-v4`, `design`.
- Firebase: `firebase-core`, `firebase-auth`.
- Facebook Android SDK.
- Google Play Services: `play-services-maps`, `play-services-location`, `play-services-auth`, `play-services`.
- Firebase antiguo: `com.firebase:firebase-client-android:2.5.2+`.
- Apache Commons IO.

## Configuración adicional

El repositorio incluye `google-services.json` en `app/` y referencias a claves de API en `res/values/google_maps_api.xml`, `src/debug/res/values/google_maps_api.xml` y `src/release/res/values/`. Asegúrate de:

- Tener un `google_maps_key` válido para Google Maps.
- Ajustar el `facebook_app_id` y la configuración de Facebook si usas login de Facebook.

## Ejecutar el proyecto

1. Abre el proyecto en Android Studio.
2. Sincroniza Gradle.
3. Ejecuta el módulo `app` en un emulador o dispositivo físico.

## Compilar desde línea de comandos

Desde la raíz del proyecto:

```bash
./gradlew clean assembleDebug
```

En Windows PowerShell:

```powershell
.
abla
gradlew.bat clean assembleDebug
```

## Notas

- Este proyecto usa versiones antiguas de dependencias de Android y Google Play Services, por lo que puede necesitar actualización para compilar con versiones modernas del SDK.
- El manifiesto solicita permisos de Internet y ubicación para funcionalidades de mapas.

---

**Package:** `com.dg_livesports.dg_livesports`
**Min SDK:** 16
**Target SDK:** 24
**Version:** 1.0
