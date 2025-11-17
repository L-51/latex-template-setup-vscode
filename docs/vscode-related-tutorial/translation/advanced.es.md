# Consejos avanzados
> Consejos y configuraciones más avanzadas para aquellos que quieren profundizar un poco más
## Configuración de salida de compilación
Vaya a settings y escriba en la barra de búsqueda `Latex: Out Dir`, y cambie la ruta de salida donde quieras guardar archivos cuales son resultados de la compilación:

<img src="/.github/assets/readme/advanced/OutDir.png" alt="OutDir" width="370"/>

<img align="right" width="330" src="/.github/assets/readme/advanced/autoBuild.png" alt="Auto Build">

## autoBuild y autoClean
Accediendo a settings, y buscar `LaTex Auto Build Run` le aparecerá un apartado donde se podrá elegir la opción de compilación:
  - `never` compila solo cuando lanza el comando **Build LaTeX project** manualmente (`Ctrl+Alt+B` por defecto)
  - `onSave` compila solo cuando **guardas el archivo** (`Ctrl+S`), más recomendable para tener un mejor control de la compilación
  - `onFileChange` compila automáticamente cada vez que **detecta un cambio en el archivo** (aunque no lo guardes)

<img align="right" width="330" src="/.github/assets/readme/advanced/autoClean.png" alt="Auto Clean">

Y al buscar `LaTex Auto Clean Run`, también dispone de opciones:
  - `onBuilt` limpia después de **cada compilación**
  - `onFailed` limpia solo si la **compilación falla**
  - `onSucceeded` limpia solo si **compilación fue exitosa**
  - `never` limpia solo cuando lanza el comando **LaTeX Workshop: Clean up auxiliary files** (lo puedes buscar con `Ctrl+Shift+P`)

O se puede añadir manualmente al final de [**settings.json**](/docs/vscode-related-tutorial/translation/vscode-tips.es.md#mejora-visual-reglas-en-80-columnas) las siguientes líneas:
<pre>
"latex-workshop.latex.autoBuild.run": "onSave",
"latex-workshop.latex.autoClean.run": "never",
</pre>
Siendo en este ejemplo, la opción `onSave` para autoBuild y `never` para autoClean.

## Eliminar archivos auxiliares
Para eliminar los archivos auxiliares de compilación manteniendo solo el `main.pdf`, hay que indicar que tipo de archivos se debe borrar en el apartado de settings -> `Clean: File Types`.

<img width="400" src="/.github/assets/readme/advanced/cleanfileTypes.png">

Posteriormente en settings -> `Clean: Method` se presenta varias opciones:
- `glob` busca los archivos en todas las carpetas siguiendo patrones definido en `Clean: File Types`
- `command` borra según lo que se definió en `Clean: Command`  

<img width="400" src="/.github/assets/readme/advanced/cleanMethod.png">

En nuestro caso, elegimos la opción **glob** o en su efecto añadiendo al archivo [**settings.json**](./vscode-tips.es.md#mejora-visual-reglas-en-80-columnas) añadir al final de ella.  
Esto es un ejemplo de una configuración donde se borraría todos los archivos temporales menos el `main.pdf`:
<pre>
"latex-workshop.latex.autoBuild.run": "onSave",
"latex-workshop.latex.autoClean.run": "onBuilt",
"latex-workshop.latex.clean.fileTypes": [
    "*.aux",
    "*.bbl",
    "*.bcf",
    "*.blg",
    "*.idx",
    "*.ilg",
    "*.ind",
    "*.lof",
    "*.lot",
    "*.out",
    "*.toc",
    "*.acn",
    "*.acr",
    "*.alg",
    "*.glg",
    "*.glo",
    "*.gls",
    "*.fls",
    "*.log",
    "*.fdb_latexmk",
    "*.snm",
    "*.synctex(busy)",
    "*.synctex.gz(busy)",
    "*.nav",
    "*.vrb",
    "*.run.xml",
    "*.synctex.gz"
],
"latex-workshop.latex.clean.method": "glob",
</pre>
Aunque es interesante destacar que, a cambio de **limpieza**, obtiene una **inconveniencia de tiempo** y [visualizar](./vscode-tips.es.md#visualizar-pdf) en tiempo real más tardado, ya que en cada guardado se tendría que **compilar** todo de nuevo y generar de vuelta todos los archivos temporales

## Creación de Snippets propios

<img align="left" width="270" src="/.github/assets/readme/advanced/configure_Snippets.png">

Son fragmentos de código predefinidos que puedes **insertar con un atajo o completado automático**.  
Puedes crear tus propios _snippets_ personalizados para escribir LaTeX más rápido.  
En VS Code para configurarlos: `Ctrl + Shift + P` -> Snippets: Configure Snippets -> Eliges **local o global**
<img width="400" src="/.github/assets/readme/advanced/snippets_file_option.png">

Un ejemplo de snippet sería:
<pre>
{
  "Theorem and Proof": {
    "prefix": "theoremproof",
    "body": [
      "\\begin{theorem}",
      "    ${1:Statement of the theorem}",
      "\\end{theorem}",
      "",
      "\\begin{proof}",
      "    ${2:Proof of the theorem}",
      "\\end{proof}"
    ],
    "description": "Snippet for theorem and proof in LaTeX"
  }
}
</pre>
- `"prefix"` lo que escribes para activar el snippet
- `"body"` el contenido que se inserta
- `$i`, *i: número*,  indica dónde estará el cursor después de insertar, y se desplaza tabulando
- `"description"` descripción opcional

[**(🔙README)**](/README.es.md#requisito-previo)