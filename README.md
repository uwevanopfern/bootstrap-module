## Dynamic Module

### Publishing steps

-   Create A Module
-   Make sure that you mentioned the type of the module in the composer.json as laravel-module
-   Push the module to github, bitbucket, gitlab etc. Make sure the repository name follows the convention then it will be moved to the right directory automatically. The repo name should be like <namespace>/<name>-module, a -module at the end. Example: https://github.com/uwevanopfern/bootstrap-module. This module will be installed in Modules/Bootstrap directory
-   Submit your code to package

## Install module in Modules directory steps

-   Install nwidart/laravel-modules in your laravel project

        composer install nwidart/laravel-modules

-   Install joshbrw/laravel-module-installer in your laravel project which will move the module files automatically into Modules directory

        composer install joshbrw/laravel-module-installer

-   Specify different directory rather than Modules by adding the following in your composer.json

          "extra": {
              "module-dir": "Custom"
          }

-   Finally install your module package

          composer require uwevanopfern/bootstrap-module
