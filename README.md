# devjumpers

-Repositorio devjumpers

Creo un repositorio en Github llamado devjumpers. Para esto me creé una cuenta en Github, fui a mi perfil y me dirigí a crear repositorio nuevo.

Ejecuté los siguientes comandos para que cuando cargué algun commmit a github pueda verlo en mi consola con el siguiente username:

git config --global user.name gonzalolamas
git config --global user.email lamasgonzaloezequiel@gmail.com

-documento README.md creado para subirlo a remoto:

utilicé git init, git add . para agregar el archivo, git commit -m, git remote add origin "link del repositorio de github" y luego realice git push -u origin main para que se suba a la rama principal.
 
-------

-Ignorar archivos

Para realizar la creación del archivo txt. use el comando "touch". Luego, mkdir "privada" para crear la carpeta.
Crear .gitignore con "touch" y para que estos archivos sean ignorados, escribí el nombre de ellos en el archivo txt. de ".gitignore".
privada/
*privado.txt

-----

- Añadir fichero 1.txt

Creo el fichero "1.txt" con "touch". 

------

-Crear una rama v0.2

utilice git branch v0.2 y para mover a esa rama usé git checkout v0.2. 
Añadí fichero "2.txt" en la rama v0.2 con "touch v0.2.txt" y para subir a remoto: git add ., git commit -m "creación rama remota" y por ultimo git push origin v0.2.

------

- Merge directo

me posicioné en main con "git checkout main", y realice el merge con "git merge v0.2". Luego, lo subí a remoto para ver el cambio con: git add ., git commit -m "git merge" y git push origin main.

------

- Merge con conflicto

En rama main pongo Hola accediendo al archivo 1.txt y lo escribo. En git bash utilizo git add ., git commit -m "hola en fichero 1.txt" y hago git push -u origin main. 
Git checkout para moverme a la rama v0.2 y coloco "Adios" en el fichero 1.txt.
Vuelvo a la rama main y hago git merge v0.2.

------

- Listado de ramas
  
Hago git branch --merged para ver las ramas fusionadas y git branch --no-merged para ver las ramas no fusionadas.

------

- Arreglar conflicto
  
Primero corrijo en los cambios en el txt y luego use "git add ." para guardar cambios, y git commit -m "conflicto resuelto" para que se resuelva el problema.

------

-Borrar rama

git branch -D v0.2 para borrar la rama v0.2

------

-Listado de cambios

use git log --oneline --decorate --all --graph

*   e6faf9b (HEAD -> main, origin/main, origin/HEAD) conflicto solucionado
|\
| * 958c022 (origin/v0.2, v0.2) adios en el fichero 1.txt
| * de2c530 agregando en el archivo git ignore el archivo de privado.txt
* | d5a94a1 agregando documentación
* | 7e8afe2 hola en fichero 1.txt
* | e74ea38 Delete privado.txt
* | 7fb7100 el archivo .txt no se ignoraba ya que debe colocarse el formato del
archivo en gitignore
* | 899c4fe git merge
|/
* b64677e agregando documentación
* 6fff103 creación rama remota v0.2
* 88d4dc8 agregando captura de imagen de primeros pasos
* 691240c commit inicial

-Crear una tabla

realice la creación de la tabla en el readme con ayuda de documentación, a traves de las líneas se genera un recuadro.

| Nombre  | Github |
| ------------- | ------------- |
| Luciano Verchelli | [GitHub perfil]([https://pages.github.com/](https://github.com/LucianoVerchelli)  |
| Aixa Cobos  | [GitHub perfil](https://pages.github.com/)  |
| Leila Balmaceda  | [GitHub perfil](https://pages.github.com/)  |
