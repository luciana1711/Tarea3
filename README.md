# Directorios Compartidos y Multiples Maquinas Virtuales en Vagrant
Este proyecto presenta como compartir directorios entre un host y la maquina virtual, la creacion de multiples maquinas virtuales con diferentes sistemas operativos y provision de programas independiente.

Se definen dos maquinas virtuales Diferentes:
 web_1 con ubuntu/xenial64 escuchará por el puerto 8080.
 web_2 con ubuntu/bionic64 escuchará por el puerto 8008. Esta maquina tendra instalado un programa adicional htop

Este repositorio tiene los siguientes archivos:
* [Vagrantfile](Vagrantfile) Archivo que permite aprovisionar por linea de comandos dos maquinas virtuales con las caracteristicas previamente descritas
* [install-apache.sh](install-apache.sh) script de intalacion de apache
* [www_1](www_1) Directorio en el host donde se encuentran los archivos web disponibles del servidor web_1 con su respectivo archivo HTML
* [www_2](www_2) Directorio en el host donde se encuentran los archivos web disponibles del servidor web_1 con su respectivo archivo HTML

