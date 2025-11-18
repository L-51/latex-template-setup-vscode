# Configuración y plantilla modular de LaTeX en Visual Studio Code

<!--==Introducción==========================================================================================-->
## Introducción
Este tutorial te enseña cómo configurar paso a paso **Visual Studio Code** para usar LaTeX junto con una plantilla de **estructura modular** pensada para poder trabajar cómodamente, con:
- configuración **automática**
- compilación **local (offline)**
- organización **modular** del proyecto por carpetas
- compatibilidad completa con **LaTeX Workshop**

Ideal para **estudiantes, docentes, investigadores o cualquier persona** que quiera escribir en LaTeX desde VS Code de forma rápida y ordenada.


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
      - [**files**](#files)
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
> [!NOTE]
> En caso de faltar algún requisito, pulse [aquí](/docs/vscode-related-tutorial/translation/setup.es.md).

<!--==Inicio Rápido=========================================================================================-->
## Inicio Rápido
1. **Clona el repositorio** con `git`([**guía sobre Git**](./docs/vscode-related-tutorial/translation/git-guide-with-vscode.es.md)), 
   o descarga el zip [**template.zip**](https://github.com/L-51/Plantilla-LaTex-para-VSCode/releases)
2. Abre la carpeta en **Visual Studio Code**
3. Instala la extensión **LaTeX Workshop** (si no la tienes)
4. Abre `main.tex` para localizar el main
5. `Ctrl + S` para compilar
6. Editar las diferentes secciones en `template/sections/`
> Y... ¡Listo! Ya estás trabajando con la plantilla
  
<!--==Estructura de la plantilla============================================================================-->
## Estructura de la plantilla
<pre>
📁template
├── 📁bibliography
│   └── 📚ref.bib
├── 📁config
│   ├── 📄packages.tex
│   └── ⚙️settings.tex
├── 📁files
│   └── 📄example.cpp
├── 📄.gitignore
├── 📁images
│   └── 🖼️Example.png
├── 📄main.tex
├── 📁sections
│   ├── 📄section_1.tex
│   ├── 📄section_2.tex
│   └── 📄section_3.tex
└── 📁title_pages
    └── 📄example_title_page.tex
</pre>

#### [**bibliography**](/template/bibliography/)
> Carpeta que guarda las referencias y bibliografías en el fichero [ref.bib](/template/bibliografia/ref.bib).

#### [**build**](/template/build/)
> Carpeta para ficheros de salida de la compilación. Recomendable para una mayor limpieza. Para establecerla pulse [aquí](/docs/vscode-related-tutorial/translation/advanced.es.md#configuración-de-salida-de-compilación).

#### [**config**](/template/config/)
> Aquí están los [paquetes](/template/config/packages.tex) que usarás en _packages.tex_ y las [configuraciones](/template/config/settings.tex) en _settings.tex_ que se aplican de forma general al proyecto.

#### [**files**](/template/files/)
> Carpeta donde se guarda cualquier tipo de fichero que se vaya usando durante el proyecto.

#### [**images**](/template/images/)
> Carpeta de las imágenes que se usarán para el proyecto.

#### [**main.tex**](/template/main.tex)
> El main donde se incluirá todo. Se indica al principio con `% !TeX root = main.tex`. Es el archivo donde se compilará y se resolverán las dependencias.

#### [**sections**](/template/sections/)
> Carpeta que contiene las distintas secciones que forman parte del trabajo, para una mejor organización.

#### [**title_pages**](/template/title_pages/)
> Carpeta que contiene las portadas del trabajo.

#### [**.gitignore**](/template/.gitignore)
> Se incluye un archivo `.gitignore` para no incluir archivos innecesarios en control de versiones. En este caso es una versión simple para omitir los ficheros de compilación en caso de haber configurado como salida **build** y mantener solo **main.pdf**.  
> En la [recopilación de enlaces sobre Git](/docs/additional-material/additional-material.es.md#enlaces-útiles-sobre-git) se incluye un tutorial sobre esto.


<!--==Siguientes pasos======================================================================================-->
## Siguientes pasos
> [!TIP]
> Si quieres aprender y empezar a usar **Git** y conocer las herramientas _GUI_ que ofrece **VS Code**, te recomiendo que mires esta [**guía sobre Git con VS Code**](/docs/vscode-related-tutorial/translation/git-guide-with-vscode.es.md).

> [!TIP]
> Si quieres conocer **atajos y consejos básicos** para agilizar y facilitar el uso de LaTeX en VS Code, mira este [**documento de configuraciones y atajos**](/docs/vscode-related-tutorial/translation/vscode-tips.es.md).

> [!TIP]
> Si quieres profundizar más sobre **configuraciones** y controlar LaTeX de forma más profesional, te sugiero mirar estos [**consejos avanzados**](/docs/vscode-related-tutorial/translation/advanced.es.md).


<!--==Material adicional====================================================================================-->
### [Material adicionales](/docs/additional-material/additional-material.es.md)
