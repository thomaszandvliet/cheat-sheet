[back to table of content](../../readme.md)

# SSH snippets #
Setup and frequently used snippets

#### Generating new keys ####

    cd ~/.ssh
    
    ssh-keygen -t rsa -b 4096 -C "<username>"
        - <filename>
        - <passphrase>
    
    ssh-add -K ~/.ssh/<filename>
    
    cat <filename>.pub

Add to [GitHub](https://github.com/settings/keys)