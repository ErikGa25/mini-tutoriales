## Git

**Más usados**
```
1. git pull (bajar los cambios)
2. [git add .] ó [git add -A] (agregar todos los cambios)
3. git commit -m 'Mensaje' (descripción de los cambios que creamos)
4. git push (subir los cambios)
5. git status (ver el estado de los cambios)
6. git checkout nombre_rama (cambiarse de rama)
```

**Otros comandos**
```
1. git init (inicializar un repositorio)
2. git config user.email "email@dom.com" (agregar tu correo al repositorio)
3. git config user.name "User" (agregar tu usuario al repositorio)
4. git clone [link] (clonar el proyecto)
5. git branch -a (mostrar todas las ramas locales)
6. git config --list (mostrar la configuración del repositorio)
```

---

## Mercurial

**Más usados**
```
1. hg pull (bajar los cambios)
2. hg update (agregar los cambios bajados)
3. hg addremove (solo si creamos algún archivo)
4. hg commit -m 'Mensaje' -u usuario (descripción de los cambios que creamos)
5. hg push (subir los cambios)
6. hg status (ver el estado de los cambios)
```

**Otros comandos**
```
1. hg log -l 4 -b default -G (ver los últimos commits creados)
2. hg up nombre_rama (cambiarse de rama)
3. hg graft 1024 (pasar un commit a otra rama)
```

---

## Configuraciones para .htaccess

**Quitar la extensión .html de la url**
```
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME}.html -f
RewriteRule ^(.*)$ $1.html
```

**Quitar la extensión .php de la url**
```
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME}.php -f
RewriteRule ^(.*)$ $1.php
```

**Denegar la vista de archivos de un directorio**
```
Options All -Indexes
```

---

## Configuración Personal de Visual Studio Code
```
{
    "editor.fontFamily": "'Courier New', monospace",
    "editor.wordWrap": "on",
    "files.autoSave": "onFocusChange",
    "editor.fontSize": 16,
    "workbench.iconTheme": "vscode-icons",
    "workbench.colorTheme": "CodeSandbox"
}
```
**Mis extensiones de uso**
```
- Beautify
- Bracket Pair Colorizer
- CodeSanbox Theme
- Color Picker
- Git History
- GitLens -- Git supercharged
- Laravel Snippets
- Live Sass Compiler
- vscode-icons
- Awesome Flutter Snippets
- Dart
- Flutter
```

---
## Instalación de LAMP en Ubuntu
```
- sudo apt install -y apache2 apache2-utils (para instalar apache)
- sudo service apache2 status (verificamos que el proceso se este ejecutando)
- sudo chown www-data:www-data /var/www/html/ -R (cambiamos el usuario del directorio html)
- sudo apt install mariadb-server mariadb-client (instalamos mariadb)
- sudo service mariadb status (verificamos que el proceso se este ejecutando)
- sudo mysql_secure_installation (iniciamos la instalación segura)
- sudo apt install php7.4 libapache2-mod-php7.4 php7.4-mysql php-common php7.4-cli php7.4-common php7.4-json php7.4-opcache php7.4-readline php7.4-mbstring php7.4-curl (instalamos php)
- sudo a2enmod php7.4 (habilitamos el modulo de php)
- sudo service apache2 restart (reiniciamos el servidor)
- sudo nano /var/www/html/info.php (escribimos la siguiente línea: <?php phpinfo(); ?>)
- sudo apt install phpmyadmin (instalamos phpmyadmin)
- sudo nano /etc/apache2/apache2.conf (hasta el final del archivo colocamos lo siguiente: Include /etc/phpmyadmin/apache.conf)
- sudo mariadb -u root -p (entramos a la base de datos)
- ALTER USER 'root'@'localhost' IDENTIFIED BY 'password'; (cambiamos el password)
- FLUSH PRIVILEGES; (cargamos los valores de la BD)
- sudo service apache2 restart (reiniciamos el servidor)
```

## Configuración apache (opcional)
```
- sudo nano /etc/apache2/apache2.conf
Modificar:
<Directory /var/www/>
	#AllowOverride None
        AllowOverride All
</Directory>
- sudo a2enmod rewrite
- sudo service apache2 restart
```
