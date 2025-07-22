# Версия для установки на WSL

Описание установки и настройки есть тут: [Wiki](https://github.com/Thinstation/thinstation-ng/wiki/Getting-Started-with-ThinStation).

WSL можно взять отсюда: [https://github.com/microsoft/WSL/releases/download/2.5.9/wsl.2.5.9.0.x64.msi](https://github.com/microsoft/WSL/releases/download/2.5.9/wsl.2.5.9.0.x64.msi)

Для сборки ThinStation 7.2-Stable-wsl, потребуется Fedora Linux 42:

```PowerShell
wsl --install FedoraLinux-42
```

Получение ThinStation 7.2-Stable-wsl:

```Bash
git clone https://github.com/Mikhail782/thinstation-wsl.git
```

Установка chroot:

```Bash
cd thinstation-wsl && sudo ./setup-chroot
```

Сборка загрузочного образа:

```Bash
cd build && ./build --autodl
```

Конфигурирование сборки ThinStation происходит с помощью двух файлов в папке build: `build.conf`, `thinstation.conf.buildtime`.
