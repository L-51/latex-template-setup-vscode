# Installing and Configuring LaTeX in VS Code
## 1. Install VS Code

<img align="right" width="250" src="/.github/assets/readme/intro/LaTeX_Extension.png" alt="Extension" />

Follow the official instructions:  
[Instalar VS Code](https://code.visualstudio.com/docs/setup/setup-overview), choosing your operating system.

## 2. LaTeX Workshop Extension
Install it from VS Code:  
`Ctrl + Shift + X` -> search for **LaTeX Workshop** -> Install

## 3. LaTeX Packages

> Install LaTeX packages depending on your operating system.


<details>
<summary> <b>Linux (Debian/Ubuntu)</b> </summary>

### Linux (Debian/Ubuntu)

Run this in the terminal. VS Code also provide an [integrated terminal](/docs/vscode-related-tutorial/translation/vscode-tips.md#terminal):
```bash
sudo apt install texlive-full -y
```
</details>

<details>
<summary> <b>Windows</b> </summary>

### Windows
1. Download [**MiKTeX**](https://miktex.org/download) from the official website.  

2. Dering installing, enable **Install missing packages on-the-fly** so MiKTeX installs missing LaTeX packages automatically when needed.  
   
3. Restart VS Code afterwards.

</details>

<details>
<summary> <b>macOS</b> </summary>

### macOS
Install **MacTeX**:
```
brew install --cask mactex
```

If you don't have Homebrew: https://brew.sh/

</details>

<br>

[**(🔙README)**](/README.en.md#table-of-contents)
