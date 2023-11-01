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

-----

- Añadir fichero 1.txt

Creo el fichero "1.txt" con "touch". 

-Crear una rama v0.2

utilice git branch v0.2 y para mover a esa rama usé git checkout v0.2. 
Añadí fichero "2.txt" en la rama v0.2 con "touch v0.2.txt" y para subir a remoto: git add ., git commit -m "creación rama remota" y por ultimo git push origin v0.2.

- Merge directo

me posicioné en main con "git checkout main", y realice el merge con "git merge v0.2". Luego, lo subí a remoto para ver el cambio con: git add ., git commit -m "git merge" y git push origin main.

- Merge con conflicto

En rama main pongo Hola accediendo al archivo 1.txt y lo escribo. En git bash utilizo git add ., git commit -m "hola en fichero 1.txt" y hago git push -u origin main. 
Git checkout para moverme a la rama v0.2
