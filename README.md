#  Comandos básicos de Git y GitHub  

## Configuración inicial  

```bash
# Configurar nombre de usuario
git config --global user.name "TuNombre"

# Configurar correo (debe ser el mismo que en GitHub)
git config --global user.email "tuemail@example.com"

# Verificar configuración
git config --list

#cambiar editor por defecto (ej:visual studio code)
git config --global core.editor "code --wait"

#abrir configuracion por defecto en el editor por defecto 
code ~/.gitconfig

# Colores en la terminal
git config --global color.ui auto

# Idioma (ejemplo: inglés)
git config --global i18n.commitEncoding utf-8
git config --global i18n.logOutputEncoding utf-8

```

---


## Flujo básico de trabajo  

```bash
# Clonar un repositorio existente desde GitHub
git clone <url-del-repositorio>

# Verificar estado de los archivos (cambios pendientes)
git status

# Agregar archivos específicos al área de preparación
git add nombre-archivo

# Agregar todos los archivos modificados
git add .

# Guardar cambios en un commit con un mensaje deben ser claros y descriptivos.
git commit -m "Descripción clara del cambio"

#Cambiar solo el mensaje del último commit
git commit --amend -m "Nuevo mensaje correcto"

#Forzar el push (cuando sabes que quieres sobrescribir el commit)
git push origin master --force

#Evitar el force y traer primero el remoto
git pull origin master --rebase

# Enviar los cambios al repositorio remoto (GitHub)
git push origin main o master

```
---

## Actualizar el repositorio local  

```bash
# Descargar los últimos cambios de GitHub
git pull origin main o master
```

---

## Ramas (Branches)  

```bash
# Crear una nueva rama
git branch nombre-rama

# Combinar cambios de una rama a otra (ej. main)
git merge nombre-rama

# Crear y cambiar a la vez
git checkout -b nombre-rama

# Cambiar a una rama existente
git checkout nombre-rama

```

---



