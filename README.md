#### **Enunciado:**
Eres nuevo en la empresa y te han dicho que tienes que encargarte de un proyecto que recién acaba de llegar. 
Tu tarea es crear y administrar el repositorio siguiendo las instrucciones que te ha dado un compañero:


### **Parte 1: Preparación del Proyecto**
1. **Crear directorios y archivos:**  
   - Desde tu carpeta principal (`~/`), crea un directorio llamado `GitApellido1Nombre2425`.
      -  _mkdir GitTamurejoSara2024_ (Crear carpeta)
      - _pwd_ (Saber carpeta donde estoy)
      -  _mkdir GitTamurejoSara2024/src (Crear nueva carpeta en GitTamurejoSara2024)

   - Dentro del directorio `GitApellido1Nombre2425`, crea una subcarpeta llamada `src` usando rutas relativas.
  ![1 1](https://github.com/user-attachments/assets/4d33bcc1-023d-40c6-be5b-9b3aebb9793b)

   - Crea un archivo `README.md` en `GitApellido1Nombre2425` con una breve descripción del proyecto, **usa costantemente el terminal**.
       -  _cat > README.md_ (Crear archivo)
       -  _cat README.md (Ver contenido del archivo README.md)_
       -  _ls_ (Ver el contenido del directorio)
    ![1 2](https://github.com/user-attachments/assets/f86b070c-5c7d-4de4-abc2-5be30ac6105a)
    ![1 3](https://github.com/user-attachments/assets/1f29664a-adf5-4f50-858d-f64349224c5b)


2. **Inicializa Git:**  
   - Entra en el directorio y conviértelo en un repositorio Git.
       - _cd GitTamurejoSara2024_ (Moverme a la carpeta GitTamurejoSara2024)
       - _git init ._ (Inciar repositorio Git)
    ![2 1](https://github.com/user-attachments/assets/8c61ee90-2355-4f2b-9581-3a301d5f7770)

   - Agrega un archivo `.gitignore` y configúralo para ignorar [archivos de log y carpetas de configuración temporales.](https://www.atlassian.com/es/git/tutorials/saving-changes/gitignore)
       - _cat > .gitignore_ (Crear archivo .gitignore)
       - _nano .gitignore_ (Editar el archivo .gitignore)
       - _cat .gitignore_ (Ver contenido del archivo .gitignore)
    ![2 2](https://github.com/user-attachments/assets/0b0ef7ec-4724-45bd-b42b-2b7b8372f296)
    ![2 3](https://github.com/user-attachments/assets/fc4f0c50-26ce-495c-abbf-a14249602111)

   - ¿Qué es el archivo `.gitignore` y para que sirve?
       - Es un archivo que se configura para especificar que directorios o archivos serán ignorados por el control de versiones.
         
   - Crea una estructura básica de web `index.html`, `style.css`, `main.js`.
       - _cat > index.html_ (Crear archivo index.html)
       - _cat > style.css_ (Crear archivo style.css)
       - _cat > main.js_ (Crear archivo main.js)
       - _ls_ (Mirar contenido de GitTamurejoSara2024)
         ![2 4](https://github.com/user-attachments/assets/bd263d50-bb92-4daf-a94e-e35ddef7a14b)
         ![2 5](https://github.com/user-attachments/assets/167fd8ba-8711-48a4-9b40-447f53ca877c)

3. **Primera confirmación:**  
   - Haz un `git add` de todos los archivos y realiza un commit inicial con el mensaje:  
     `Inicio del proyecto con README.md y estructura básica`.
       - _git add *_ (Añadir todos los archivos para que tengan control de versiones)
       - _git status_ (Ver status)
       - _git commit -m "Inicio del proyecto con README.md y estructura basica"_ (Hacer un commit con un mensaje)
![3 1](https://github.com/user-attachments/assets/863cc8c8-5181-457e-a989-1a3ca7ed66b0)
![3 2](https://github.com/user-attachments/assets/f262f457-5653-43da-9a4f-6c145ed6cd71)

---

### **Parte 2: Colaboración en Equipo**
1. **Configura del repositorio remoto:**  
   - Entra en GitHub y crea un repositorio.
   - ¿Qué pasa si creo un repositorio con el archivo `README.md` desde GitHub?
       - El repositorio que se ha creado no estará vacio y se verá el contenido del READ.me en la primera página.
     ![4 1](https://github.com/user-attachments/assets/f5f1fd4d-341f-40bd-9a18-6570e3d2055a)

   - ¿Qué pasa si crea un repositorio sin el archivo `README.md` desde GitHub?
       - Está vacio y te pone algunas comandas que puedes usar para empezar un repositorio y añadir cosas.
    ![4 2](https://github.com/user-attachments/assets/55383a32-d1bb-4f4d-95ae-610ee13e28ee)
   - Explica las diferencias entre las 2 preguntas anteriores.
       - En la primera opción tendrá solo el archivo README.md y el la segunda estará vacio pero te saldrán comandos para iniciar un repositorio y añadir cosas.
   - Indica que comandos te da GitHub al crear un repositorio. Los encontrarás en el apartado `…or create a new repository on the command line
`
![4 3](https://github.com/user-attachments/assets/a685204e-50b0-4eee-ab9e-be98d82b6d71)

   - Vincula el repositorio remoto con el repositorio local.
       - _git remote add GitTamurejoSara2425 https://github.com/SaraTamurejoMora/GitTamurejoSara2425.git_  (Enlazar el repositorio local con el remoto)
       - _git push GitTamurejoSara2425 master_ (Hacer push del contenido de GitTamurejoSara2425 en la rama master)
         ![4 4](https://github.com/user-attachments/assets/8ba1d2a0-87fc-427f-a16e-c649d32f1fbf)
         ![4 5](https://github.com/user-attachments/assets/d59ce2e0-5cc5-43e8-9f24-d97dabdc1c89)

     - Comprovar que se han subido al repositorio remoto los archivos
![4 6](https://github.com/user-attachments/assets/3e9ceb1c-9b95-49a2-812d-13f0c04b077a)

      - Token para poder enlazar el repositorio.
![4 7](https://github.com/user-attachments/assets/5d0ba6e0-f84f-467c-a37b-1418ec32eb8f)


2. **Actualización del Proyecto:**
   - Crea una nueva rama llamada `feature/documentacion` y cámbiate a ella.
       - _git checkout master_ (Cambiar a rama master)
       - _git branch feature/documentacion_ (Crear rama feature/documentacion)
       - _git checkout feature/documentacion_ (Cambiar a rama feature/documentacion)
         ![5 1](https://github.com/user-attachments/assets/5089c7bf-f7db-478d-95cd-9fc0128faacd)

   - Cambia a la nueva rama:
     - Crea un archivo `docs.md` en la carpeta raíz. Escribe un resumen de las funcionalidades del proyecto.
         - _nano docs.md_ (Crear y editar archivo docs.md)
         - _cat docs.md_ (Ver contenido de docs.md)
           ![5 2](https://github.com/user-attachments/assets/65ac02ae-5323-4e6b-b63f-082b83e322d0)

     - Haz un commit con el mensaje:  
       `Agregada documentación inicial del proyecto`.
         -  _git add docs.md_ (Añadir docs.md para que se haga control de versiones)
         -  _git comit -m "Agregada documentación inicial del proyecto"_ (Hacer commit con mensaje)
           ![5 3](https://github.com/user-attachments/assets/8cfe014e-ebf0-4d15-99fd-192563e7e36e)

   - Cambia a la rama `main` y usa `git diff` para comparar las diferencias entre `main` y `feature/documentacion`.
       - _git diff master..feature/documentacion_ (Comparar las dos ramas)
![6 1](https://github.com/user-attachments/assets/bc6c4c44-ca59-480c-88b3-7c398c36d4a8)

3. **Sincronización:**  
   - Desde la rama `main`, realiza un `git pull` para simular la descarga de cambios del remoto. Si hay conflictos, resuélvelos.
      -__
---

### **Parte 3: Gestión de Archivos y Cambios**
1. **Ediciones rápidas:**  
   - Crea un nuevo archivo llamado `src/app.py` con un mensaje básico (`print("Hola, mundo!")`).
       - _cat > src/app.py_ (Crear archivo)
       - _cat src/app.py_ (Ver el contenido)
      ![7 1](https://github.com/user-attachments/assets/574b807d-7d21-47c9-a28a-67ac26acd9c0)

   - Haz un `add` y luego un `commit`. Verifica su estado con ` status` o con algún comando alias que hayas creado tú.
        - _git add src/app.py_ (Añadir para que se haga control de versiones)
        - _git commit -m "Crear archivo app.py"_ (Hacer commit con comentario)
          ![7 2](https://github.com/user-attachments/assets/f3ef1b8e-3b8a-410f-930e-94427701919b)

   - Visualiza el historial de `commit` con `log` o con algún comando alias que hayas creado tú.
       - _git log_ (Ver el historial)
     ![7 3](https://github.com/user-attachments/assets/b39e87b6-4a15-43a2-af46-d9994d95b826)

   - Si has utilizado comandos alias, indica el equivalente al comando alias. Por ejemplo, mi comando alias `git s` es igual al comando `git status --short`.

2. **Borrado y recuperación:**  
   - Borra el archivo `src/app.py` usando un comando de terminal. Recupera el archivo con el comando necesario, lo vimos la semana pasada.
     - _rm src/app.py_ (Borrar el archivo app.py)
     - _git checkout HEAD src/app.py_ (Comanda para recuperar el archivo)
     - _ls src/_ (Ver si el archivo se ha recuperado)
     ![8 1](https://github.com/user-attachments/assets/c5f2c4da-f11a-4f08-9ae4-a4be372e6d18)

3. **Combina ramas:**  
   - Desde `main`, haz un merge de `feature/documentacion`.
         - _git checkout master_ (Cambiar a la rama master)
         - _git merge feature/documentacion_ (Combinar ramas)
     ![9 1](https://github.com/user-attachments/assets/d8d65fe4-805d-46d0-b2b8-59874a1f80e2)
![9 2](https://github.com/user-attachments/assets/659f4bfb-73b8-4909-866f-517d193221af)

   - Usa `log` o un alias para verificar los cambios realizados y el historial.
       - _git log_ (Ver el historial y los cambios)
     ![9 3](https://github.com/user-attachments/assets/b86674fd-c059-4fc9-ba3a-1cc8fe441c23)

---

### **Parte 4: Entrega del Proyecto**
1. **Últimos pasos:**  
   - Asegúrate de que todos los archivos estén en su lugar y realiza un `push` final al remoto.
       - _git checkout master_ (Cambiar a rama master)
       - _git push GitTamurejoSara master_ (Hacer push de GitTamurejoSara2425 en la rama master)
     ![10 1](https://github.com/user-attachments/assets/a10bd2fc-8816-40e0-9f02-4e2c23a76fb3)

   - Realiza una limpieza eliminando la rama `feature/documentacion`.
       - _git branch -d feature/documentacion -f_ (Eliminar la rama feature/documentacion)
     ![10 2](https://github.com/user-attachments/assets/7f2fd97e-57d5-4c6d-bb1f-db3012ffeb0d)

2. **Explora el proyecto desde el terminal:**  
   - Usa el comando necesario de Linux para listar el contenido de cada directorio.
       - _ls_ (Listar contenido)
       - _ls src/_ (Listar contenido src/)
     ![11 1](https://github.com/user-attachments/assets/156fa17d-1826-43a5-a029-8428a862b7c8)

   - Muestra el contenido de los archivos finales con el comando necesario de Linux.
     - _cat docs.md_ (Ver contenido)
     - _cat index.html_ (Ver contenido)
     - _cat main.js_ (Ver contenido)
     - _cat README.md_ (Ver contenido)
     - _cat styles.css_ (Ver contenido)
     - _cat src/app.py_ (Ver contenido)
![11 2](https://github.com/user-attachments/assets/0201a4d9-cdb6-4a0f-83e2-2715fe6f8735)

     
       
