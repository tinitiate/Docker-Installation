# Docker-installation
# Windows
## Download Docker Desktop for Windows
[Docker Desktop for Windows](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe)

[Docker Desktop for Mac with Intel chip](https://desktop.docker.com/mac/main/amd64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-amd64)

[Docker Desktop for Mac with Apple chip](https://desktop.docker.com/mac/main/arm64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-arm64)
## Install interactively
1. Double-click Docker Desktop Installer.exe to run the installer.
![image](https://user-images.githubusercontent.com/51730523/174503709-5eb96362-797a-4c95-9d8e-99a39de3497d.png)

2. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.
3. When the installation is successful, click Close to complete the installation process.
4. If you get WSL2 installation is in complete error:

![image](https://user-images.githubusercontent.com/51730523/174503480-da66df95-6c0d-4832-87a9-dec2005f1c16.png)

![image](https://user-images.githubusercontent.com/51730523/174503525-b9bcae75-4ff6-4184-80a1-1b0267c56fc4.png)



![image](https://user-images.githubusercontent.com/51730523/174503528-cf5a5666-2ab5-4e58-9699-fd87f7db95a9.png)

  1. Open PowerShell as Administrator (Start menu > PowerShell > right-click > Run as Administrator) and enter this command:
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

```
![image](https://user-images.githubusercontent.com/51730523/174503534-6d450057-50b4-444f-9b9e-f73a0d9a19c3.png)

  2. Open PowerShell as Administrator and run:
```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

```

![image](https://user-images.githubusercontent.com/51730523/174503542-f50193ad-4646-474d-a672-caaefc5da557.png)

5. Download the Linux kernel update package
[Linux kernel update](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)
