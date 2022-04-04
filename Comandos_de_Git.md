# Comandos de Git

## Iniciar un repositorio

```powershell
$ git init
```
## Verificar status de los archivos
Esta comando listará los archivos "trakeados" y "untracked"

```powershell
$ git status
```

## Agregar archivos al Tracking de Git

Para agregar todo los archivos modificados

```powershell
$ git add -A
```
ó

```powershell
$ git add .
```
Para agregar un archivo específico
```powershell
$ git add index.html
```

## Hacer "commit" de los cambio

```powershell
$ git commit -m "Mensaje de commit"
```
## Ver historia de los cambios
```powershell
$ git log
```
## Clonar un repositorio existente

Usando el URL de la página de Github

```powershell
$ git clone https://github.com/Latis-Informatica/LTS_Implementacion_Latis.git
```
Una vez clonado cambiarse al la carpeta **LTS_Implementacion_Latis** para empezar a trabajar.

## Subir cambios a Github
La primera vez
```powershell
$ git push origin main
```
Luego se puede usar sól 

```powershell
$ git push
```
## Descargar la última versión
```powershell
$ git pull origin main
```
## Crear un rama
Crear nueva 'rama' con el nombre '**mirama**'
```powershell
$ git branch mirama
```
### Cambiarse a una rama
```powershell
$ git checkout mirama
```
## Crear una rama y cambiarse
```powershell
$ git checkout -b mirama
```
## Empujar 'mirama' al repositorio remoto
La primera vez
```powershell
$ git push -u origin mirama
```
Luego 
```powershell
$ git push
```
## Hacer merge de 'mirama'

Cambiarse a la rama que va a recibir los cambios

  Ej: **main**

```powershell
$ git checkout main
```
Luego, hacer el merge de **mirama**
```powershell
$ git merge mirama
```
## Borrar una rama remota
```powershell
$ git push origin --delete mirama
```
## Borrar una rama local
```powershell
$ git branch -d mirama
```














