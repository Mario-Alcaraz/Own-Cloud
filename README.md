# Own-Cloud
En este tutorial, enseñaré paso a paso, como configurar Owncloud a través del terminal de Linux
# Instal·lació d'apache2, mysql i algunes llibreries al contenidor
Para este paso tendremos que hacer varios pasos pero el primero es actualizar la máquina.

Para actualizar la máquina tendremos que poner el código **sudo apt update**, después de eso le daremos a enter

![Text alternatiu](1.png)

Cuando nos pregunte la contraseña pondremos usuario, todo en minusculas y le daremos a enter

![Text alternatiu](2.png)

Después de esto le pondremos otro comando, el cual és: **sudo apt upgrade** y le daremos a enter.

![Text alternatiu](3.png)

Cuando nos pregunte si deseamos continuar le daremos a enter para aceptar.

![Text alternatiu](4.png)

Después tendremos que hacer el siguiente paso que es instalar el servidor web apache 2, para esto en el terminal tendremos que poner:**sudo apt install -y apache2**

![Text alternatiu](5.png)

El siguiente paso será instalar el servidor mysql-server, tendremos que poner: **sudo apt install -y mysql-server**

![Text alternatiu](6.png)

Después de esto tendremos que instalar algunas librerias de php, con el siguiente comando:**sudo apt install -y php libapache2-mod-php**

![Text alternatiu](7.png)

Seguido de esto,pondremos el comando:**sudo apt install -y php-fpm php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-ldap php-zip php-curl**

![Text alternatiu](8.png)

Finamlmente reiniciamos el servidor con el siguiente comando:sudo systemctl restart apache2

![Text alternatiu](9.png)
