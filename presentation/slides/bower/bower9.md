<span class="mysql-color">Destino de paquetes</span><br/>
El destino predeterminado para los paquetes es el folder <em>bower_components</em>.

En la arquitectura web el directorio mas usado para estos paquetes es vendor por lo que
crearemos un archivo <b>.bowerrc</b> y introduciremos el siguiente codigo:
<pre>	{
		"directory": "public/vendor"
		"json":"bower.json"
	 }
</pre>
Lo cual hará que los paquetes se guarden en el folder public/vendor o cualquiera que deseemos.