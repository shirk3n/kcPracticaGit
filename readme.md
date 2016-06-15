# Respuestas práctica Git

---

### ¿Qué comando utilizaste en el paso 11? ¿Por qué? 
> `git reset --hard HEAD~1`

Porque si usamos el comando reset con `--hard` bajaría los punteros al anterior commit pero no perdeíamos los cambios realizados,
por el contrario el comando reset con `--hard` si se pierde los cambios (este es menos conservador). Lo he comprobado con
`nano git-nuestro.md`.

---

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 
>`git reflog`

>`git reset <ID>`

>`git checkout --git-nuestro.md`

Porque con el `git reflog` buscamos exáctamente el ID donde se hizo el commit. Una vez que tengamos ese identificador, nos movemos con el `git reset <ID>`
y descarto los cambios con `git checkout --git-nuestro.md>`.

---

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No, porque la rama **styled** ya contiene a **Master**, con lo cual te aparece en consola *Already up-to-date*.

---

### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
Sí, porque el archivo **git-nuestro.md** coincide lineas entre los dos archivos en distintas ramas, con lo que hay que resolver el conflicto.

---
### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
No, porque no coincide ninguna linea de código que se haya cambiado.

---

### ¿Qué comando o comandos utilizaste en el paso 25? 
>`git graph`

Ya tenía configurado el config así:
>`git config --global alias.graph "log --graph --decorate --pretty=oneline"`

--- 

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si, aunque no tiene sentido porque la rama title contiene a la master.

---

### ¿Qué comando o comandos utilizaste en el paso 27?
> `git reset HEAD~1`

---

### ¿Qué comando o comandos utilizaste en el paso 28?
>`git checkout --git-nuestro.md`

---

### ¿Qué comando o comandos utilizaste en el paso 29?
>`git checkout master`
>`git branch -D title`

---

### ¿Qué comando o comandos utilizaste en el paso 30?
>`git reflog`
>`git reset <ID>`
>`git checkout --git-nuestro.md`

---

### ¿Qué comando o comandos usaste en el paso 32?
>`git log`
>`git reset --hard <ID>`
Con el comando `git log` busco el ID inicial. Mensaje del commit: Creo el padre nuestro versionado a Git.

---

### ¿Qué comando o comandos usaste en el punto 33?
>`git log`
>`git reset --hard <ID>`
Con el comando `git log` busco el ID. Mensaje del commit: Añado título al padre nuestro versionado a Git.

