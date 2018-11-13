[back to table of content](../../readme.md)

# Brew snippets #
Setup and frequently used snippets

#### Installation ####

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

#### Default packages ####

    brew install composer
    brew install node
    brew install mysql@5.7
    
    #optional
    brew install php72
    brew install php72-xdebug

#### Linking packages ####

    brew link <package>
    brew unlink <package>

#### Services ####

    brew services start mysql@5.7
    brew services stop mysql@5.7

#### Package location ####

    /usr/local/Cellar

#### Specific version

    brew install <package>@<version>
