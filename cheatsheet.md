# Consigna
Realizar un resumen sobre el trabajo con git. Cada grupo debera contribuir con una sección determinada. 
Nota: el documento está escrito en [Markdown](https://guides.github.com/features/mastering-markdown/)

```bash
git -v 
```


## Configuración inicial
git config --global user.name "tu nombre" / otorga un nombre a la persona que este trabajando con git 
git config --global user.email "tu email" / otorga una direccion de correo a la persona que esta trabajando con git 
git config --global http.proxy http://192.168.0.250:3128 / habilita el uso del servidor proxy 

## Comenzando a trabajar
<<<<<<< HEAD
 **colaboracion belve,ricardo,medina,alvarez**
=======
 **colaboracion belve,ricardo,medina,gabo**
>>>>>>> 01d2e6739470e3f6c7fa6310f08b3e3c2a8af334
1) Para empezar se debe (primeramente realizar la configuracion inicial)
2) se debe realizar una carpeta con el siguiente comando: 
```bash
*mkdir [nombre de la carpeta]*
```
en la cual se guardan todos los documentos.
3) Luego se ingresa en esa carpeta con el siguiente comando: 
```bash
*cd [nombre de la carpeta]*
```
4) Luego mientras estes en la carpeta se realiza el siguiente comando:
```bash
*git init*
```
es para empezar a trabajar con git sino no te deja insertar comando

## Creando un repositorio local


<<<<<<< HEAD
## Clonando un repositorio
 **Esto fue hecho por medina y alvarez**
 Para obtener una copia de un repositorio GIT existente se tiene que ingresar elsiguiente comando
 ```bash
 *git clone [url]*
 ```
 Para clonar un repositorio remoto existente [SSH]
 ```bash
 *git clone git+ssh://[nombre de usuario en el servidor remoto][dirreccion ip] [ruta exacta de donde esta ubicado]*
 ```
 Para clonar un repositorio remoto existente [HTTPS]
 ```bash
 *git clone [URL]*
 ```
 una vez clonado el repositorio **se pueden realizar las mismas acciones que si 
hubiesemos iniciado nuestro propio repositorio local**
=======

## Clonando un reposito



>>>>>>> 01d2e6739470e3f6c7fa6310f08b3e3c2a8af334
## Trabajando con repositorios remotos 



## Diferencia entre fetch/merge y pull



## Etiquetas



## Gestión de logs

<<<<<<< HEAD
Podemos ver el historial de commits del proyecto usando el comando log.
Muestra el historial con el formato que indicamos:
git log --pretty=format:"%h - %an, %ar : %s"

Cambiamos la n por cualquier n�mero entero:
git log -n

Muestra los commits realizados despu�s de la fecha especificada:
git log --after="2016-04-07 00:00:00"

Muestra los commits realizados antes de la fecha especificada:
git log --before="2016-04-08 00:00:00"

Las banderas del comando git log se pueden usar juntas seg�n nos convenga:
git log --after="2016-04-07 12:00:00" --before="2016-04-07 12:30:00"

Este comando nos muestra el historial en una sola l�nea por commit:
git log --oneline


=======
<<<<<<< HEAD
## Deshaciendo cambi
=======
>>>>>>> 62eddef74fcc9ca6c5ffa44d16450760dee83d70
=======


>>>>>>> 090f30c2f65176aa1e0229e23952268b0b921272
## Deshaciendo cambios
**Los cambios pueden deshacer en cualquier momento.**
Ten cuidado, a veces no es posible recuperar algo luego que lo has deshecho. Esta es una de las pocas áreas en las que Git puede perder parte de tu trabajo si cometes un error.

**Para deshacer el commit perdiendo las modificaciones:**
Para deshacer el ultimo commit usaremos:

```bash
*git reset --hard HEAD~1*
```
Donde "HEAD 1" indica la cantidad de commit a retoceder.
La sintaxis "HEAD 1" del comando anterior la podríamos traducir como “El commit al que está apuntando la rama activa menos uno”.

**Para deshacer el commit manteniendo las modificaciones:**
Existe la posibilidad de eliminar el commit pero manteniendo las modificaciones que contiene ese commit en el área de trabajo. 
Para ello, ejecutaríamos el siguiente comando: 

```bash
*git reset HEAD~1*
```

Así que podemos seguir trabajando, corregir el bug o completar las modificaciones que habíamos dejado incompletas y hacer un nuevo commit con los cambios completos.