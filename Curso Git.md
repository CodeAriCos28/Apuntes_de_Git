# Hola Mundo Curos de Git

# Configuar git 
## Para configuar el Nombre de tu Git usa:
```
git config --global user.name ["Tu nombre"]
```
## Para configurar Git con el correo eletronico usa:
``` 
git config --global user.name [Tu correo]
```
## Para que Git tenga a Vscode Como Predeterminado Usa:
```
git config --global core.editor "code --wait"
```
## Para ver el Archivo de configuracion Usa:
```
git config --global -e
```
## Para que Git sepa como tratar los santo de linea entre Linux y Windows usa:
```
git config --global core.editor true 
```
Para Linux y mac usa:
```
git config --global core.editor input
```
## para que git siempre escoja a la rama main por defecto usa:

```
git config --global init.defaultBranch main
```

## Para inicial un repositorio usa:
```
git ini
```
## Para ver el estado actual del repositorio usa:
```
git status
```
Para mejor formato del estado usa:
```
git status -s
```
## Para selecional los archivo usa:
seleciona todo los archivos
```
git add .
```
Seleciona los archivos que quieres subir, si son varios separados por espacio.
```
git add [Nombre de los archibos]
```
## Para comentar los archivos usa:
```
git commit -m "di que hiciste"
```
## Para eliminar Archivos usa:
```
git rm [Npmbre del Archivo]
```
Para remonbrar usa:
```
git mv [Nombre actual del Archivo] [Nombre que quieres que tenga]
```
## Para Sacar algun cambio que algamos hecho usa:
```
git restore --staged [Nombre del Archivo]
```
## Para recuperar algun Archivo Usa:
```
git restore [Nombre del Archvo]
```
## para ver cuales son los cambio que vamos a agregar usa:
se muestran todo los cambio que todabia no hemos subido.
```
git diff 
```
Este comando nos muestra los cambio que puedes comitiar.
```
git diff --staged
```
##  para ver el historial de de los commit.
```
git log --oneline
```
o tambien la normal
```
git log
```
## Para verificar en que rama estas usa:
```
git branch
```
## Para Crear una Nueva Rama usa:
```
git checkout -b [Nombre de la rama]
```
## para traer los cambio de una rama a otra usa:
Debes estar en la rama main para poder traer la otra a ella.
```
git merge [nombre de la rama que queremos traer a main]
```
# Github
## para activar el repositorio remoto de github usa:
```
git remote add origin [URL que te da el Repo]
```
## Para Activar la Rama Main en el Repo de Github usa:
```
git push -u origin [nombre de la rama]
```
## Para forzar la combinacion entre historiales no relacionados usa:
```
git pull origin main --allow-unrelated-histories
```
##  Fusiona Rama en main permitiendo historiales no relacionados:
Aqui tienes que usar la Rama que quieres emparejar con main:
```
git merge [Rama] --allow-unrelated-histories
```
## Para subir los cambios fucionados entre una Rama a Otra usa:
```
git push origin [Rama que estas]
```
## Para Descarga la información más reciente del repositorio remoto usa:
Antes de crear o cambiar a una rama que pueda existir en el remoto.
```
git fetch origin
```
## Para renombrar la rama master a main usa:
```
git branch -m master main
```
## Para Borrar la Rama remota usa:
```
git push origin --delete main
```
## Para Sobreescribir en el remoto usa:
verificando que tengas la copia actualizada y si alguien escribio abortar:
```
git push -u origin main --force-with-lease
```
## para cambiar permanentemente el comportamiento de git pull en todos los Repositorios de Git usa:
haciendo que siempre use rebase en lugar de merge al traer cambios del repositorio remoto:
```
git config --global pull.rebase true
```
## Para remover el un remote usa:
```
git remote remove origin
```
