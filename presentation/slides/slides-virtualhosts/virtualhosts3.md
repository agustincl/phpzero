## Crear directiva VirtualHost en Apache (1/2)

Editar el fichero *"httpd-vhosts.conf"* dentro del directorio *"conf/extra"* dentro del directorio de Apache y realizar los siguientes cambios:

1. Quitar los espacios después de especificar el puerto (después de los dos puntos ":").

2. Crear una directiva &lt;VirtualHost&gt; para localhost (si no existe) y otra para nuestro nuevo sitio ([Ver siguiente &rarr;](#/4)).