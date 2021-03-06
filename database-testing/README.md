### Blog Sample:  Database Testing

Steps to run the code referenced in the blog post [Database Testing with PHPUnit](http://blog.fraserreed.com/phpunit/2016/04/06/database-testing-with-phpunit.html).

1.  Install Vagrant (https://www.vagrantup.com/)
2.  Run `vagrant up` to install the ubuntu 14.04 vm, with MySQL preinstalled
3.  Run `composer install` to install local PHP packages
4.  Run `vendor/bin/phinx migrate` to install the correct database schema and data
5.  Run `vendor/bin/phpunit` to run the unit tests

You can also optionally run the tests with code coverage, which can be viewed in the `report` directory:

`vendor/bin/phpunit --coverage-html report`