# Consejos avanzados
> Consejos y configuraciones más avanzadas para quienes quieran profundizar un poco más

## Configuración de salida de compilación
Ve a settings y escribe en la barra de búsqueda `Latex: Out Dir`, y cambia la ruta donde quieras guardar los archivos generados por la compilación:

<img src="/.github/assets/readme/advanced/OutDir.png" alt="OutDir" width="370"/>

<img align="right" width="330" src="/.github/assets/readme/advanced/autoBuild.png" alt="Auto Build">

## autoBuild y autoClean
Accediendo a settings, y buscar `LaTex Auto Build Run` le aparecerá un apartado donde se podrá elegir la opción de compilación:
  - `never`: compila solo al ejecutar el comando **Build LaTeX project** (`Ctrl+Alt+B`)
  - `onSave`: compila **al guardar el archivo** (`Ctrl+S`)
  - `onFileChange`: compila cada vez que **detecta un cambio**, aunque no guardes

<img align="right" width="330" src="/.github/assets/readme/advanced/autoClean.png" alt="Auto Clean">

Y al buscar `LaTex Auto Clean Run`, dispondrás de opciones como:
  - `onBuilt`: limpia después de **cada compilación**
  - `onFailed`: limpia solo si la **compilación falla**
  - `onSucceeded`: limpia solo si la **compilación fue exitosa**
  - `never`: limpia solo al ejecutar **LaTeX Workshop: Clean up auxiliary files** (lo puedes buscar con `Ctrl+Shift+P`)

También se puede configurar manualmente en [**settings.json**](/docs/vscode-related-tutorial/translation/vscode-tips.es.md#mejora-visual-reglas-en-80-columnas):

<pre>
"latex-workshop.latex.autoBuild.run": "onSave",
"latex-workshop.latex.autoClean.run": "never",
</pre>

## Eliminar archivos auxiliares
Para mantener solo `main.pdf`, ve a settings -> `Clean: File Types` y define qué archivos se deben borrar.

<img width="400" src="/.github/assets/readme/advanced/cleanfileTypes.png">

Luego en settings -> `Clean: Method` puedes elegir:
- `glob`: busca y elimina archivos según los patrones de `Clean: File Types`
- `command`: elimina según lo definido en `Clean: Command`

<img width="400" src="/.github/assets/readme/advanced/cleanMethod.png">

Ejemplo de configuración completa:
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

> [!NOTE]
> Ten en cuenta que, a cambio de **limpieza**, obtienes la **desventaja de tiempo**: al guardar, debe **recompilarse todo** desde cero, lo que ralentiza la previsualización.

## Creación de Snippets propios

<img align="left" width="270" src="/.github/assets/readme/advanced/configure_Snippets.png">

Los snippets son fragmentos de código predefinidos que puedes **insertar con un atajo o autocompletado**.  
Para configurarlos: `Ctrl + Shift + P` -> **Snippets: Configure Snippets** -> elige **local o global**.

<img width="400" src="/.github/assets/readme/advanced/snippets_file_option.png">

Ejemplo de snippet:
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
- `"prefix"`: lo que escribes para activar el snippet
- `"body"`: contenido insertado
- `$i`: posición del cursor tras insertar (se avanza con Tab)  
- `"description"` descripción opcional

[**(🔙README)**](/README.es.md#tabla-de-contenido)