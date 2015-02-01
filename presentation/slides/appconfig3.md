### Configuración de aplicaciones PHP
##### Configuración global

*global.php* - Fichero que devuelve una matriz asociativa con los parámetros
por defecto para cualquier instalación:
```
<?php

return array (
    'filename'=> '../data/usuarios.txt',
    'config1'=>'data1',
    'config2'=>'data2',
    'view_path'=>$_SERVER['DOCUMENT_ROOT'].
    	'/../modules/application/src/application/views',
    
);
```