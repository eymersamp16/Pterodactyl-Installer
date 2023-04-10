# Pterodactyl Installer

Con este script puede instalar, actualizar o eliminar fácilmente Pterodactyl Panel. Todo está reunido en un guión. Utilice este script si desea instalar, actualizar o eliminar sus servicios rápidamente. Las cosas que se están haciendo ya están listadas en Pterodactyl , pero esto claramente lo hace más rápido ya que es automático.

Tenga en cuenta que este script está diseñado para funcionar en una instalación nueva. Existe una buena posibilidad de que falle si no es una instalación nueva. El script debe ejecutarse como root.

Si encuentra algún error, cosas que le gustaría cambiar o consultas sobre cosas en el futuro para este script, escriba un "Problema". Lea sobre el pterodáctilo aquí. Este script no está asociado con el Proyecto Pterodactyl oficial.

# Características
Este script es uno de los únicos que tiene una función de cambio de dominios que funciona bien.

- Panel de instalación
- instalar alas
- Instalar PHPMyAdmin
- Cambiar dominios de pterodáctilo
- Panel de desinstalación
- Desinstalar alas

# Sistema operativo y servidor web compatibles
Sistemas operativos compatibles.

| Operating System | Version               | Supported                          |
| ---------------- | ----------------------| ---------------------------------- |
| Ubuntu           | from 18.04 to 22.04   | :white_check_mark:                 |
| Debian           | from 10 to 11         | :white_check_mark:                 |
| CentOS           | no supported versions | :x:                                |
| Rocky Linux      | no supported versions | :x:                                |

| Webserver        | Supported           |
| ---------------- | --------------------| 
| NGINX            | :white_check_mark:  |
| Apache           | :white_check_mark:  |
| LiteSpeed        | :x:                 |
| Caddy            | :x:                 |

# Copyright
Please do not say you created this script. You may create a fork for this Pterodactyl-Installer, but I would appreciate this github being linked to.
Also, please not remove my copyright at the top of the Pterodactyl-Installer script.

# Support
No support is offered for this script.
The script has been tested many times without any bug fixes, however they can still occur.
If you find errors, feel free to open an "Issue" on GitHub.

# Interactive/Normal installation
The recommended way to use this script.
Debian based systems only.
```bash
bash <(curl -s https://raw.githubusercontent.com/guldkage/Pterodactyl-Installer/main/installer.sh)
```

### Raspbian
Only for raspbian users. They might need a extra < in the beginning.
```bash
bash < <(curl -s https://raw.githubusercontent.com/guldkage/Pterodactyl-Installer/main/installer.sh)
```

# Autoinstall / Developer Installation
Only use this if you know what you are doing!
You can now install Pterodactyl using 1 command without having to manually type anything after running the command.

```
<fqdn> = What you want to access your panel with. Eg. panel.domain.ltd
<ssl> = Whether to use SSL. Options are true or false.
<email> = Your email. If you choose SSL, it will be shared with Lets Encrypt.
<username> = Username for admin account on Pterodactyl
<firstname> = First name for admin account on Pterodactyl
<lastname> = Lastname for admin account on Pterodactyl
<password> = The password for the admin account on Pterodactyl
<wings> = Whether you want to have Wings installed automatically as well. Options are true or false.
```

You must be precise when using this script. 1 typo and everything can go wrong.
It also needs to be run on a fresh version of Ubuntu or Debian.

```bash
bash <(curl -s https://raw.githubusercontent.com/guldkage/Pterodactyl-Installer/main/autoinstall.sh)  <fqdn> <ssl> <email> <username> <firstname <lastname> <password> <wings>
```
