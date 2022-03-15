# masteruah

### Clonar repositorio

Para clonar el repositorio, una vez creado, he usado en la consola de Windows el comando "git clone https://github.com/victor-aljama/masteruah/"

### Commit inicial

Usamos el comando "git add README.md" para prepararlo para realizar el commit y tras esto usaremos el comando "git commit -m "commit inicial"".

Una vez hemos realizado el commit  subiremos el archivo README.md modificado al repositorio de GitHub mediante el comando "git push https://github.com/victor-aljama/masteruah/".

### Creación archivo .txt

En el siguiente apartado crearemos un archivo con formato .txt desde la consola, para ello ejecutaremos "type nul > 1.txt" y después lo añadiremos al repositorio local con el comando "git add 1.txt". Podemos comprobar que efectivamente se ha subido al repositorio local usando "git status".![image-20220314170837861](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220314170837861.png)

### Creación de una etiqueta

Para crear un tag escribiremos "git tag v0.1 -m "Esta es la version inicial"" y tras esto podremos mostrarlo usando "git show v0.1"![image-20220314174115827](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220314174115827.png)

Para subirlo necesitamos el comando "git push origin v0.1"

### Crear una nueva rama y archivo .txt en ella

Si queremos crear una rama nueva introduciremos el código "git branch v0.2" y para posicionarnos en ella haremos uso de "git checkout v0.2". Podemos comprobar que nos encontramos en dicha rama con "git branch". Utilizaremos el mismo comando para crear el archivo2.txt (type nul > 2.txt)

### Merge directo

Nos posicionamos en la rama main con "git checkout main" y después usamos "git merge v0.2" para hacer merge directo.![image-20220314201421905](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220314201421905.png)

### Merge con conflicto

Abrimos el archivo 1.txt mediante el comando "start 1.txt", lo modificamos, lo guardamos y hacemos commit y realizamos el mismo proyecto en la rama v0.2, para posicionarnos sobre ella recuerdo que debemos usar el comando "git checkout v0.2". Una vez que hayamos hecho "git push https://github.com/victor-aljama/masteruah2" y hayamos subido los archivos modificados en ambas ramas nos volvemos a posicionar en la rama main.

Para comprobar que efectivamente hay diferencias entre las ramas introducimos en la consola "git diff main v0.2" y se nos mostrarán todas las diferencias que existen en todos los archivos de cada rama.<img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315104826136.png" alt="image-20220315104826136" style="zoom:50%;" />

Esto nos servirá para saber qué cambios tenemos que hacer y en qué rama para conservar la versión deseada. Una vez hayamos entrado en los archivos necesarios para modificarlos finalmente podremos hacer el merge que nos piden mediante el código ya visto estando antes posicionados en la rama main: "git merge v0.2" ![image-20220315105138475](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315105138475.png)

### Lista de ramas

Para mostrar una lista de las ramas que hemos creado basta con introducir el siguiente comando:![image-20220315110245406](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315110245406.png)

### Eliminar rama y crear etiqueta

Para eliminar la rama v0.2 solamente tendremos que usar "git branch -d v0.2" o, como ha sido mi caso al no estar completamente sincronizada con la rama remota, "git branch -D v0.2". Una vez la hemos borrado a nivel local, para hacerlo a nivel remoto utilizaremos "git push origin --delete v0.2".![image-20220315111227480](C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315111227480.png)

Para crear la etiqueta con el mismo nombre de la rama seguiremos el mismo proceso que con la etiqueta v0.1.

### Perfil  de  GitHub

Esta captura pertenece a mi perfil de github: <img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315111658591.png" alt="image-20220315111658591" style="zoom: 33%;" />

### Autenticación en dos factores

Para realizar la autenticacion en dos factores tenemos que acceder a ajustes>autenticacion en dos factores y seguir los pasos que nos indican. Al final nos aparecerá esta pantalla<img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315112046826.png" alt="image-20220315112046826" style="zoom: 33%;" />

### Perfil GitHub de mis compañeros

Estos son los compañeros a los que he seguido en github:

