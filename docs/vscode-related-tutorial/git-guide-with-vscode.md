# Connecting with Git and GitHub
> Basic tutorial for configuring and using Git with the VS Code GUI

## 1. Install **Git**

<details>
<summary><b>Linux (Debian/Ubuntu)</b></summary>

### Linux (Debian/Ubuntu)
From the terminal:
```
sudo apt install git -y
```
</details>

<details>
<summary><b>Windows</b></summary>

### Windows
Install following the [official guide](https://git-scm.com/install/windows).  
It is recommended to keep the default option:  
`Git from the command line and also from 3rd-party software`  
to work with _PowerShell_ or _CMD_.

</details>

<details>
<summary><b>macOS</b></summary>

### macOS
Follow the instructions in the [official tutorial](https://git-scm.com/install/mac).

</details>

## 2. Clone the repository
```
git clone https://github.com/L-51/latex-template-setup-vscode.git
```
Or using **SSH**:
```
git clone git@github.com:L-51/latex-template-setup-vscode.git
```
Or download the zip [**template.zip**](https://github.com/L-51/latex-template-setup-vscode/releases) from the **Releases** page and extract it.

## 3. Open the folder
Using _File_ → **Open Folder** in VS Code,  
or right-click the **template folder** → _Open with…_ → select **VS Code**,  
or via terminal:
```
cd latex-template-setup-vscode
code template
```

<img align="right" width="250" src="/.github/assets/readme/git/Source_Control.png" alt="Source_Control" />

## 4. Using Source Control
To initialize a **Git** repository or connect to a **remote repository**, you can use the terminal following this [GitHub tutorial](https://docs.github.com/es/get-started/git-basics/about-remote-repositories),  
or use VS Code’s GUI tool: **Source Control**, accessible via the shortcut `Ctrl + Shift + G` or from the left panel.

<img align="left" width="300" src="/.github/assets/readme/git/Pull_Push_Combined.png" alt="Pull_Push_Combined" />

Once the repository is initialized, you can make **commits** from Source Control.  
For a remote repository, use **pull** (receive changes) and **push** (send changes).  
When committing, you can expand the dropdown and use **Commit & Push** or **Commit & Pull**.

Although all commands can still be used traditionally via the terminal, VS Code provides a GUI that simplifies these tasks.

<br>

[**(🔙README)**](/README.es.md#tabla-de-contenido)
