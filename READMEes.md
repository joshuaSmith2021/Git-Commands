Git Commands
============

## Translated Versions
- [English Version](README.md) (Original)
- [Versão em português](READMEpt.md)

___

_Una lista de mis comandos mas usados_

*Si usted está interesado en mis aliases de Git, mire mi `.bash_profile`, encontrado acá: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Getting & Creating Projects

| Comando | Descripción |
| ------- | ----------- |
| `git init` | Inicialice un repositorio Git local |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Cree una copia local de un repositorio remoto |

### Basic Snapshotting

| Comando | Descripción |
| ------- | ----------- |
| `git status` | Compruebe estado |
| `git add [file-name.txt]` | Añada un archivo al área de ensayo |
| `git add -A` | Agregue todos los archivos nuevos y modificados al área de preparación |
| `git commit -m "[commit message]"` | Cometa cambios |
| `git rm -r [file-name.txt]` | Elimine un archivo (o carpeta) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
