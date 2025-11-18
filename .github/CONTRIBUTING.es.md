# Pautas para contribución

¡Agradezco por su interés en contribuir!  
Este proyecto ofrece una **plantilla modular y un tutorial de configuración de LaTex para Visual Studio Code**.  
Las contribuciones son bienvenidas, mejora de la estructura de la plantilla, añadir documentación, arreglar problemas, o mejorar el tutorial.  

---

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/fork.png" alt="fork the repository" />

## 1. Haz un fork del repositorio
Crea un fork del repositorio, dándole al botón que se encuentra en la zona superior izquierda de la página.   
Esto creará una copia del repositorio en tu cuenta

## 2. Clona el repositorio bifurcado(forked)

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone the repository" />

Clonas el repositorio que hiciste *fork*, no el repositorio main.  
Ve a tu cuenta de GitHub, localiza el repositorio, pulsa el **botón de code** y copia el url.  

Para clone escribe lo siguiente:
```bash
  git clone https://github.com/<your-username>/latex-vscode-template.git
```
o  
```bash
  git clone git@github.com:L-51/latex-template-vscode.git
```
Para navegar y acceder al repositorio clonado:
```bash
  cd latex-vscode-template
```

## 3. Crea una nueva rama(branch)
Usa un nombre descriptivo para la rama.  
Git moderno recomenda `switch` para crear nuevas ramas:
<pre>
  git switch -c nueva-rama
</pre>
Prefijos comunes para las ramas:
- `feature/` -> para nuevas funciones o mejoras
- `fix/` -> para correcciones de errores
- `hotfix/` -> para parches urgentes
- `docs/` -> para cambios de documentación
Por ejemplo:
```bash
  git switch -c feature/mejorar-estructura
```
## 4. Realiza los cambios
Modifica los archivos necesarios.  
Asegurando que:
- La plantilla sigue compilando correctamente
- La documentación permanece consistente
- La nueva estructura sigue siendo modular
Puedes verificar que efectivamente hubo cambios con `git status`.

## 5. Confirma(commit) esos cambios
Añade los cambios y realizas un commit:
<pre>
  git add .
  git commit -m "Describe los cambios aquí"
</pre>
Escribir un mensaje que sea claro y descriptivo.

## 6. Sube(push) los cambios a GitHub
Realiza un push de tu rama al repositorio bifurcado:  
```bash
  git push origin nueva-rama
```

## 7. Envía(submit) los cambios para ser revisados
Ve al repositorio bifurcado de GitHub, y pulsa el botón de **"Compare & pull request"**.  
Añade en la descripción de `pull request` lo siguiente:
- Los nuevos cambios realizados
- La utilidad de los cambios
- Problemas relacionados(Si es aplicable)
La contribución será revisado lo más pronto posible

# Estilo del código y reglas del proyecto
Respeta las siguientes normas para la contribución:
- Mantener una estructura **modular** para LaTex
- Mantener el proyecto compatible con **VS Code**
- Escribir la documentación de forma clara y un estilo conciso
- Para cambios no triviales, actualiza en **ambas versiones de README, Inglés y Español**

# ❤️ ¡Gracias!
Cualquier contribución sea grande o pequeña mejorará este proyecto.

[**(🔙README)**](/README.md)