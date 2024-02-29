# PHP Tools
_Static analysis tools for PHP projects_

Provides `php-cs-fixer`, `phpstan`, `psalm`, `rector`, & `twigcs` as isolated
composer installs within your project. This eliminates the need to worry about 
any underlying conflicts with tool dependencies and your own project dependencies.

## Install

1) From within your project,
`git submodule add https://github.com/rushlow-development/php-tools tools`. This
will "clone" the `php-tools` repo into `path-to-project/tools`.

2) Run `tools/bin/install` which will run `composer upgrade` in each of the tool
directories.

3) Copy and paste the contents of `scripts.json` into your _`root`_ composer.json
file. This will allow you to run `composer tools:run` from your project root
directory. 

## In the future

I'd like to use composer plugins / custom installers to automate this. Allowing one
to run `composer require --dev rushlow-development/php-tools` and then the tools
would be installed as needed... 
