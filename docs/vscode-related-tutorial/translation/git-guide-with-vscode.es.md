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
Instala según la [guía oficial](https://git-scm.com/install/windows) de Git.  
Se recomienda mantener la opción por defecto de `Git from the command line and also from 3rd-party software` para poder trabajar con la terminal de _PowerShell_ o _CMD_

</details>

<details>
<summary> <b>macOS</b> </summary>

### macOS
Seguir las instrucciones del [tutorial oficial](https://git-scm.com/install/mac) de Git.

</details>

## 2. Clona el repositorio
```
git clone https://github.com/L-51/Plantilla-LaTex-para-VSCode.git
```
O con **SSH**
```
git clone git@github.com:L-51/Plantilla-LaTex-para-VSCode.git
```
O descarga el zip [**template.zip**](https://github.com/L-51/Plantilla-LaTex-para-VSCode/releases) en **release** y posteriormente lo descomprime.
## 3. Accede a la carpeta 
Usando _File_ -> **Open Folder** de VSC o _click derecho_ sobre la **carpeta template** -> _abrir con_ -> buscar **VS Code** -> _Enter_, o vía terminal(si dispone) con:
<pre>
cd Plantilla-LaTex-para-VSCode
code template
</pre>

<img align="right" width="250" src="/.github/assets/readme/git/Source_Control.png" alt="Source_Control" />

## 4. Utilización de Source Control
Para inicializar un repositorio con **Git** o un **respositorio remoto**, se puede hacer vía terminal como lo indica este [tutorial](https://docs.github.com/es/get-started/git-basics/about-remote-repositories) de GitHub, o, mediante VS Code cual te ofrece una herramienta GUI, **Source Control**, se puede acceder mediante atajo `Ctrl + Shift + G`, o desde el explorador situado a la izquierda.

<img align="left" width="300" src="/.github/assets/readme/git/Pull_Push_Combined.png" alt="Pull_Push_Combined" />

Donde una vez iniciado el repositorio se podrá realizar **commit** utilizando el **Source Control**.  
Para repositorio remoto, **pull**(recibir cambios del remoto) y **push**(enviar cambios al remoto), a la hora de hacer **commit**, se puede desplegar a la derecha y emplear **Commit & Push** o **Commit & Pull**.  
Aunque aún se puede reliazar todos estos comandos a lo tradicional via terminal, VS Code ofrece una herramienta que facilita esta tarea.

[**(🔙README)**](/README.es.md#tabla-de-contenido)