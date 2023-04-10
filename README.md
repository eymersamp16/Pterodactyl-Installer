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

| Sistema operativo| Versión               | Soportado                          |
| ---------------- | ----------------------| ---------------------------------- |
| Ubuntu           | from 18.04 to 22.04   | :white_check_mark:                 |
| Debian           | from 10 to 11         | :white_check_mark:                 |
| CentOS           | no supported versions | :x:                                |
| Rocky Linux      | no supported versions | :x:                                |

| Servidor web	   | Soportado           |
| ---------------- | --------------------| 
| NGINX            | :white_check_mark:  |
| Apache           | :white_check_mark:  |
| LiteSpeed        | :x:                 |
| Caddy            | :x:                 |

# Derechos de autor
Por favor, no digas que creaste este script. Puede crear una bifurcación para este Pterodactyl-Installer, pero agradecería que se vinculara este github. Además, no elimine mis derechos de autor en la parte superior del script Pterodactyl-Installer.

# Apoyo
No se ofrece soporte para este script. El script se probó muchas veces sin corregir errores, sin embargo, aún pueden ocurrir. Si encuentra errores, no dude en abrir un "Problema" en GitHub.

# Instalación Interactiva/Normal
La forma recomendada de usar este script. Solo sistemas basados en Debian.
```bash
bash <(curl -s https://raw.githubusercontent.com/guldkage/Pterodactyl-Installer/main/installer.sh)
```

### Raspbian
Solo para usuarios de raspbian. Es posible que necesiten un < extra al principio.
```bash
bash < <(curl -s https://raw.githubusercontent.com/guldkage/Pterodactyl-Installer/main/installer.sh)
```

# Instalación automática / Instalación del desarrollador
¡Úsalo solo si sabes lo que estás haciendo! Ahora puede instalar Pterodactyl usando 1 comando sin tener que escribir nada manualmente después de ejecutar el comando.


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

Debe ser preciso al usar este script. 1 error tipográfico y todo puede salir mal. También debe ejecutarse en una versión nueva de Ubuntu o Debian.


```bash
bash <(curl -s https://raw.githubusercontent.com/guldkage/Pterodactyl-Installer/main/autoinstall.sh)  <fqdn> <ssl> <email> <username> <firstname <lastname> <password> <wings>
```
