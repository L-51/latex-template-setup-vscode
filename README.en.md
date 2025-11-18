# LaTeX Modular Template and Configuration in Visual Studio Code

## Introduction
This tutorial teaches you how to configure **Visual Studio Code** step by step to use LaTeX together with a **modular structure template**, designed to work comfortably with:
- **Automatic** configuration
- **Local (offline)** compilation
- **Modular** project organization by folders
- Full compatibility with **LaTeX Workshop**

Ideal for **students, teachers, researchers, or anyone** who wants to write LaTeX from VS Code in a clean and organized way.

<!--==Table of content======================================================================================-->
## Table of Contents
- [LaTeX Modular Template and Configuration in Visual Studio Code](#latex-modular-template-and-configuration-in-visual-studio-code)
  - [Introduction](#introduction)
  - [Table of Contents](#table-of-contents)
  - [Prerequisite](#prerequisite)
  - [Quick Start](#quick-start)
  - [Template Structure](#template-structure)
      - [**bibliography**](#bibliography)
      - [**build**](#build)
      - [**config**](#config)
      - [**files**](#files)
      - [**images**](#images)
      - [**main.tex**](#maintex)
      - [**sections**](#sections)
      - [**title\_pages**](#title_pages)
      - [**.gitignore**](#gitignore)
  - [Next Steps](#next-steps)
    - [Additional Material](#additional-material)

<!--==Prerequisite==========================================================================================-->
## Prerequisite
- Have **Visual Studio Code** installed  
- Have the **LaTeX Workshop** extension by *James Yu* installed  
- Have the required **LaTeX packages** installed  

> [!NOTE]  
> If you are missing any requirement, click [here](/docs/vscode-related-tutorial/setup.md).

<!--==Quick Start===========================================================================================-->
## Quick Start
1. **Clone the repository** using `git` ([**Git guide**](/docs/vscode-related-tutorial/git-guide-with-vscode.md)),  
   or download the zip [**template.zip**](https://github.com/L-51/Plantilla-LaTex-para-VSCode/releases)
2. Open the folder in **Visual Studio Code**
3. Install the **LaTeX Workshop** extension (if you haven’t already)
4. Open `main.tex` to locate the main file
5. Press `Ctrl + S` to compile
6. Edit the different sections in `template/secciones/`

> And… Done! You are now working with the template.

<!--==Template structure====================================================================================-->
## Template Structure
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
> Folder that stores references and bibliographies in the file [ref.bib](/template/bibliografia/ref.bib).

#### [**build**](/template/build/)
> Folder for compilation output files. Recommended for keeping things clean. To configure it, click [here](/docs/vscode-related-tutorial/translation/advanced.es.md#compilation-output-configuration).

#### [**config**](/template/config/)
> Contains the [packages](/template/config/packages.tex) used in *packages.tex* and the [settings](/template/config/settings.tex) in *settings.tex*, which apply globally to the project.

#### [**files**](/template/files/)
> Folder where any type of file used in the project is stored.

#### [**images**](/template/images/)
> Folder containing the images used in the project.

#### [**main.tex**](/template/main.tex)
> The main file where everything is included. Declared at the top with `% !TeX root = main.tex`. This is the file that compiles and resolves dependencies.

#### [**sections**](/template/sections/)
> This folder contains the different sections that make up the project for better organization.

#### [**title_pages**](/template/title_pages/)
> This folder contains the title pages of the work.

#### [**.gitignore**](/template/.gitignore)
> A `.gitignore` file is included to exclude files from version control. This version ignores compilation files if you configured **build** as the output directory and keeps only **main.pdf**. In the [Git resource list](/docs/additional-material/additional-material.md#useful-links-about-git), a tutorial on this topic is included.

<!--==Next Steps============================================================================================-->
## Next Steps
> [!TIP]  
> If you want to learn and start using **Git** and explore the GUI tools offered by **VS Code**, I recommend this [**Git guide with VS Code**](./docs/vscode-related-tutorial/translation/git-guide-with-vscode.md).

> [!TIP]  
> If you want to learn **basic shortcuts and settings** to speed up using LaTeX in VS Code, check this [**basic configuration and shortcuts document**](./docs/vscode-related-tutorial/translation/vscode-tips.md).

> [!TIP]  
> If you want to go deeper into **configuration** and manage LaTeX more professionally, I suggest this [**advanced tips guide**](./docs/vscode-related-tutorial/translation/advanced.md).

### [Additional Material](/docs/additional-material/additional-material.md)

