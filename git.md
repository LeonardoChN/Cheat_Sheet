# Codigos de Git

======
======
### Configuracion inicial

```bash
$ git config --global user.name "[name]
$ git config --global user.email "[email address]"
$ git config --global color.ui auto
```
======
======
### Comandos basicos
- Iniciar (dentro de la carpeta)
```bash
git init 
```
- Consultar estado 
```bash
git status
```
- Agregar archivos o documentos (Todos) 
```bash
git add .
```
- Comentar
```bash
git commit -m "[descriptive message]"
```
- Agregar el repositorio de GitHub (primera vez del proyecto)
```bash
git remote add origin [Url]
```
- Push primera vez

```bash
git push -u origin main
```

- Push
```bash
git push
```

======
======
### Git en Grupo

- Clonar repositorio
```bash
git clone [url]
```
- Bajar la Ultima Actualización
```bash
git pull
```
======
======
### Ramas en Git

- Listar las ramas
```bash
git branch
```
- Crear nueva rama
```bash
git branch [branch-name]
```
- Cambiarse a una rama
```bash
git checkout [branch-name]
```
- Crear Rama y Cambiarse
```bash
git checkout -b [branch-name]
```
- Unir todo en 1 rama (la rama especificada con la rama actual)
```bash
git merge [branch]
```
- Eliminar Rama
```bash
git branch -d [branch-name]
```
======
======
### Otros Comandos
- Eliminar un archivo o documento
```bash
git rm [file]
```

- Quitar git a un archivo especifico (Rastreo)
```bash
git rm --cached [file]
```

- Renombrar un Archivo
```bash
git mv [old_filename.txt] [new_filename.txt]
```

- Enumera el Historial
```bash
git log

```

- Rehacer todo antes del comit seleccionado
```bash
git reset [commit]
```
```bash
git reset --hard [commit]
```

======
======
### Flujo de Trabajo en Git (Ejemplo)

1. Iniciamos en Rama MAIN
```sh
main: o---o
```

2. Creamos nueva rama 
```bash
(git checkout -b feature)
```
```sh
main:    o---o
             \
feature:       o
```

3.  Trabajamos en la rama feature normalmente
```bash
git add .
git commit -m "Add new feature"
```
```sh
main:    o---o
             \
feature:       o---o
```

4. Fusionamos Rama Feature a Main
```bash
git checkout main
git merge feature
```
```sh
main:    o---o---o---o---o---o---o
             \               /
feature:       o---o---o---o
```

5. Eliminamos Feature (Si no lo necesitamos)
```bash
git branch -d feature

```
```sh
main:    o---o---o---o---o---o---o

```

======
======
### Buenas Practicas de los Commits

```sh
Add: significa que se añade un nuevo archivo
```

```sh
Change: significa que se modifica un archivo existente
```

```sh
Fix: significa que se arregla un bug.
```

```sh
remove: Significa que se elimino un archivo existente
```
