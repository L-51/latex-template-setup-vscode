# Conectar con Git y GitHub
> Tutorial básico para configurar y usar Git aprovechando la herramienta GUI de VS Code

## 1. Instalación de **Git**
<details>
<summary> <b>Linux (Debian/Ubuntu)</b> </summary>

### Linux (Debian/Ubuntu)
Desde la terminal:
```
sudo apt install git -y
```
</details>

<details>
<summary> <b>Windows</b> </summary>

### Windows
Instala siguiendo la [guía oficial](https://git-scm.com/install/windows) de Git.  
Se recomienda mantener la opción por defecto `Git from the command line and also from 3rd-party software` para poder trabajar con la terminal de _PowerShell_ o _CMD_.

</details>

<details>
<summary> <b>macOS</b> </summary>

### macOS
Sigue las instrucciones del [tutorial oficial](https://git-scm.com/install/mac) de Git.

</details>

## 2. Clona el repositorio
```
git clone https://github.com/L-51/Plantilla-LaTex-para-VSCode.git
```
O con **SSH**
```
git clone git@github.com:L-51/Plantilla-LaTex-para-VSCode.git
```
O descarga el zip [**template.zip**](https://github.com/L-51/Plantilla-LaTex-para-VSCode/releases) en **Release** y descomprímelo.

## 3. Accede a la carpeta 
Usando _File_ -> **Open Folder** de VSC,  
o _clic derecho_ sobre la **carpeta template** -> _abrir con_ -> **VS Code**,  
o vía terminal (si dispones de ella):

<pre>
cd Plantilla-LaTex-para-VSCode
code template
</pre>

<img align="right" width="250" src="/.github/assets/readme/git/Source_Control.png" alt="Source_Control" />

## 4. Utilización de Source Control
Para inicializar un repositorio con **Git** o un **repositorio remoto**, puedes hacerlo vía terminal como indica este [tutorial](https://docs.github.com/es/get-started/git-basics/about-remote-repositories),  
o mediante la herramienta GUI de VS Code: **Source Control** (`Ctrl + Shift + G`).

<img align="left" width="300" src="/.github/assets/readme/git/Pull_Push_Combined.png" alt="Pull_Push_Combined" />

Una vez iniciado el repositorio, podrás realizar **commits** desde **Source Control**.  
Para repositorios remotos se pueden hacer **pull** (recibir cambios) y **push** (enviar cambios).  
También se puede usar **Commit & Push** o **Commit & Pull**.  
Aunque aún puedes realizar todas estas acciones desde terminal, VS Code ofrece una herramienta que facilita estas tareas.

<br>

[**(🔙README)**](/README.es.md#tabla-de-contenido)
