# Instalación y configuración de LaTeX en VS Code
## 1. Instalar VS Code

<img align="right" width="250" src="/.github/assets/readme/intro/LaTeX_Extension.png" alt="Extension" />

Sigue las instrucciones oficiales:  
[Instalar VS Code](https://code.visualstudio.com/docs/setup/setup-overview), elige el sistema operativo correspondiente.

## 2. Extensión LaTeX Workshop
Instálala desde VS Code:  
`Ctrl + Shift + X` -> busca **LaTeX Workshop** -> Instalar

## 3. Paquetes de LaTeX

> Intala los paquetes según el sistema operativo.


<details>
<summary> <b>Linux (Debian/Ubuntu)</b> </summary>

### Linux (Debian/Ubuntu)

Ejecuta en la terminal. VS Code también dispone de un [terminal integrado](/docs/vscode-related-tutorial/translation/vscode-tips.es.md#terminal):
```bash
sudo apt install texlive-full -y
```
</details>

<details>
<summary> <b>Windows</b> </summary>

### Windows
1. Descarga [**MiKTeX**](https://miktex.org/download) desde su página web oficial.  

2. Durante la instalación, activa **Install missing packages on-the-fly** para que, cuando falte un paquete, MiKTeX lo instale automáticamente.  
   
3. Reinicia VS Code.

</details>

<details>
<summary> <b>macOS</b> </summary>

### macOS
Instala **MacTeX**:
```
brew install --cask mactex
```

Si no tienes Homebrew: https://brew.sh/

</details>

<br>

[**(🔙README)**](/README.es.md#tabla-de-contenido)
