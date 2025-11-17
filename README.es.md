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
  - [Requisito previo](#requisito-previo)
  - [Inicio Rápido](#inicio-rápido)
  - [Estructura de la plantilla](#estructura-de-la-plantilla)
      - [**bibliography**](#bibliography)
      - [**build**](#build)
      - [**config**](#config)
      - [**images**](#images)
      - [**main.tex**](#maintex)
      - [**sections**](#sections)
      - [**title\_pages**](#title_pages)
      - [**.gitignore**](#gitignore)
  - [Siguientes pasos](#siguientes-pasos)
    - [Material adicionales](#material-adicionales)

<!--==Requisito previo======================================================================================-->
## Requisito previo
- Tener instalado **Visual Studio Code**
- Tener instalado la extensión de **LaTeX Workshop** de _James Yu_
- Tener instalado los **paquetes** de LaTeX

En caso de faltar algún requisito, pulse [aquí](/docs/vscode-related-tutorial/translation/setup.es.md).
<!--==Inicio Rápido=========================================================================================-->
## Inicio Rápido
1. **Clona el repositorio**
   ```bash
     git clone https://github.com/L-51/Plantilla-LaTex-para-VSCode.git
   ```
   o con **SSH**:
   ```bash
     git clone git@github.com:L-51/Plantilla-LaTex-para-VSCode.git
   ```
2. Abre la carpeta en **Visual Studio Code**
3. Instala la extensión **LaTeX Workshop** (si no la tienes)
4. Abre `main.tex` para localizar el main
5. `Ctrl + S` para compilar
6. Editar las diferentes secciones en `template/secciones/`
> Y... ¡Listo! Ya estás trabajando con la plantilla
  
<!--==Estructura de la plantilla============================================================================-->
## Estructura de la plantilla
<pre>
📁template
├── 📁bibliografia
│   └── 📚ref.bib
├── 📁config
│   ├── ⚙️settings.tex
│   └── 📄packages.tex
├── 📁files
│   └── 📄example.cpp
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
</pre>

#### [**bibliography**](./template/bibliography/)
> Aquí guardará las referencias y bibliografías en el fichero [ref.bib](./template/bibliografia/ref.bib).
#### [**build**](./template/build/)
> Carpeta para ficheros salida de la compilación, recomendable para una mayor limpieza, para establecerlo pinchar [aquí](./docs/vscode-related-tutorial/translation/advanced.es.md#configuración-de-salida-de-compilación).
#### [**config**](./template/config/)
>  Aquí están los [paquetes](./template/config/packages.tex) que usarás en _package.tex_ y [configuraciones](./template/config/settings.tex) en _settings.tex_ que se aplica de forma general al proyecto.
#### [**images**](./template/images/)
> Carpeta de las imágenes que se usarán para el proyecto.
#### [**main.tex**](./template/main.tex)
> El main donde se incluirá todo, se indica al principio de esta `% !TeX root = main.tex`, y es el archivo donde se compilará y se resolverá las dependencias, etc.
#### [**sections**](./template/sections/)
> Esta carpeta contendrá las distintas secciones que forman parte del trabajo, para una mejor organización.
#### [**title_pages**](./template/title_pages/)
> Esta carpeta contiene las portadas del trabajo.
#### [**.gitignore**](/template/.gitignore)
> Se incluye un archivo `.gitignore` para no incluir archivos en control de versiones, en este caso es una versión simple para obviar los ficheros de compilación en caso de haber configurado como salida **build** y mantener solo **main.pdf**, en [recopilación de enlaces sobre Git](/docs/additional-material/additional-material.es.md#enlaces-útiles-sobre-git) incluye un tutorial sobre esto.

<!--==Siguientes pasos======================================================================================-->
## Siguientes pasos
- Si quieres aprender y empezar a usar **Git** y conocer sobre las herramientas _GUI_ que ofrece **VS Code**, te recomiendo que mires esta [**guía sobre Git con VS Code**](./docs/vscode-related-tutorial/translation/git-guide-with-vscode.es.md)
- Si quieres saber unos **atajos y consejos básicos**, mira este [**documento**](./docs/vscode-related-tutorial/translation/vscode-tips.es.md) para agilizar y facilitar el uso de LaTeX en VS Code
- Posteriormente si aún quieres profundizar más sobre **configuraciones** y controlar de forma más profesional LaTeX, te sugiero mirar estos [consejos avanzados](./docs/vscode-related-tutorial/translation/advanced.es.md).

<!--==Material adicional====================================================================================-->
### [Material adicionales](./docs/additional-material/additional-material.es.md)
