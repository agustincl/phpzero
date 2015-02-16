## mysqldump 4/4

Para realizar copias de seguridad en un hosting remoto:<br />
<span style="color:#268BD2; background: #003542;">$ mysqldump -u usuario_remoto -p -h ip_host_remoto nombre_base_de_datos > copia_seguridad_remota.sql </span><br /><br />
 
El comando scp también es muy útil ya que nos permite transferir archivos desde una máquina local a otra remota, usando conexión ssh (encriptada):<br />
<span style="color:#268BD2; background: #003542;">$ scp copia_seguridad.sql usuario_remoto@ip_host_remoto:/ruta/ejemplo</span>