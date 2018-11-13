[back to table of content](../../readme.md)

# SSH snippets #
Setup and frequently used snippets

#### Installation ####

    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

#### Use brew over local ####

    nano ~/.zshrc

    # Always let /usr/local/bin overwrite binaries. This is where brew creates symlinks.
    export PATH="$PATH:/usr/local/bin"