## mysqldump 2/4

Para exportar una base de datos a un archivo.sql necesitamos: tener un usuario con privilegios, abrir la consola de comandos, colocarnos en el directorio destino deseado y ejecutar el comando:<br /> 

<span style="color:#268BD2; background: #003542;">$ mysqldump -u root -p nombre_base_de_datos > copia_seguridad.sql</span><br />

Gracias a la inclusi�n del par�metro <span style="color:#268BD2">-p</span>, se nos pedir� introducir la contrase�a del usuario, de forma oculta, despu�s de su ejecuci�n.