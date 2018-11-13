[back to table of content](../../readme.md)

# Git snippets #
Setup and frequently used snippets

#### Global user ####

    git config --global user.name "Thomas Zandvliet"
    
    git config --global user.email "info@thomasmedia.nl"

#### Global .gitignore ####

    touch ~/.gitignore
    
    git config --global core.excludesfile ~/.gitignore

[global gitignore](global-gitignore.md)

#### Reload .gitignore ####

    git -rm -r --cached .

    git add .

    git commit -m ".gitignore is now working"

[source](https://stackoverflow.com/questions/1139762/ignore-files-that-have-already-been-committed-to-a-git-repository)

#### Git clone ####

    # branch and folder are optional
    git clone -b <branch> <source> <into-folder>

#### Rebase ####

    # make sure both branches are up-to-date
    # start in feature/branch
    git rebase master feature/branch
    
    # dependency
    git rebase feature/dependency feature/branch

[source](https://git-scm.com/docs/git-rebase)