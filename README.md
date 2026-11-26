# Puni Emu Offline 4.178.0

[Descargar APK y archivos para Android](https://github.com/mentahelada/puni-emu/releases/tag/v4.178.0)

## Instalar en Android ARM64

1. Descarga e instala **Termux.apk** y **PuniPuni-Offline.apk** desde los archivos de esta publicación. Abre Termux primero.
2. Con Internet y unos 12 GB de espacio libre, pega este bloque en Termux.

```sh
pkg update -y && pkg install -y curl &&
curl -fL --retry 3 https://github.com/mentahelada/puni-emu/releases/download/v4.178.0/instalar-puni.sh -o "$HOME/instalar-puni.sh" &&
bash "$HOME/instalar-puni.sh" &&
bash "$HOME/puniemu/arrancar.sh"
```

3. Espera a que el servidor arranque y abre el juego en el mismo móvil. Deja Termux abierto en segundo plano.

La próxima vez basta con ejecutar `bash ~/puniemu/arrancar.sh`. El instalador descarga los recursos y comprueba sus sumas SHA-256. El APK del juego apunta al servidor local del mismo móvil.
