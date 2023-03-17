# taller-git

Desde [GitHub](https://github.com/) cree un repositorio, con el boton que esta al lado izquierdo de la página, como se ve en la figura de abajo para su trabajo. 

Recuerde, como recomendación, ponerle un nombre que sea diciente de lo que representa el proyecto, o que este relacionado al problema que esta resolviendo.

Desde este punto en su computador vaya a la carpeta donde esta su proyecto.

dentro de esa carpeta habra su cliente de git (el cual puede ser, powershell, cmd, gitbash, etc...) y escriba los siguientes comandos: 

```bash
git init
git add --all
git commit -m "upload my proyect"
git branch -M main
git remote add origin https://github.com/NombreDeUsuario/NombreRepositorio.git
git push -u origin main
```

## Revisemos cada uno: 

1. ```bash
   git init
   ```

Este comando inicializa un proyecto de git en su equipo, en la carpeta `TareaIntegradora2` (carpeta usada para el ejemplo) donde usted trabajará y hará sus cambios

2. ```bash
   git add --all
   ```

Este comando agregará **TODOS** los cambios hechos en su repositorio (Nota: existen muchas formas de agregar cambios, esta les garantiza que todos los cambios hechos serán agregados)

3. ```bash
   git commit -m "upload my proyect"
   ```

Este comando se usa para identificar el cambio que esta subiendo al repositorio, se recomienda que el mismo sea en ingles y sea diciente del cambio que se va a subir, por ejemplo si usted fuera a subir la clase `Player` podría crear un commit que fuera `git commit -m "upload class player"` 



4. ```bash
   git branch -M main
   ```

Este comando creará su *Rama principal del proyecto* en la cual usted podrá subir cambios 

5. ```bash
   git remote add origin git@github.com:nombreUsuario/nombreProyecto.git
   ```

Este comando se usa para indicar que su repositorio local va a quedar sincronizado con el repositorio en la plataforma de GitHub, note que deberá cambiar `com:nombreUsuario` por su nombre de usuario y `nombreProyecto` por el nombre de su proyecto

6. ```bash
   git push -u origin main
   ```

Este comando debería de subir los cambios de su repositorio a la plataforma pero ... 

Si usted no ha configurado el cliente de git saldra un mensaje diciendo que debe indentificarse, para ello usaremos los diguientes comandos: 

```bash
git config --global user.email "your_email@example.com"
```

Donde deberá especificar el correo electronico con el que creo su cuenta de GitHub

```bash
git config --global user.name "your_user_name"
```

Donde deberá especificar su nombre de usuario en git

Ahora si, podrá subir sus cambios: 

```bash
git push -u origin main
```

Una vez hecho esto, en el caso de windows aparecerá una ventana que le pedirá que ingrese su nombre de usuario y contraseña, en el caso de Mac se los pedira por la terminal de comandos. 


Una vez hecho esto usted podrá subir mas cambios en su código al repositorio, por ejemplo, agreguemos el método `toString()` a una clase `Person` 

```java
public String toString(){
    return 
        "Nombre : " + name + "\n"
        "Cedula : " + cc + "\n"
        "Edad : " + years + "\n";
}
```

Luego de agregar este método vamos a nuestro cliente de git y hacemos: 

```bash
git add --all 
git commit -m "Upload toString() in class Person"
git push
```

Esto subirá los cambios que acabamos de realizar en nuestro repositorio !!



# Recursos adicionales:

[Creating a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

[¿Qué es y como se usa un repositorio?](https://teloexplicocongatitos.com/poster/tlecg04)

[GIT CHEAT SHEET](https://education.github.com/git-cheat-sheet-education.pdf)

[Hoja de referencia para Git de Github - GitHub Cheatsheets](https://training.github.com/downloads/es_ES/github-git-cheat-sheet/)

[Markdown Cheat Sheet | Markdown Guide](https://www.markdownguide.org/cheat-sheet/)

[Basic Syntax | Markdown Guide](https://www.markdownguide.org/basic-syntax)
