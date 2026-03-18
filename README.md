# 🤠 Billy Walters PRO — APK Builder

Este repositorio compila automáticamente el APK de **Billy Walters PRO** usando GitHub Actions.

## ✅ Cómo obtener tu APK

### Opción A — Descarga desde Releases (más fácil)
1. Ve a la pestaña **Releases** del repo
2. Descarga `app-debug.apk`
3. Instala en tu Android

### Opción B — Desde Actions
1. Ve a **Actions → Build Billy Walters APK**
2. Descarga el artifact `BillyWaltersPRO-debug`

---

## 📂 Estructura del proyecto
```
├── .github/
│   └── workflows/
│       └── build-apk.yml       ← Compilación automática
├── android/
│   ├── app/
│   │   ├── src/main/
│   │   │   ├── assets/public/
│   │   │   │   └── index.html  ← La app HTML completa
│   │   │   ├── java/com/billywalters/pro/
│   │   │   │   └── MainActivity.java
│   │   │   ├── res/            ← Iconos y recursos
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   ├── build.gradle
│   ├── settings.gradle
│   └── gradlew
└── README.md
```

---

## 🔄 Actualizar la app
Para actualizar el contenido, reemplaza `android/app/src/main/assets/public/index.html` y haz push — el APK se recompila solo.
