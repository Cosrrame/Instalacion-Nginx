# README - Configuración de Servidor Web con Nginx en Vagrant

Este proyecto configura un servidor web con Nginx en una máquina virtual Debian usando Vagrant. Se utiliza un repositorio GitHub para alojar un sitio estático.


## Pasos para Ejecutar



### Iniciar la máquina virtual

   
   vagrant up
   

### Acceder a la máquina virtual

   vagrant ssh


### Acceder al sitio web

   Abre tu navegador y accede a `http://192.168.57.10`.


## Preguntas

### ¿Qué pasa si no hago el link simbólico entre sites-available y sites-enabled de mi sitio web?

  Si no haces el link simbólico, Nginx no habilitará el sitio web, ya que no lo incluirá en su configuración activa. El sitio no será accesible.

### ¿Qué pasa si no le doy los permisos adecuados a /var/www/nombre_web?

  Si no ajustas los permisos correctamente, Nginx no podrá leer ni servir los archivos del sitio web, lo que resultará en un error 403 (prohibido) o 404 (no encontrado).