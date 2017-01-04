# PHP 7 return type declarations and mock objects

When using PHP 7 return type declarations and using a PHPUnit mock object. You must use PHPUnit 5.1 or greater. Otherwise you will get the following error:

``` PHP Fatal error:  Declaration of Mock_Example_62b1a36c::exampleMethod(int $id) must be compatible with Example\Namespace\ExampleInterface::exampleMethod(int $id): Example\Collection in /project/path/vendor/phpunit/phpunit-mock-objects/src/Framework/MockObject/Generator.php(291) : eval()'d code on line 1 ```

[more info](https://github.com/sebastianbergmann/phpunit-mock-objects/issues/283)
