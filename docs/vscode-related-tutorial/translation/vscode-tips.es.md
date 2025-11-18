# Consejos básicos
> Consejos y atajos para VS Code a la hora de hacer un proyecto en LaTeX

## Compilar/Guardar
```
Ctrl + S
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Save.png" alt="Save" width="250"/><br>
<em>Vía botón GUI</em>

</td>
</tr>
</table>

## Visualizar PDF
```
Ctrl + Alt + V
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Visualise.png" alt="Visualise" width="220"/><br>
<em>Vía botón GUI</em>

</td>
</tr>
</table>

Si tienes el **main.pdf** abierto para visualizar, al guardar se pueden ver los cambios reflejados en el visor.

## Terminal
```
Ctrl + `
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Terminal.png" alt="Terminal" width="300"/><br>
<em>Vía botón GUI</em>

</td>
</tr>
</table> 

## Snippets y utilidades de LaTeX
```
Ctrl + Alt + X
```
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Snippet_and_Utility.png" alt="Snippet_and_Utility" width="300"/><br>
<em>Vía botón GUI</em>

</td>
</tr>
</table> 


## Copilot (en caso de su disposición)
```
Ctrl + I
``` 
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Inline_chat_Copilot.png" alt="Inline_chat_Copilot" width="300"/><br>
<em>Botón derecho y seleccionar vía GUI</em>

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
<em>Ajuste vía GUI</em>

</td>
</tr>
</table>

## Mejora visual (reglas en 80 columnas)


Vamos a [settings](#settings), escribimos en la barra de búsqueda **rulers**:
<table>
<tr>
<td align="center">

<img src="/.github/assets/readme/basic/Rulers_search.png" alt="Rulers_search" width="300"/><br>
<em>Resultado de la búsqueda</em>

</td>
</tr>
</table>

Pulsamos **Edit in settings.json** y añadimos lo siguiente para que aparezca un delimitador a la anchura de 80 caracteres:
<pre>
  "editor.rulers": [80],
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 80,
</pre>

Por ejemplo, un `settings.json` completo sería:
<pre>
{
  "workbench.colorTheme": "Default Light Modern",
  "editor.rulers": [80],
  "editor.wordWrap": "wordWrapColumn",
  "editor.wordWrapColumn": 80,
}
</pre>

## Consejo extra: Copilot gratuito para estudiantes
Si tienes cuenta de estudiante, el **Copilot de GitHub** se puede usar gratuitamente.  

Para activarlo, instala **GitHub Copilot** y **GitHub Copilot Chat**.  

Después ve a tu perfil -> `Settings` -> `Emails` y añade tu correo de estudiante.

## ⚠️ Trabajando de forma cooperativo
> [!WARNING]
> Si tienes **poco** manejo usando GitHub con varios usuarios, para mayor comodidad se recomienda **separar explícitamente los archivos** donde trabajará cada uno y **evitar modificar archivos ajenos** de forma accidental.


[**(🔙README)**](/README.es.md#requisito-previo)
