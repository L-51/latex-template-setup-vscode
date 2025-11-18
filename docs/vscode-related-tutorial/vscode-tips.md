# Basic Tips
> Tips and shortcuts for VS Code when working on a LaTeX project

## Compile/Save
```
Ctrl + S
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Save.png" alt="Save" width="250"/><br>
<em>Via GUI button</em>

</td>
</tr>
</table>

## View PDF
```
Ctrl + Alt + V
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Visualise.png" alt="Visualise" width="220"/><br>
<em>Via GUI button</em>

</td>
</tr>
</table>

If you have **main.pdf** open in the viewer, saving will automatically refresh the PDF with the latest changes.

## Terminal
```
Ctrl + `
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Terminal.png" alt="Terminal" width="300"/><br>
<em>Via GUI button</em>

</td>
</tr>
</table> 

## LaTeX Snippets and Utilities
```
Ctrl + Alt + X
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Snippet_and_Utility.png" alt="Snippet_and_Utility" width="300"/><br>
<em>Via GUI button</em>

</td>
</tr>
</table> 


## Copilot (in case of its availability)
```
Ctrl + I
``` 
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Inline_chat_Copilot.png" alt="Inline_chat_Copilot" width="300"/><br>
<em>Right click and choose</em>

</td>
</tr>
</table>

## Settings
```
Ctrl + ,
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Settings.png" alt="Settings" width="300"/><br>
<em>Settings via GUI</em>

</td>
</tr>
</table>

## Visual improvemente (80-columns ruler)


Open [settings](#settings), search for **rulers**:
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Rulers_search.png" alt="Rulers_search" width="300"/><br>
<em>Resultado de la búsqueda</em>

</td>
</tr>
</table>

select **Edit in settings.json**. Add the following:
<pre>
  "editor.rulers": [80],
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 80,
</pre>

Example `settings.json`:
<pre>
{
  "workbench.colorTheme": "Default Light Modern",
  "editor.rulers": [80],
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 80,
}
</pre>

## Extra Tip: Free Copilot for Students
If you have a student account, **GitHub Copilot** is free.  

Install **GitHub Copilot** and **GitHub Copilot Chat** from the extensions panel.  

To link your student account, go to your GitHub profile → `Settings` → `Emails` and add your student email.

## ⚠️ Working Collaboratively
> [!WARNING]
> If you are inexperienced with GitHub when working with multiple contributors, it is strongly recommended to **explicitly separate files** each person will work on, and **avoid modifying files assigned to others** to prevent accidental conflicts.


[**(🔙README)**](/README.en.md#prerequisite)
