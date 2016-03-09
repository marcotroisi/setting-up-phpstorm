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

## Remote Server

To connect to a remote server where your code is stored, follow [this guide](https://www.jetbrains.com/phpstorm/help/create-new-project-add-remote-server.html).

## Issue Tracker

Should you want to integrate an issue tracker (e.g. Jira, YouTrack, Redmine, Pivotal Tracker) with PhpStorm, you can follow [this guide](https://www.jetbrains.com/phpstorm/help/enabling-integration-with-an-issue-tracking-system.html).

PhpStorm will differentiate between *local tasks* and *tracker tasks*, with the latter being a representation of all the tasks currently visible in the issue tracker, and the former being the tasks you are currently working on. PhpStorm will keep track of what you do in your local tasks.

## Version Control

It is also possible to integrate your version control system with PhpStorm. [Git](https://www.jetbrains.com/phpstorm/help/using-git-integration.html), [Subversion](https://www.jetbrains.com/phpstorm/help/using-subversion-integration.html), and [Mercurial](https://www.jetbrains.com/phpstorm/help/using-mercurial-integration.html) are supported amongst others.

Besides obvious version control functionalities like pull/checkout, commit, push, etc, probably one of the most useful tools that PhpStorm offers would be the ability to *fix merge/text conflicts* using a handy visual tool that will show the differences between your file and the one on the server, allowing you to quickly select which version would you like to keep.

## Database

A database integration couldn't be missing from PhpStorm. With PhpStorm, there is no need to use external software to handle database queries. You comfortably look at your tables/collections and safely run your queries the built-in console. Several database engines are supported, including MySql, Postgres, Oracle, SQLite and SQL Server. No official support appears to be available for NoSQL databases, but plugins can be found for [Mongo](https://plugins.jetbrains.com/plugin/7141). 
