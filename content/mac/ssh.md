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

### Copy files (scp)

    # remote -> local (download)
    scp -rp {username}@{remote}:{path} {localPath}
    
    # local -> remote (upload)
    scp -rp {localPath} {username}@{remote}:{path}
    
    # remote -> remote (external)
    scp -rp {username}@{remote}:{path} {username}@{remote}:{path}
    
    # -r means recursive
    # -p preserves modification times, access times, and modes from the original file
