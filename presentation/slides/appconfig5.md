### Configuración de aplicaciones PHP

*getConfig* 

Función que devuelve la matriz asociativa con todos los parámetros de la aplicación
globales actualizados con los parámetros locales: 
```
<?php

function getConfig()
{   
    return (array_merge(require_once('../configs/global.php'),
                        require_once('../configs/local.php')
                        )
            );    
);
```