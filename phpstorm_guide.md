# PhpStorm

## How to set up PHPUnit

To enable PHPUnit support and run it from within PhpStorm, follow [this guide](https://www.jetbrains.com/phpstorm/help/enabling-phpunit-support.html).

Ideally, the best approach would be to run PHPUnit from Composer, but in case you're working on a project that doesn't use Composer, the way to go is to follow the instructions under the section *[Running PHPUnit from the phpunit.phar archive](https://www.jetbrains.com/phpstorm/help/enabling-phpunit-support.html#usePhpUnitFromPhar)*.

A good idea would be to place the executable in your OS's `PATH`. To do that, write the following on a terminal:

    curl https://phar.phpunit.de/phpunit.phar -o phpunit.phar
    chmod +x phpunit.phar
    mv phpunit.phar /usr/local/bin/phpunit

This way you'll be able to run phpunit directly from anywhere, e.g. `phpunit ~/MyProject/src/Tests/`.

## Code Styling

To define and customise code styling rules on PhpStorm, follow [this guide](https://www.jetbrains.com/phpstorm/help/code-style-php.html).

In most cases, the simplest way to keep code styling consistent, is to click on the *Set From* option and choose one of the options. The most used and traditionally accepted styling guideline is **PSR2**, which you should choose unless told otherwise. The same applies for all other options: unless told otherwise, keep the default values that will come out once you've chosen **PSR2** as your guideline.

### Reformatting code

PhpStorm offers a handy shortcut to [reformat code](https://www.jetbrains.com/phpstorm/help/reformatting-source-code.html). By pressing `Ctrl+Alt+L` (`⌥⌘L` on Mac) you can quickly format a block of code and possibly fix styling errors you may have just made.
