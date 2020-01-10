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

#### SSH Tunnel ####

    ssh -D 8123 -f -C -q -N {username}@{host}
    # System Preferences > Network > Advanced > Proxies > SOCKS Proxy
    # localhost : 8123
    
    ssh -L {remotePort}:localhost:{localPort} {username}@{host}
    # port tunneling
    

#### Copy files (scp) ####

    # remote -> local (download)
    scp -rp {username}@{host}:{path} {localPath}
    
    # local -> remote (upload)
    scp -rp {localPath} {username}@{host}:{path}
    
    # remote -> remote (external)
    scp -rp {username}@{host}:{path} {username}@{remote}:{path}
    
    # -r means recursive
    # -p preserves modification times, access times, and modes from the original file
