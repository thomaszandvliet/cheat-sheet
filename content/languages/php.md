[back to table of content](../../readme.md)

# PHP #
Useful PHP snippets and settings

#### .ini location ####

    php --ini

#### Increase memory (composer) ####
Get current `memory_limit`

    php -r "echo ini_get('memory_limit').PHP_EOL;"

Increase limit

    # unlimited
    memory_limit = -1

    # specified value
    memory_limit = 2G

[Source](https://stackoverflow.com/questions/49212475/composer-require-runs-out-of-memory-php-fatal-error-allowed-memory-size-of-161)