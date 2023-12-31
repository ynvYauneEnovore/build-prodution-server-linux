<h1>Upload for production project laravel-debian-server</h1>
<h2> <span>Desarrollador: Yovan R. Yaune Enovore</span></h2>

<h3>Paso 1: Preparación</h3>
Abre una terminal en tu computadora.

<h3>Paso 2: Actualiza tu sistema y prepara herramientas</h3>
Escribe y presiona Enter después de cada línea:
<pre><code>sudo apt update</code></pre>
<pre><code>sudo apt install lsb-release apt-transport-https ca-certificates software-properties-common -y</code></pre>

<h3>Paso 3: Instala Git</h3>

<pre><code>sudo apt install git</code></pre>

<h3>Paso 4: Instala Emacs</h3>

Elige a tu eleccón (nano) viene por defecto en la mayoría de OS basados en KERNEL LINUX.
<pre><code>sudo apt install emacs</code></pre>

<h3>Paso 5: Instala PHP 8.2 [DEBIAN]</h3>

<pre><code>sudo wget -O /etc/apt/trusted.gpg.d/php.gpg https://packages.sury.org/php/apt.gpg</code></pre>
<pre><code>sudo sh -c 'echo "deb https://packages.sury.org/php/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/php.list'</code></pre>
<pre><code>sudo apt update</code></pre>
<pre><code>sudo apt install php8.2</code></pre>

<h3>Paso 5: Instala PHP 8.2 [UBUNTU]</h3>

<pre><code>sudo apt update && apt upgrade -y</code></pre>
<pre><code>sudo add-apt-repository ppa:ondrej/php</code></pre>

<pre><code>sudo apt update</code></pre>
<pre><code>sudo apt install php8.2 -y</code></pre>

<pre><code>php --version</code></pre>

  
<h3>Paso 6: Instala el servidor de base de datos MariaDB</h3>

<pre><code>sudo apt install mariadb-server</code></pre>

<h3>Paso 7: Cambia la contraseña del usuario 'root' en MariaDB</h3>

<pre><code>mysql</code></pre>

Una vez en la interfaz de MySQL, ejecuta lo siguiente:
<pre><code>ALTER USER 'root'@'localhost' IDENTIFIED BY 'NUEVA_CONTRASEÑA';</code></pre>
Reemplaza NUEVA_CONTRASEÑA con la contraseña que deseas asignar. 
Luego, para salir de la interfaz de MySQL, escribe:
<pre><code>exit</code></pre>

<h3>Paso 8: Instala Composer</h3>
Sitio web:
<pre><code>https://getcomposer.org/</code></pre>

<h3>Paso 9: Instala extensiones y dependencias de PHP</h3>
Escribe y presiona Enter después de cada línea:
<pre><code>sudo apt install php-gd</code></pre>
<pre><code>sudo apt install php-curl</code></pre>
<pre><code>sudo apt install php-xml</code></pre>
<pre><code>sudo apt install php-zip</code></pre>
<pre><code>sudo apt install php-mysql</code></pre>
<pre><code>sudo apt install php-mbstring</code></pre>
<pre><code>sudo apt install php-unzip</code></pre>

