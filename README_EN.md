# Version to install on WSL

You can find installation and configuration instructions here: [Wiki](https://github.com/Thinstation/thinstation-ng/wiki/Getting-Started-with-ThinStation).

WSL can be downloaded from here: [https://github.com/microsoft/WSL/releases/download/2.5.9/wsl.2.5.9.0.x64.msi](https://github.com/microsoft/WSL/releases/download/2.5.9/wsl.2.5.9.0.x64.msi)

To build ThinStation 7.2-Stable-wsl, you will need Fedora Linux 42:

```PowerShell
wsl --install FedoraLinux-42
```

Getting ThinStation 7.2-Stable-wsl:

```Bash
git clone https://github.com/Mikhail782/thinstation-wsl.git
```

Installing the chroot:

```Bash
cd thinstation-wsl && sudo ./setup-wsl
```

Building a boot image:

```Bash
cd build && ./build --autodl
```
