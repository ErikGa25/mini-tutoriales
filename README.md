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
2. git config user.email "User" (agregar tu correo al repositorio)
3. git config user.name "email@dom.com" (agregar tu usuario al repositorio)
4. git clone [link] (clonar el proyecto)
5. git brach -a (mostrar todas las ramas locales)
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

**Configuración Personal de Visual Studio Code**
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
