# Own-Cloud
En este tutorial, enseñaré paso a paso, como configurar Owncloud a través del terminal de Linux
# Instal·lació d'apache2, mysql i algunes llibreries al contenidor
1. Actualización de la máquina.
   
Para actualizar la máquina tendremos que poner el código **sudo apt update**, después de eso le daremos a enter

![Text alternatiu](1.png)

Cuando nos pregunte la contraseña pondremos usuario, todo en minusculas y le daremos a enter

![Text alternatiu](2.png)

Después de esto le pondremos otro comando, el cual és: **sudo apt upgrade** y le daremos a enter.

![Text alternatiu](3.png)

Cuando nos pregunte si deseamos continuar le daremos a enter para aceptar.

![Text alternatiu](4.png)
2. Instalación del servidor web `apache2`.

Para esto en el terminal tendremos que poner:**sudo apt install -y apache2**

![Text alternatiu](5.png)
3. Instalación del servidor de bases de datos `mysql-server`.

Tendremos que poner: **sudo apt install -y mysql-server**

![Text alternatiu](6.png)
4. Instalación de algunas librerías de `php`, el lenguaje principal que utilizan las aplicaciones.

Esto lo haremos con el siguiente comando:**sudo apt install -y php libapache2-mod-php**

![Text alternatiu](7.png)

Seguido de esto,pondremos el comando:**sudo apt install -y php-fpm php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-ldap php-zip php-curl**

![Text alternatiu](8.png)
5. Reiniciamos el servidor apache2

Finamlmente reiniciamos el servidor con el siguiente comando:**sudo systemctl restart apache2**

![Text alternatiu](9.png)

# Configuració de MySQL


