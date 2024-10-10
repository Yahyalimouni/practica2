# Practica 2

Pasos para instalar y configurar Nginx en Debian 12.

## Instalación servidor web Nginx
Instalamos Nginx
![01_sudo_apt_install_nginx.png](../capturas/01_sudo_apt_install_nginx.png)

Verificamos La instalacion:
![02_verificar_la_instalacion.png](../capturas/02_verificar_la_instalacion.png)

## Creacion de la carpeta de la web
Creacion de la carpeta de la web en /var/www/
![03_creacion_del_directorio.png](../capturas/03_creacion_del_directorio.png)

Inicializar el repositorio git, y clonar el repo https://github.com/cloudacademy/statis-website-example
![04_inicializar_git.png](../capturas/04_inicializar_git.png)
![05_clonar_repo.png](../capturas/05_clonar_repo.png)

Dar permisos al usuario `yahya`
![06_chown_cambiar_prop.png](../capturas/06_chown_cambiar_prop.png)
![07_chmod_755_practica2.png](../capturas/07_chmod_755_practica2.png)

Comprobacion del funcionamiento de Nginx
![08_comprobar_funcionamiento_nginx.png](../capturas/08_comprobar_funcionamiento_nginx.png)

## Configuración de servidor web NGINX
Abrimos el fichero de configuracion /etc/nginx/sites-available/vuestro_dominio
![09_abrir_fichero_configuracion.png](../capturas/09_abrir_fichero_configuracion.png)

Configurarlo
![09_fichero_configuracion.png](../capturas/09_fichero_configuracion.png)

Crear el archivo simbolico al sites-enabled
![10_crear_archivo_simbolico.png](../capturas/10_crear_archivo_simbolico.png)

Reiniciar el servidor
![11_reiniciar_servidor.png](../capturas/11_reiniciar_servidor.png)

Modificar el archivo C:\Windows\System32\drivers\etc\hosts poniendole la ip del servidor
![12_ip_debian.png](../capturas/12_ip_debian.png)
![12_DNS_local_etc_hosts_.png](../capturas/12_DNS_local_etc_hosts_.png)

## FTP
El FTP es un protocolo de transferencia de archivos entre sistemas conectados a una red TCP. Como su nombre indica, se trata de un protocolo que permite transferir archivos directamente de un dispositivo a otro. 

## Configuracion SFTP en Debian
Instalamos vsftpd
![13_instalar_vsftpd.png](../capturas/13_instalar_vsftpd.png)

Creamos una carpeta ftp en /home/yahya
![13_crear_una_carpeta.png](../capturas/13_crear_una_carpeta.png)

Creamos los certitificados de seguridad de la conexion
![15_securizar_ftp.png](../capturas/15_securizar_ftp.png)
