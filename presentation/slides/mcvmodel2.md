## MODELO MVC
### Model View Controler
1. El usuario escribe la URL a la que quiere ir.
2. **.htaccess**: Se comprueban las directivas. Si *Allow override ON*, se puede leer el .htaccess.
3. **index.php**
4. **Config**: accede a las variables de configuración global y local.
5. **Router**: se analiza la dirección URL con **parseURL** y se enruta con **routeURL**.
6. **Request**: realiza la petición.
