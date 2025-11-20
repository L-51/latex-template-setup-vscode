# Contributing Guidelines

Thank you for your interest in contributing!  
This project provides a **modular LaTeX template and a setup tutorial for Visual Studio Code (Linux)**.  
All contributions are welcome: improving the folder structure, enhancing documentation, fixing issues, or extending the tutorial.

---

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/fork.png" alt="fork the repository" />

## 1. Fork the repository
Click the **Fork** button in the upper-right corner of the page.  
This will create a copy of the repository under your GitHub account.

## 2. Clone your fork

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone the repository" />

You must clone **your fork**, not the main repository.  
Go to your GitHub account, open the forked repository, click **Code**, and copy the URL.  

Clone it using:
```bash
git clone https://github.com/<your-username>/latex-vscode-template.git
```
or  
```bash
  git clone git@github.com:L-51/latex-template-setup-vscode.git
```
Then change into the project directory:
```bash
cd latex-vscode-template
```

## 3. Create a new branch
Use a descriptive branch name.  
Modern Git recommends using switch:
```bash
  git switch -c new-branch
```
Common branch prefixes:
- `feature/` -> new features or enhancements
- `fix/` -> bug fixes
- `hotfix/` -> urgent fixes
- `docs/` -> documentation updates
For example:
```bash
  git switch -c feature/improve-structure
```

## 4. Make your changes
Modify the necessary files. Make sure:
- The template still compiles correctly
- The documentation remains consistent
- The project structure stays modular
You can check modified files with `git status`.

## 5. Commit your changes
Stage and commit:
<pre>
  git add .
  git commit -m "Describe your changes here"
</pre>
Please write clear and descriptive commit messages.

## 6. Push your branch
Push your branch to your fork:  
```bash
  git push origin new-branch
```

## 7. Open a Pull Request
Go to your fork on GitHub and click “Compare & pull request”.  
In your PR description, include:
- What you changed
- Why the change is useful
- Related issues (if applicable)  
Your contribution will be reviewed as soon as possible

# Code Style and Project Rules
Please respect the following guidelines:
- Keep the LaTeX folder structure modular
- Maintain compatibility with VS Code + LaTeX Workshop
- Write documentation in a clear and concise style
- For non-trivial changes, update **both English and Spanish READMEs**

# ❤️ Thank you!
Every contribution —big or small— helps improve this project.

[**(🔙README)**](/README.md)
