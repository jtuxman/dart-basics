# Hola Mundo Android (Flutter)

App Flutter mínima que muestra "¡Hola, Mundo!" y un contador de toques.

## Requisitos

- [Flutter SDK](https://docs.flutter.dev/get-started/install) 3.10 o superior
- Android Studio o la línea de comandos del Android SDK (API 21+)
- Un emulador Android o un dispositivo físico con depuración USB activada

## Primera vez: generar el resto del scaffolding

Este proyecto contiene solo las piezas específicas de la app (`lib/main.dart`, `pubspec.yaml`, `AndroidManifest.xml`, `MainActivity.kt`). Para completar los archivos Gradle, Kotlin y recursos que Flutter genera automáticamente:

```bash
cd hola_mundo_android
flutter create --org com.example --project-name hola_mundo_android .
flutter pub get
```

`flutter create .` sobre un directorio existente respeta los archivos que ya están y rellena los que faltan (Gradle, `ic_launcher`, temas, etc.).

## Ejecutar

Con un emulador o dispositivo conectado:

```bash
flutter devices        # verifica que aparezca tu Android
flutter run            # compila y ejecuta en modo debug
```

## Generar APK

```bash
flutter build apk --release
```

El APK queda en `build/app/outputs/flutter-apk/app-release.apk`.
