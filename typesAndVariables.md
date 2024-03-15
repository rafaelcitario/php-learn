# Types and Variables

[return to list](https://github.com/rafaelcitario/php-learn/blob/master/Readme.md)

- to define types and variables:

```php
// is valid:

$variable = 'no underscore';
$_variable = 'underscore';
$_9variable = 'underscore + number';
$__variable = "two underscors";

// Strings:
$message = 'message';
echo '$message'; // this prints $message and dont 'message'
echo "$message"; // this prints 'message'

// Boolean types:
$isTrue = true | True | TRUE;
$isFalse = false | False | FALSE;

// integers types:
$twoelve = 12;
$twoelveNegative = -12;
$twoelveOctal = 012; // this is equals 10, because 0 denotes octal
$twoelveHex = 0x0C; // this is equals 12, but in hexadecimal
$twoelveBinary = 0b1100; // this is equals 12, but 0b detones binary

// floats types (knowledge how doubles to):
$justNumbers = 1.234;
$numbersAndLetters = 1.2e3;
$iDontKnow = 7E-10;

// to delete variables:
$name = 'Dwayne "The Rock" Johnson';
unset($name);
// echo $name; // this is a error, because is unasigned (null) variable

// Arithmetic
$sum        = 1 + 1; // 2
$difference = 2 - 1; // 1
$product    = 2 * 2; // 4
$quotient   = 2 / 1; // 2

// Shorthand arithmetic
$number = 0;
$number += 1;      // Increment $number by 1
echo $number++;    // Prints 1 (increments after evaluation)
echo ++$number;    // Prints 3 (increments before evaluation)
$number /= $float; // Divide and assign the quotient to $number

// to use \t \n \anything do you need use double quotes:
$dobleQuotes = "this contains a tab \t <-- do you see?";
$singleQuotes = 'this dont contains a tab \t just a slash and t';

// the same is to use interpolation of string:
$age = 27;
$toldMyAge = "I'm ${age} yeas old"; // note: this is deprecate since 8.2 php version
$toldMyAgeRight = "I'm $age years old"; // use this way!

// newdoc:
$nowdoc = <<<'END'
Multi line
strings
END;
echo $nowdoc;

// String concatenation is done with .
echo 'This string ' . 'is concatenated';  // Returns 'This string is concatenated'

// Strings can be passed in as parameters to echo
echo 'Multiple', 'Parameters', 'Valid';  // Returns 'MultipleParametersValid'
```
