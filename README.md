# iaw-practica-12

Crear una máquina virtual en Amazon EC2.

La Amazon Machine Image (AMI) que vamos a seleccionar para esta práctica será una Community AMI de Bitnami con la última versión de WordPress.
https://bitnami.com/stack/wordpress/cloud/aws/amis
https://console.aws.amazon.com/ec2/v2/home?region=us-east-1#LaunchInstanceWizard:ami=ami-05bb13389b5d8cb2e

tendremos que añadir 2g de ram

Cuando esté creando la in stancia deberá configurar los puertos que estarán abiertos para poder conectarnos por SSH y para poder acceder por HTTP/HTTPS.
SSH (TCP)22
HTTP (TCP)80
HTTPS (TCP)443

Crear un par de claves (pública y privada) para conectar por SSH con su instancia.

Una vez que haya iniciado su instancia deberá buscar cuál es la contraseña de administración del sitio WordPress.
en acciones , monitoreo y solucion de problemas, obtener registro del sistema

  65.416800] bitnami[542]: #########################################################################
[   65.423394] bitnami[542]: #                                                                       #
[   65.430034] bitnami[542]: #        Setting Bitnami application password to 'gXqwFHRfns4W'         #
[   65.436231] bitnami[542]: #        (the default application username is 'user')                   #
[   65.442226] bitnami[542]: #                                                                       #
[   65.448812] bitnami[542]: #########################################################################

Busque cuál es la dirección IP pública de su instancia y compruebe que puede acceder a ella desde una navegador web.

http://3.236.92.160/
