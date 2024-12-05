### **Actividad: Remoto y repaso de comandos anteriores**

**¿De qué trata?** 
Hay que practicar la sincronización y administración de un repositorio Git, manejar ramas, resolver diferencias (diff) e interactuar entre repositorios locales y remotos.

**IMPORTANTE**
- Quiero capturas del terminal donde se muestre el comando
- Quiero que escribas el comando en el ejercicio
- Quiero que expliques que estás haciendo
- **IMPORTANTE**: Vas a documentar todo el proyecto en un README.md dentro de la actividad. Vas a escribirlo en [Markdown](https://github.com/VelezBeatriz/ITB-M08-DAW1/blob/main/Markdown.md)
---

#### **Enunciado:**

Eres nuevo en la empresa y te han dicho que tienes que encargarte de un proyecto que recién acaba de llegar. 
Tu tarea es crear y administrar el repositorio siguiendo las instrucciones que te ha dado un compañero:


### **Parte 1: Preparación del Proyecto**
1. **Crear directorios y archivos:**  
   - Desde tu carpeta principal (`~/`), crea un directorio llamado `GitApellido1Nombre2425`.  
   - Dentro del directorio `GitApellido1Nombre2425`, crea una subcarpeta llamada `src` usando rutas relativas.
   - Crea un archivo `README.md` en `GitApellido1Nombre2425` con una breve descripción del proyecto, **usa costantemente el terminal**.
   
![Captura de pantalla de 2024-11-28 08-49-42](https://github.com/user-attachments/assets/a1cb09bf-a1d9-491a-b7a1-eb04ab72b763)

2. **Inicializa Git:**  
   - Entra en el directorio y conviértelo en un repositorio Git.
   - Agrega un archivo `.gitignore` y configúralo para ignorar [archivos de log y carpetas de configuración temporales.](https://www.atlassian.com/es/git/tutorials/saving-changes/gitignore)
  
![Captura de pantalla de 2024-11-28 09-07-31](https://github.com/user-attachments/assets/427225b4-ab50-4928-9492-7f72e873da4d)


   - ¿Qué es el archivo `.gitignore` y para que sirve?

       - El archivo `.gitignore` es un archivo de texto que sirve para evitar que archivos no deseados, como configuraciones           locales, archivos temporales o de log, se incluyan en el repositorio.
     
   - Crea una estructura básica de web `index.html`, `style.css`, `main.js`.

![capM08](https://github.com/user-attachments/assets/8fa017c7-cca0-4c35-b675-678a7067b75a)

2. **Primera confirmación:**  
   - Haz un `git add` de todos los archivos y realiza un commit inicial con el mensaje:  
     `Inicio del proyecto con README.md y estructura básica`.
     
![capm082](https://github.com/user-attachments/assets/594edbd0-9368-4e8c-9fb0-e8e5284cdbcf)

---

### **Parte 2: Colaboración en Equipo**
1. **Configura del repositorio remoto:**  
   - Entra en GitHub y crea un repositorio.
   - ¿Qué pasa si creo un repositorio con el archivo `README.md` desde GitHub?

        - Ocurre que se crea automáticamente el README en el repositorio.

   - ¿Qué pasa si crea un repositorio sin el archivo `README.md` desde GitHub?
  
       - Que se crea vacío el repositorio
         
   - Explica las diferencias entre las 2 preguntas anteriores.
  
       - En la primera si ponemos un README, el repositorio no se crea vacío, en cambio en el segundo si.
   
   - Indica que comandos te da GitHub al crear un repositorio. Los encontrarás en el apartado `…or create a new repository on the command line`
     
       - echo  "# nombre-del-repositorio" >> README.md
       - git add .
       - git commit -m "primer commit"
       - git remote add origin https://github.com/tu-usuario/nombre-del-repositorio.git
       - git branch -M main
       - git push -u origin main
       - git remote add origin https://github.com/tu-usuario/nombre-del-repositorio.git
      
   - Vincula el repositorio remoto con el repositorio local.
     
![Captura de pantalla de 2024-12-05 08-33-49](https://github.com/user-attachments/assets/4c4c7b9b-1066-4654-bedd-ef56486ea05f)

2. **Actualización del Proyecto:**
   - Crea una nueva rama llamada `feature/documentacion` y cámbiate a ella.
   - Cambia a la nueva rama:
     - Crea un archivo `docs.md` en la carpeta raíz. Escribe un resumen de las funcionalidades del proyecto.
     - Haz un commit con el mensaje:  
       `Agregada documentación inicial del proyecto`.
   - Cambia a la rama `main` y usa `git diff` para comparar las diferencias entre `main` y `feature/documentacion`.

![Captura de pantalla de 2024-12-05 08-44-19](https://github.com/user-attachments/assets/0519d510-9587-4a57-a6ed-3e60060b3011)


3. **Sincronización:**  
   - Desde la rama `main`, realiza un `git pull` para simular la descarga de cambios del remoto. Si hay conflictos, resuélvelos.
   - 
![Captura de pantalla de 2024-12-05 08-49-17](https://github.com/user-attachments/assets/5e6eddc9-07d0-4586-94a2-8d003a03a813)

---

### **Parte 3: Gestión de Archivos y Cambios**
1. **Ediciones rápidas:**  
   - Crea un nuevo archivo llamado `src/app.py` con un mensaje básico (`print("Hola, mundo!")`).
   - Haz un `add` y luego un `commit`. Verifica su estado con ` status` o con algún comando alias que hayas creado tú.

![Captura de pantalla de 2024-12-05 09-01-10](https://github.com/user-attachments/assets/9d428d07-b938-4310-adcf-14222795745b)
 
   - Visualiza el historial de `commit` con `log` o con algún comando alias que hayas creado tú.

![Captura de pantalla de 2024-12-05 09-01-51](https://github.com/user-attachments/assets/38f353ad-a5e8-49c1-9de2-60b8cd93f17b)

   - Si has utilizado comandos alias, indica el equivalente al comando alias. Por ejemplo, mi comando alias `git s` es igual al comando `git status --short`.

2. **Borrado y recuperación:**  
   - Borra el archivo `src/app.py` usando un comando de terminal. Recupera el archivo con el comando necesario, lo vimos la semana pasada.
     
     ![Captura de pantalla de 2024-12-05 09-09-08](https://github.com/user-attachments/assets/6dc4dd3a-7963-4c12-8913-08df49ba394e)
     
![Captura de pantalla de 2024-12-05 09-07-57](https://github.com/user-attachments/assets/27464c05-8cc5-4764-818a-b4b1f0fe7f8e)
  
3. **Combina ramas:**  
   - Desde `main`, haz un merge de `feature/documentacion`.  
   - Usa `log` o un alias para verificar los cambios realizados y el historial.
     
![Captura de pantalla de 2024-12-05 08-59-02](https://github.com/user-attachments/assets/a269a1bd-2f7d-40d1-bcb7-1beaed1e42c3)

![Captura de pantalla de 2024-12-05 09-11-14](https://github.com/user-attachments/assets/a9786098-b4f4-4214-8218-e1cc40701a52)

---

### **Parte 4: Entrega del Proyecto**
1. **Últimos pasos:**  
   - Asegúrate de que todos los archivos estén en su lugar y realiza un `push` final al remoto.  
   - Realiza una limpieza eliminando la rama `feature/documentacion`.

2. **Explora el proyecto desde el terminal:**  
   - Usa el comando necesario de Linux para listar el contenido de cada directorio.
     
       - `esta parte no me funcionaba, pero lo he hecho junto a mi compañero`
         
![CAP13](https://github.com/user-attachments/assets/a7a3a025-2925-45e7-855b-61a01f532ec2)

   - Muestra el contenido de los archivos finales con el comando necesario de Linux.

      - `esta parte no me funcionaba, pero lo he hecho junto a mi compañero`

![CAP14](https://github.com/user-attachments/assets/db4a7364-9bac-4670-8da8-b3ca6246cf59)
