# Marcador Skull King (Android)

App Android mínima: una WebView que carga el marcador desde `app/src/main/assets/index.html`. Funciona sin conexión; la partida se guarda en el propio móvil.

## Conseguir el APK

1. Crea un repo nuevo en GitHub (puede ser privado).
2. Sube el contenido de esta carpeta:
   ```bash
   git init
   git add .
   git commit -m "Marcador Skull King"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/skullking-marcador.git
   git push -u origin main
   ```
3. En el repo, pestaña **Actions**: el workflow "Compilar APK" arranca solo con el push (tarda unos 3-5 min).
4. Entra en la ejecución terminada y descarga el artefacto **skull-king-apk** (un .zip con el APK dentro).
5. Pasa el APK al móvil, ábrelo y permite instalar apps de fuentes desconocidas cuando te lo pida.

## Cambiar el marcador

Edita `app/src/main/assets/index.html`, sube los cambios y Actions vuelve a compilar. Para que se instale encima de la versión anterior, sube `versionCode` en `app/build.gradle`.
