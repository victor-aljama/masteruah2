# masteruah2

1- Para clonar el repositorio, una vez creado, he usado en la consola de Windows el comando "git clone https://github.com/victor-aljama/masteruah/"

2- Usamos el comando "git add README.md" para prepararlo para realizar el commit y tras esto usaremos el comando "git commit -m "commit inicial"".

3- Una vez hemos realizado el commit  subiremos el archivo README.md modificado al repositorio de GitHub mediante el comando "git push https://github.com/victor-aljama/masteruah/".

4- En el siguiente apartado crearemos un archivo con formato .txt desde la consola, para ello ejecutaremos "type nul > 1.txt" y después lo añadiremos al repositorio local con el comando "git add 1.txt". Podemos comprobar que efectivamente se ha subido al repositorio local usando "git status".![image-20220314170837861](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220314170837861.png)

5- Para crear un tag escribiremos "git tag v0.1 -m "Esta es la version inicial"" y tras esto podremos mostrarlo usando "git show v0.1"![image-20220314174115827](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220314174115827.png)

Para subirlo necesitamos el comando "git push origin v0.1"

6- Si queremos crear una rama nueva introduciremos el código "git branch v0.2" y para posicionarnos en ella haremos uso de "git checkout v0.2". Podemos comprobar que nos encontramos en dicha rama con "git branch". Utilizaremos el mismo comando para crear el archivo2.txt (type nul > 2.txt)

7- Nos posicionamos en la rama main con "git checkout main" y después usamos "git merge v0.2" para hacer merge directo.![image-20220314213512471](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220314213512471.png)

8- Abrimos el archivo 1.txt mediante el comando "start 1.txt", lo modificamos, lo guardamos y hacemos commit y realizamos el mismo proyecto en la rama v0.2, para posicionarnos sobre ella recuerdo que debemos usar el comando "git checkout v0.2". Una vez que hayamos hecho "git push https://github.com/victor-aljama/masteruah2" y hayamos subido los archivos modificados en ambas ramas nos volvemos a posicionar en la rama main.

Para comprobar que efectivamente hay diferencias entre las ramas introducimos en la consola "git diff main v0.2" y se nos mostrarán todas las diferencias que existen en todos los archivos de cada rama.![image-20220315104826136](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315104826136.png)

Esto nos servirá para saber qué cambios tenemos que hacer y en qué rama para conservar la versión deseada. Una vez hayamos entrado en los archivos necesarios para modificarlos finalmente podremos hacer el merge que nos piden mediante el código ya visto estando antes posicionados en la rama main: "git merge v0.2" ![image-20220315105138475](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315105138475.png)

9- Para mostrar una lista de las ramas que hemos creado basta con introducir el siguiente comando:![image-20220315110245406](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315110245406.png)

10- Para eliminar la rama v0.2 solamente tendremos que usar "git branch -d v0.2" o, como ha sido mi caso al no estar completamente sincronizada con la rama remota, "git branch -D v0.2". Una vez la hemos borrado a nivel local, para hacerlo a nivel remoto utilizaremos "git push origin --delete v0.2"![image-20220315111227480](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315111227480.png)

