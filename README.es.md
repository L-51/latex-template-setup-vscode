# Configuración y plantilla modular de LaTeX en Visual Studio Code

<!--==Introducción==========================================================================================-->
## Introducción
Este tutorial te eseña como configurar paso a paso **Visual Studio Code** para usar LaTeX junto con una plantilla de **estructura modular** pensada para poder trabajar cómodamente, con:
- configuración automática
- compilación local (offline)
- organización del proyecto por carpetas
- compatibilidad completa con LaTeX Workshop
Ideal para estudiantes, docentes, investigadores o cualquier persona que quiera escribir en LaTeX desde VS Code de forma rápida y ordenada.

<!--==Tabla de contenido====================================================================================-->
## Tabla de contenido
- [Configuración y plantilla modular de LaTeX en Visual Studio Code](#configuración-y-plantilla-modular-de-latex-en-visual-studio-code)
  - [Introducción](#introducción)
  - [Tabla de contenido](#tabla-de-contenido)
  - [Inicio Rápido](#inicio-rápido)
  - [Instalación y configuración de LaTeX en VS Code (Linux)](#instalación-y-configuración-de-latex-en-vs-code-linux)
    - [1. Visual Studio Code instalado](#1-visual-studio-code-instalado)
    - [2. Extensión LaTeX Workshop](#2-extensión-latex-workshop)
    - [3. Paquetes de LaTeX en Linux](#3-paquetes-de-latex-en-linux)
  - [Estructura de la plantilla](#estructura-de-la-plantilla)
  - [Tips(Consejos)](#tipsconsejos)
  - [Conectar con el repositorio Git](#conectar-con-el-repositorio-git)
  - [Organización del proyecto (Hay texto de ejemplo en los ficheros)](#organización-del-proyecto-hay-texto-de-ejemplo-en-los-ficheros)
  - [⚠️Recomendación final:](#️recomendación-final)
  - [Colaboración](#colaboración)
  - [Recursos adicionales:](#recursos-adicionales)

<!--==Inicio Rápido=========================================================================================-->
## Inicio Rápido
Si quieres usar la plantilla de inmediato, sin leer todo el tutorial:
1. **Clona el repositorio**
   ```bash
     git clone https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE.git
   ```
   o con SSH:
   ```bash
     git clone git@github.com:L-51/Plantilla-LaTex-para-VSCode.git
   ```
2. Abre la carpeta en Visual Studio Code
3. Instala la extensión **LaTeX Workshop** (si no la tienes)
4. Abre `main.tex`
5. Pulsa `Ctrl + S` para compilar
6. Edita las secciones en `template/secciones/`
> Y... ¡Listo! Ya estás trabajando con la plantilla

<!--==Instalación y configuración de LaTeX en VS Code (Linux)===============================================-->
## Instalación y configuración de LaTeX en VS Code (Linux)
Ante de usar la plantilla, asegúrate de tener:
### 1. Visual Studio Code instalado
<p align="right" style="padding-right: 210px;">
  <img align="right" width="160" src="./.github/assets/LaTeX_Extension.png" alt="Extension" />
</p>

Sigue las instrucciones oficiales:
[Instalar VSC para Linux](https://code.visualstudio.com/docs/setup/linux)

### 2. Extensión LaTeX Workshop
Instálala desde VS Code:  
`Ctrl + Shift + X` -> busca LaTeX Workshop -> Instalar

### 3. Paquetes de LaTeX en Linux

<img align="right" src="./.github/assets/Terminal.png" alt="Terminal" width="250"/>

Ejecuta en la terminal:
```bash
sudo apt install texlive-full -y
```

Esto instala todo lo necesario para compilar localmente  

Se puede usar el atajo `Ctrl + '` para abrir el terminal o desde el icono interactivo:
  
<!--========================================================================================================-->
## Estructura de la plantilla
```bash
📁Plantilla-de-LaTeX-para-VSCode
├── 📄README.md
└── 📁template
    ├── 📁bibliografia
    │   └── 📚ref.bib
    ├── 📁config
    │   ├── ⚙️settings.tex
    │   └── 📄packages.tex
    ├── 📁ficheros
    ├── 📄.gitignore
    ├── 📁images
    │   └── 🖼️Example.png
    ├── 📄main.tex
    ├── 📁portadas
    │   └── 📄portada_ejemplo.tex
    └── 📁secciones
        ├── 📄ejercicio_1.tex
        ├── 📄ejercicio_2.tex
        └── 📄ejercicio_3.tex
```

<!--========================================================================================================-->
## Tips(Consejos)
- Al tener cuenta de estudiante, el **Copilot de Github** se puede usar gratuitamente.
  
  En caso de querer usarlo, instalar **Github Copilot** y **Github Copilot Chat** en el apartado de extensiones como previamente se indicó.
  
  Para conectar con su cuenta de estudiante, sería ir al apartado de su perfil -> `setting` -> `Emails` y añadir tu cuenta de estudiante
  
- `Ctrl + S` para guardar/compilar:
  <p align="left">
    <img src="./.github/assets/Ctrl%2BS.png" alt="Guardar/Compilar" width="250"/>
    <p><em>Guardar de manera interactiva</em></p>
  </p>

- `Ctrl + Alt + V` para visualizar:
  <p align="left">
    <img src="./.github/assets/Ctrl%2BAlt%2BV.png" alt="Visualizar" width="400"/>
    <p><em>Icono para visualizar</em></p>
  </p>

- Si tienes el `main.pdf` abierto para visualizar como previa mención, al guardar, se puedes ver los cambios reflejados en el pdf
  
- `Ctrl + Alt + X` le abrirá una ventana asociado al compilador de Latex y abajo izquierda con snippet
  <p>
    <img src="./.github/assets/Snippet.png" alt="Snippet" width="200"/>
    <p><em>Localización de las facilidades de LaTeX</em></p>
  </p>

- `Ctrl + I` para abrir **Copilot**(en caso de disposición de su extensión)
  <p>
    <img src="./.github/assets/Ctrl%2BI.png" alt="Inline chat" width="350"/>
    <p><em>Iniciar una interacción con el chatbot</em></p>
  </p>

- **(Comodidad visual)** Para una mejor visualización del entorno, abrimos configuración o en su defecto `Ctrl + ,`, escribir en la barra de búsqueda **rulers**, para posteriormente abrir **Edit in setting.json**, tras `"workbench.colorTheme": "Default Light Modern",` añadimos lo siguiente para que aparezca a la anchura de 80 caracteres un delimitador cual ajusta la anchura de texto de forma automática:
  <pre>
    "editor.rulers": [80],
    "editor.wordWrap": "wordWrapColumn",
    "editor.wordWrapColumn": 80,
  </pre>
     
  <p>
    <img src="./.github/assets/Ctrl%2B%2C.png" alt="Configuración" width="250"/>
    <p><em>Localización de configuración de manera interactiva</em></p>
  </p>
  <p>
    <img src="./.github/assets/Edit_setting_rulers.png" alt="Rulers" width="900"/> 
    <p><em>Resultado de búsqueda de "rulers"</em></p>
  </p>
  <p>
    <img src="./.github/assets/Settings_json.png" alt="settings.json" width="900"/>
    <p><em>settings.json tras introducir las reglas</em></p>
  </p>

- **(Opcional 1)** Para configurar la localización de los archivos de salida de compilación, pulse `Ctrl + ,` para abrir configuración y busque `Latex: Out Dir`, cambie la salida por una carpeta o una ruta donde quieras preservar los archivos. Una vez compilado el proyecto la salida se verá reflejado en dicha ruta(se usó [./build](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/build) de ejemplo). Para esta parte es recomendable que se use un fichero [`.gitignore`](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/blob/main/template/.gitignore) para que no se guarde archivos que no le interese en el repositorio. En comparación a **Opcional 2** como se indica abajo, hay una carpeta de más, pero a la hora de compilación es más **rápido** ya que mantiene los archivos de compilación, aunque ocupe más espacio
  <p>
    <img src="./.github/assets/Out_dir.png" alt="Out dir" width="1000"/>
    <p><em>Ejemplo de establecer la salida en <a href="https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/build">./build</a></em></p>
  </p>
  
- **(Opcional 2)** Si accedes a ajuste sea por icono o sea por `Ctrl + ,`, y busca `LaTex Auto Build Run` le aparecerá un apartado donde se podrá elegir la opción de compilación:
  - `never` compila solo cuando lanza el comando **Build LaTeX project** manualmente (`Ctrl+Alt+B` por defecto)
  - `onSave` compila solo cuando **guardas el archivo** (`Ctrl+S`), más recomendable para tener un mejor control de la compilación
  - `onFileChange` compila automáticamente cada vez que **detecta un cambio en el archivo** (aunque no lo guardes)
    
  Y al buscar `LaTex Auto Clean Run`, también dispone de opciones:
  - `onBuilt` limpia después de **cada compilación**
  - `onFailed` limpia solo si la **compilación falla**
  - `onSucceeded` limpia solo si **compilación fue exitosa**
  - `never` limpia solo cuando lanza el comando **LaTeX Workshop: Clean up auxiliary files** (lo puedes buscar con `Ctrl+Shift+P`)
<p>
  <img src="./.github/assets/autoBuild.png" alt="AutoBuild Run" width="750"/>
  <p><em>Resultado de la búsqueda</em></p>
</p>
<p>
  <img src="./.github/assets/autoClean.png" alt="AutoBuild Run" width="750"/>
  <p><em>Resultado de la búsqueda</em></p>
</p>
<p>
  <img src="./.github/assets/setting_json_alt.png" alt="AutoBuild Run" width="550"/>
  <p><em>settings.json tras elegir el modo</em></p>
</p>

  Además para poder eliminar todos los archivos de compilación manteniendo solo el `main.pdf`, habría que añadir parámetros en ajuste buscando `Clean: File Types` y en `Clean: Method` elegir la opción **glob** o en su efecto añadiendo al archivo `settings.json` buscando **rulers** como previo en **comodidad visual** del apartado [tips](#tipsconsejos) se indica, y añadir al final de ella:
  <pre>
    "latex-workshop.latex.autoBuild.run": "onSave",
    "latex-workshop.latex.autoClean.run": "onBuilt",
    "latex-workshop.latex.clean.fileTypes": [
        "*.aux",
        "*.bbl",
        "*.bcf",
        "*.blg",
        "*.idx",
        "*.ilg",
        "*.ind",
        "*.lof",
        "*.lot",
        "*.out",
        "*.toc",
        "*.acn",
        "*.acr",
        "*.alg",
        "*.glg",
        "*.glo",
        "*.gls",
        "*.fls",
        "*.log",
        "*.fdb_latexmk",
        "*.snm",
        "*.synctex(busy)",
        "*.synctex.gz(busy)",
        "*.nav",
        "*.vrb",
        "*.run.xml",
        "*.synctex.gz"
    ],
    "latex-workshop.latex.clean.method": "glob",
  </pre>
  <p><em>Con opción de onSave y onBuilt, eliminando todos los archivos de compilación</em></p>
  <p>
    <img src="././.github/assets/CleanFileTypes.png" alt="CleanFileTypes" width="450"/>
    <p><em>Resultado de búsqueda y añadir parámetros de forma interactiva</em></p>
  </p>
  <p>
    <img src="././.github/assets/CleanMethod.png" alt="CleanMethod" width="450"/>
    <p><em>Elegir el método de limpieza de forma interactiva</em></p>
  </p>
<!--========================================================================================================-->

## Conectar con el repositorio Git
1. Instalación de **Git**: si no lo tenían previamente instalado, `sudo apt install git -y`
2. Configurar tu usuario y correo:<br>
   `git config --global user.name "Tu Nombre"` <br>
   `git config --global user.email "tuemail@dominio.com"`
4. Accede a la carpeta donde quieras tener este proyecto guardado y clónalo escribiendo en la terminal de VSC y poner: <br>
   `git clone https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE` <br>
   O en su defecto descargarse el fichero zip [descargar](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/releases)
6. Abre la carpeta usando **Open Folder** de VSC o la carpeta que te interesa para realizar _click derecho_ -> _abrir con_ -> escribir **code** -> _Enter_
7. Para guardar los cambios en **Git** o para sincronizar con el repositorio vayase al apartado de **Source Control** o mediante atajo `Ctrl + Shift + G`, donde podrá realizar un **commit**, para recibir cambios del repositorio **pull**, o modificar el respositorio mediante **push**, en su defecto, a la hora de hacer **commit**, se puede desplegar a la derecha y emplear **Commit & Push** o **Commit & Pull**.
<p>
  <img src="./.github/assets/Source_Control.png" alt="Source Control" width="300"/>
</p>
<p>
  <img src="./.github/assets/Simbolo_pull.png" alt="Pull" width="350"/>
</p>
<p>
  <img src="./.github/assets/Simbolo_push.png" alt="Push" width="350"/>
</p>
<p>
  <img src="./.github/assets/Commit%26.png" alt="Commit &" width="400"/>
</p>
<!--========================================================================================================-->

## Organización del proyecto (Hay texto de ejemplo en los ficheros)
- [**bibliografia**](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/bibliografia) Aquí guardará las referencias en el fichero [ref.bib](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/blob/main/template/bibliografia/ref.bib)
- [**config**](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/config) Aquí están los [paquetes](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/config/packages.tex) que usarás y [setting](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/config/settings.tex) que se aplica de forma general al proyecto
- [**secciones**](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/secciones) Esta carpeta contendrá las distintas secciones que forman parte del trabajo
- [**images**](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/tree/main/template/images) Carpeta de las imágenes que se usarán para el proyecto
- [**portadas**](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/blob/main/template/portadas) Esta carpeta contiene las portadas del trabajo en formato LaTeX
- [**main.tex**](https://github.com/L-51/Plantilla-de-LaTex-para-Visual-Studio-Code-VSCODE/blob/main/template/main.tex) El main donde se incluirá todo, se indica al principio de esta `% !TeX root = main.tex
`
<!--========================================================================================================-->

---  
## ⚠️Recomendación final:
Si tienes poco manejo a la hora de usar GitHub para trabajar con varios usuarios y una mayor comodidad, se recomienda separar de forma explícita los ficheros donde trabajarán cada uno de ellos, y evitar en la medida de lo posible modificar ficheros no correspondido de forma accidental

---
<!--========================================================================================================-->
## Colaboración
¡Siempre son bienvenidas las contribuciones!
Si quieres colaborar, por favor sigue estos pasos:
1. Haz un **fork** del repositorio
2. Crea una nueva rama para tus cambios:
   ```bash
     git -checkout -b feature/nueva-funcion
   ```
   O para otros propósitos:
   - `feature/` -> para nuevas funciones o mejoras
   - `fix/` -> para correcciones de errores
   - `hotfix/` -> para parches urgentes
   - `docs` -> para cambios de documentación
3. Realiza tus modificaciones y haz commit:
   ```bash
     git commit -m "mensaje"
   ```
4. Sube tus cambios:
   ```bash
     git push origin feature/nueva-funcion
   ```
5. Abre un **Pull Request** para revisión

Puedes consultar el apartado de [**Recursos adicionales**](#recursos-adicionales) donde hay un tutorial

## Recursos adicionales:
- [Documentación de LaTeX Workshop](https://github.com/James-Yu/LaTeX-Workshop)
- [Manual sencillo de LaTex](https://manualdelatex.com/tutoriales)
- [Plantillas realizadas por LosDelGIIM](https://github.com/LosDelDGIIM/LosDelDGIIM.github.io/tree/main/subjects/_plantillas)
- [Tutorial para realizar un **pull request** en Github](https://github.blog/developer-skills/github/beginners-guide-to-github-creating-a-pull-request/)
- [Badges para readme](https://github.com/inttter/md-badges)
- [Generar y configurar SSH key para tu cuenta de GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
- [Cómo realizar tu primera contribución](https://github.com/firstcontributions/first-contributions)
- [Enlaces utiles sobre Git](https://github.com/firstcontributions/first-contributions/blob/main/docs/additional-material/git_workflow_scenarios/Useful-links-for-further-learning.md)
