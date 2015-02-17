### Configuración de aplicaciones PHP
##### Configuración local

*local.php* - Fichero que devuelve una matriz asociativa con los parámetros específicos
para una instalación local: 
```
<?php

return array (
    'filename'=> '../data/usuarios.txt',
    'config1'=>'data1',
    'config2'=>'data2'
    
);
```