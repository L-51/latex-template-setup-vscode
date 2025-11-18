# Advanced Tips
> Advanced configurations for users who want to go further

## Compilation Output Configuration
Go to settings and search for `Latex: Out Dir`, then change the output path where compilation files should be saved.

<img src="/.github/assets/readme/advanced/OutDir.png" alt="OutDir" width="370"/>

<img align="right" width="330" src="/.github/assets/readme/advanced/autoBuild.png" alt="Auto Build">

## autoBuild and autoClean
In settings, search for `LaTex Auto Build Run` and choose a compilation mode:
- `never`: compiles only when running **Build LaTeX project** manually (`Ctrl + Alt + B`)
- `onSave`: compiles only when you **save the file** (`Ctrl + S`), recommended for better control
- `onFileChange`: compiles automatically when it **detects any file change**

<img align="right" width="330" src="/.github/assets/readme/advanced/autoClean.png" alt="Auto Clean">

Then search for `LaTex Auto Clean Run`, and choose:
- `onBuilt`: cleans after **every compilation**
- `onFailed`: cleans only when compilation **fails**
- `onSucceeded`: cleans only when it **succeeds**
- `never`: cleans only when manually running **LaTeX Workshop: Clean up auxiliary files**

You can also add the following to [**settings.json**](/docs/vscode-related-tutorial/vscode-tips.md#visual-improvemente-80-columns-ruler):

<pre>
"latex-workshop.latex.autoBuild.run": "onSave",
"latex-workshop.latex.autoClean.run": "never",
</pre>

## Removing Auxiliary Files
To remove auxiliary compilation files while keeping only `main.pdf`, configure in settings → `Clean: File Types`.

<img width="400" src="/.github/assets/readme/advanced/cleanfileTypes.png">

Then in settings → `Clean: Method`, choose:
- `glob`: searches for files according to the patterns in `Clean: File Types`
- `command`: executes the command defined in `Clean: Command`

<img width="400" src="/.github/assets/readme/advanced/cleanMethod.png">

Example configuration:
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
> This improves **cleanliness**, but also increases **compilation time** and makes real-time [PDF preview](./vscode-tips.es.md#visualizar-pdf) slower, since LaTeX must regenerate all temporary files on each save.

## Creating Your Own Snippets

<img align="left" width="270" src="/.github/assets/readme/advanced/configure_Snippets.png">

Snippets are predefined code fragments that you can insert with a **shortcut or autocompletion**.  
To configure them: `Ctrl + Shift + P` → **Snippets: Configure Snippets** → select **local** or **global**.

<img width="400" src="/.github/assets/readme/advanced/snippets_file_option.png">

Example:
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

- `"prefix"`: what you type to trigger the snippet  
- `"body"`: content to insert  
- `$i`: placeholder position for the cursor (moving with Tab)
- `"description"`: optional description  

[**(🔙README)**](/README.en.md#table-of-contents)