<img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315112441776.png" alt="image-20220315112441776" style="zoom:35%;" /><img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315112535921.png" alt="image-20220315112535921" style="zoom:41%;" /><img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315112637849.png" alt="image-20220315112637849" style="zoom:38%;" /><img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315112732952.png" alt="image-20220315112732952" style="zoom:37%;" />

Para añadir una estrella a sus repositorios debemos acceder a dicho apartado en cada uno de sus perfiles y pulsar sobre el icono de la estrella.

### Tabla con información de compañeros de clase

|            NOMBRE             |                           GITHUB                            |
| :---------------------------: | :---------------------------------------------------------: |
|      Javier García Ruiz       | [GitHub Javier García](https://github.com/JavierGarciaRuiz) |
|   Javier Escribano Claudel    | [GitHub Javier Escribano](https://github.com/javieresccla)  |
| Rafael Damián Cristea Cristea |  [GitHub Damián Cristea](https://github.com/MrDamian1723)   |

### Colaboradores

Si queremos añadir colaboradores al repositorio para que lo puedan modificar sin necesidad de realizar pull requests accederemos al repositorio deseado>ajustes>colaboradores>añadir. Una vez aquí necesitamos su email o nombre de usuario para enviar una invitación. El resultado final es este: <img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315125447349.png" alt="image-20220315125447349" style="zoom:50%;" />

### Organizaciones

Crearemos una nueva organización pulsando en el símbolo + en la parte superior y posteriormente en nueva organización, desde aquí no tenemos más que seguir las instrucciones que nos dan y cumplir el requisito que nos piden del nombre, en mi caso "misteruah-victor-aljama".

<img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315131918097.png" alt="image-20220315131918097" style="zoom:50%;" />

### Equipos

Para crear los equipos accederemos a la organización>equipos>nuevo. En este apartado crearemos ambos apartados y añadiremos a las personas deseadas. Tras esto pulsaremos sobre "ajustes" de la organización y configuraremos a nuestro gusto los permisos para miembros y administradores.

### Fork y pull request

Para realizar los forks tendremos que buscar y acceder al repositorio de dos compañeros buscando el nombre del mismo, después, en la esquina superior derecha pulsaremos sobre "fork", lo que hara que se descargue una copia del archivo en nuestro perfil. En este punto tendríamos que usar en la consola el comando "git clone https://github.com/victor-aljama/Pagina-web.git" para guardar una copia en nuestro repositorio local y así poder editar el código de html y escribir nuestro nombre en el mismo. Tras esto tenemos que guardar los cambios y enviar el html editado de vuelta al repositorio remoto y sollicitar el pull request al autor para que añada al código los cambios que nosotros hemos realizado. Esto lo haremos pulsando sobre "pull request" en su repositorio donde tiene el código de la página web y elegir las ramas que queremos comparar, que en este caso serían su rama donde tiene almacenado el documento original y nuestra rama con el archivo modificado.

Una vez la otra persona nos envíe su pull request tendremos que acceder a nuestro repositorio y pulsar en el apartado de pull request, aquí nos aparecerán las solicitudes y tendremos que decidir su hacemos merge o no con la versión que hemos creado y la versión modificada por la otra persona. Llegados a este punto y después de aceptar la solicitud, nuestro archivo .html quedaría modificado.

<img src="C:\Users\victo\AppData\Roaming\Typora\typora-user-images\image-20220315161625922.png" alt="image-20220315161625922" style="zoom:50%;" />

En este caso solamente he podido realizar uno de los dos pull request que se pedían, ya que nadie más ha conseguido llegar a este punto por el momento.

Ambos hemos modificado los ajustes de nuestros repositorios para que la vista de los mismos sea pública. No obstante, dejo aquí los enlaces.

- https://github.com/masteruah-victor-aljama/prueba1.git (Mi repositorio)
- https://github.com/victor-aljama/Pagina-web.git (Fork del repositorio de Javi)
- https://github.com/masteruah-javieresccla/Pagina-web (Repositorio de Javi)
