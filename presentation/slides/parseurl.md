<section>
	<h1>parseURL</h1>
	<ul>
		Toma la URL de la petición.
		<pre><code>$_SERVER['REQUEST_URI']</code></pre>
		<p>Que obtiene en un string donde cada parte de la URL va separada por barras.</p>
		<pre><code>'/controller/action/param1/value1/param2/value2'</code></pre>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
	<p>La descompone en partes.</p>
	<pre><code>explode('/', $_SERVER['REQUEST_URI'])</code></pre>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Y analiza el contenido para pasar al request el resultado.</p>
		<p>Según esté, correcta o haya algún fallo, actuará de la siguiente manera.</p>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si todo está correcto. Es decir, la URL es algo así</p>
		<pre><code>/controller/action/param1/value1/param2/value2</code></pre>
		<p>Entonces devolverá:</p>
		<li>Como controlador => controller</li>
		<li>Como acción => action</li>
		<li>Como parámetros => param1=value1 , param2=value2</li>
		
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si a la URL le falla un par parámetro-valor</p>
		<pre><code>/controller/action/param1/value1/param2</code></pre>
		<p>Entonces devolverá un error por falta de ese valor mandando:</p>
		<li>Como controlador => error</li>
		<li>Como acción => 412</li>
		<li>Como parámetros => </li>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si la URL es sin parámetros</p>
		<pre><code>/controller/action</code></pre>
		<p>Entonces devolverá:</p>
		<li>Como controlador => controller</li>
		<li>Como acción => action</li>
		<li>Como parámetros => </li>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si la URL tiene el controlador pero hay una acción o parámetro que no existe</p>
		<pre><code>/controller/not found</code></pre>
		<p>Entonces devolverá un error de página no encontrada enviando:</p>
		<li>Como controlador => error</li>
		<li>Como acción => 404</li>
		<li>Como parámetros => </li>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si la URL tiene sólo el controlador</p>
		<pre><code>/controller</code></pre>
		<p>Entonces devolverá:</p>
		<li>Como controlador => index</li>
		<li>Como acción => index</li>
		<li>Como parámetros => </li>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si la URL tiene sólo la barra o nada</p>
		<pre><code>/</code></pre>
		<p>o</p>
		<pre><code> </code></pre>
		<p>Entonces devolverá:</p>
		<li>Como controlador => index</li>
		<li>Como acción => index</li>
		<li>Como parámetros => </li>
	</ul>
</section>
<section>
	<h1>parseURL</h1>
	<ul>
		<p>Si la URL sólo tiene datos que no reconoce el parseURL</p>
		<pre><code>not found</code></pre>
		<p>Entonces devolverá un error de página no encontrada enviando:</p>
		<li>Como controlador => error</li>
		<li>Como acción => 404</li>
		<li>Como parámetros => </li>
	</ul>
</section>
