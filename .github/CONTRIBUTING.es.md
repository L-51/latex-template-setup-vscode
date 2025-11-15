# Pautas para contribución
¡Agradezco por su interés en contribuir!  
Este proyecto ofrece una **plantilla modular y un tutorial de configuración de LaTex para Visual Studio Code**.  
Las contribuciones son bienvenidas, mejora de la estructura de la plantilla, añadir documentación, arreglar problemas, o mejorar el tutorial.  

---

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/fork.png" alt="fork the repository" />

## 1. Haz un fork del repositorio
Crea un fork del repositorio, dandole al botón que se encuentra en la zona superior izquierda de la página. Esto creará una copia del repositorio en tu cuenta

## 2. Clona el repositorio bifurcado(forked)
<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone the repository" />
Clonas el repositorio que hiciste *fork*, no el repositorio main.  
Ve a tu cuenta de GitHub, localiza el repositorio, pulsa el **botón de code** y luego en la parte de copiar el url, ahora ya puedes clonar el repositorio, se te presenta varias opciones, para `https` es necesario haber configurado el usuario y contraseña:
<pre>
  git config --global user.name "Tu Nombre"
  git config --global user.email "tuemail@dominio.com"
</pre>
Si es para la opción `ssh` aquí le dejo un [tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) por parte de GitHub.
```bash
  git clone https://github.com/<your-username>/latex-vscode-template.git
```
Para navegar y acceder al respositorio clonado, simplementes realice el siguiente comando:
```bash
  cd latex-vscode-template
```

## 3. Crea una nueva rama(branch)
Ahora crea una nueva rama usando el comando `branch` y cambiarte a ella con `switch`, o, directamente realizando ambos pasos en uno con la opción `-b` con `switch`:
<pre>
  git branch nueva-rama
  git switch nueva-rama
</pre>
Alternativamente:
<pre>
  git switch -c nueva-rama
</pre>
Es recomendable usar prefijos para aclarar el propósito de la nueva rama:
- `feature/` -> para nuevas funciones o mejoras
- `fix/` -> para correcciones de errores
- `hotfix/` -> para parches urgentes
- `docs` -> para cambios de documentación
Por ejemplo:
```bash
  git switch -c feature/mejorar-estructura
```
## 4. Realizas los cambios
Modifica los archivos necesarios.  
Asegurando que:
- La plantilla sigue compilando correctamente
- La documentación permanece consistente
- La nueva estructura sigue siendo modular
Puedes verificar que efectivamente hubo cambios escribiendo `git status`.

## 5. Confirma(commit) esos cambios
Añade los cambios y realizas un commit:
<pre>
  git add .
  git commit -m "Mensaje de commit"
</pre>

## 6. Sube(push) los cambios a GitHub
Realiza un push de tu rama al repositorio bifurcado:
`git push origin nueva-rama`

## 7. Envía(submit) los cambios para ser revisados
Si ahora va al repositorio bifurcado de GitHub, aparecerá un botón de `Compare & pull request`. Haz click en el botón.  
Añade en la descripción de `pull request` lo siguiente:
- Los nuevos cambios realizados
- La utilidad de los cambios
- Problemas relacionados(Si es aplicable)
La contribución será revisado lo más pronto posible

# Estilo del código y reglas del proyecto
Respecte las siguientes normas para la contribución:
- Mantener una estructura modular para LaTex
- Mantener el proyecto compatible con **VS Code**
- Escribir la documentación de forma clara y un estilo conciso
- Para cambios no triviales, actualiza en **ambas** versiones de README, Inglés y Español
# ❤️ ¡Gracias!
Cualquier contribución sea grande o pequeñas mejorará este proyecto
