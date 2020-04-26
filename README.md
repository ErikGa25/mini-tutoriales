## Git

1. git pull (bajar los cambios)
2. git add . (agregar los cambios)
3. git commit -m 'Mensaje' (descripción de los cambios que creamos)
4. git push (subir los cambios)
5. git status (ver el estado de los cambios)

---

## Mercurial

**Subir cambios**

1. hg pull (bajar los cambios)
2. hg update (agregar los cambios bajados)
3. hg addremove (solo si creamos algún archivo)
4. hg commit -m 'Mensaje' -u usuario (descripción de los cambios que creamos)
5. hg push (subir los cambios)
6. hg status (ver el estado de los cambios)


**Pasar cambios a otra rama**

1. hg log -l 4 -b default -G (ver los últimos commits creados)
2. hg up nombre_rama (cambiarse de rama)
3. hg graft 1024 (pasar un commit a otra rama)
4. hg push (subir los cambios)
