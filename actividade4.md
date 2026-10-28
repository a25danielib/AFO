
### Pregunta 1
**¿Qué diferencia existe entre el repositorio local de tu ordenador y el repositorio remoto que acabas de crear?**  
El repositorio local está guardado en tu ordenador y funciona sin conexión a Internet; el remoto está alojado en los servidores de GitHub en la nube para hacer copias de seguridad y compartir el proyecto.

---

### Pregunta 2
**¿Qué representa `origin` en Git?**  
Es el alias o nombre por defecto que utiliza Git para referirse a la URL del repositorio remoto.

---

### Pregunta 3
**¿Qué función realiza el comando `git push`?**  
Envía los *commits* y cambios registrados en el repositorio local hacia el repositorio remoto en GitHub.

---

### Pregunta 4
**¿Por qué es necesario ejecutar `git push` después de realizar un commit local?**  
Porque el `commit` solo guarda la versión en tu equipo; `git push` la sube a la nube para que esté disponible y actualizada en GitHub.

---

### Pregunta 5
**¿Qué diferencia existe entre `git push` y `git pull`?**  
* `git push`: Sube los cambios del local al remoto.  
* `git pull`: Descarga e integra los cambios del remoto al local.

---

### Pregunta 6
**¿Qué diferencia existe entre clonar un repositorio con `git clone` y descargar sus archivos como ZIP desde GitHub?**  
`git clone` descarga el proyecto con todo su historial y la carpeta `.git` para seguir usando comandos de Git; la descarga en ZIP solo obtiene los archivos estáticos sin el historial de versiones.