## mysqldump 3/4

Para poder importar una base de datos al servidor, previamente deberemos crearla:<br />
<span style="color:#268BD2; background: #003542;">CREATE DATABASE nombre_base_de_datos;</span><br /><br />
 
Para restaurar una base de datos desde un archivo.sql:<br />
<span style="color:#268BD2; background: #003542;">$ mysqldump -u root -p nombre_base_de_datos < copia_seguridad.sql</span>