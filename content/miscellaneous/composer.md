[back to table of content](../../readme.md)

# Composer #
Useful command line snippets and cheat sheet

### Useful commands ###

    # update autoloaded files (new classes)
    composer dump-autoload
    
    # install dependencies
    composer install
    
    # update dependency versions
    composer update

#### Update .env / parameters.yml on deploy ####

    "scripts": {
        "symfony-scripts": [
            "Incenteev\\ParameterHandler\\ScriptHandler::buildParameters"
        ],
        "post-install-cmd": [
            "@symfony-scripts"
        ],
        "post-update-cmd": [
            "@symfony-scripts"
        ]
    }
