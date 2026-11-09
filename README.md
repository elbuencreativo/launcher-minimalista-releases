# Launcher minimalista — versiones

APK del **Launcher minimalista** para Android. Este repositorio solo contiene las versiones publicadas (pestaña **Releases**);
el launcher las consulta desde *Ajustes → Sistema → Actualizaciones* para actualizarse solo.

## Instalar
1. Abre la última versión: [Releases → latest](../../releases/latest)
2. Descarga `launcher-<versión>.apk` y ábrelo. Android pedirá permitir instalar apps desconocidas.
3. Elige el launcher como pantalla de inicio cuando Android lo pregunte.

Requiere Android 10 o superior.

## Verificar la descarga
Cada versión incluye `SHA256SUMS.txt`:

```bash
shasum -a 256 -c SHA256SUMS.txt
```

Todos los APK están firmados con la misma clave. Huella SHA-256 del certificado de firma:

```
18338108fb86b71de6b1b6eac639d7e6cf3446d20d5d49ec3d32a2723f65e505
```

Si un APK muestra otra huella, no es de este proyecto (`apksigner verify --print-certs launcher-<versión>.apk`).

## Fuentes incluidas
La app incluye fuentes de Google Fonts (Inter, DM Sans, Work Sans, Source Sans 3, Nunito Sans, Lora, Playfair Display,
Libre Baskerville, Bitter, Crimson Text) bajo la licencia SIL Open Font License 1.1; el texto de cada licencia viaja dentro del APK.
