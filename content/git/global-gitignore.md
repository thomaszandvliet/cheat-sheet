[back to table of content](../../readme.md) |
[git snippets](git-snippets.md)

# Global gitignore #

    ### General Development ###
    /vendor/
    node_modules/
    npm-debug.log
    yarn-error.log
    .env



    ### macOS ###
    # General
    .DS_Store
    .AppleDouble
    .LSOverride

    # Thumbnails
    ._*

    # Files that might appear in the root of a volume
    .DocumentRevisions-V100
    .fseventsd
    .Spotlight-V100
    .TemporaryItems
    .Trashes
    .VolumeIcon.icns
    .com.apple.timemachine.donotpresent

    # Directories potentially created on remote AFP share
    .AppleDB
    .AppleDesktop
    Network Trash Folder
    Temporary Items
    .apdisk



    ### Laravel ###
    # Laravel 4 specific
    bootstrap/compiled.php
    app/storage/

    # Laravel 5 & Lumen specific
    public/storage
    public/hot
    storage/*.key
    Homestead.yaml
    Homestead.json



    ### Symfony ###
    # Cache and logs (Symfony2)
    /app/cache/*
    /app/logs/*
    !app/cache/.gitkeep
    !app/logs/.gitkeep

    # Email spool folder
    /app/spool/*

    # Cache, session files and logs (Symfony3)
    /var/cache/*
    /var/logs/*
    /var/sessions/*
    !var/cache/.gitkeep
    !var/logs/.gitkeep
    !var/sessions/.gitkeep

    # Logs (Symfony4)
    /var/log/*
    !var/log/.gitkeep

    # Parameters
    /app/config/parameters.yml
    /app/config/parameters.ini

    # Managed by Composer
    /app/bootstrap.php.cache
    /var/bootstrap.php.cache
    /bin/*
    !bin/console
    !bin/symfony_requirements

    # Assets and user uploads
    /web/bundles/
    /web/uploads/

    # PHPUnit
    /app/phpunit.xml
    /phpunit.xml

    # Build data
    /build/

    # Composer PHAR
    /composer.phar

    # Embedded web-server pid file
    /.web-server-pid
    
    ### Symfony Patch ###
    /web/css/
    /web/js/



    ### Node ###
    # Logs
    logs
    *.log
    npm-debug.log*
    yarn-debug.log*
    yarn-error.log*

    # Runtime data
    pids
    *.pid
    *.seed
    *.pid.lock

    # Directory for instrumented libs generated by jscoverage/JSCover
    lib-cov

    # Coverage directory used by tools like istanbul
    coverage

    # Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
    .grunt

    # Optional npm cache directory
    .npm

    # Optional eslint cache
    .eslintcache

    # Optional REPL history
    .node_repl_history

    # Yarn Integrity file
    .yarn-integrity

    # parcel-bundler cache (https://parceljs.org/)
    .cache

    # next.js build output
    .next

    # nuxt.js build output
    .nuxt

    # vuepress build output
    .vuepress/dist

    # Serverless directories
    .serverless

    # FuseBox cache
    .fusebox/



    ### PhpStorm ###    
    # User-specific stuff
    .idea/*

    # CMake
    cmake-build-*/

    # File-based project format
    *.iws

    # JIRA plugin
    atlassian-ide-plugin.xml