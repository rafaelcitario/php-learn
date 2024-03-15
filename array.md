# Arrays

[return to list](https://github.com/rafaelcitario/php-learn/blob/master/Readme.md)

```php
// Associative Array [key => value];
$associative = array('one' => 1, 'two' => '2');
$_associative = [
  'one' => 1,
  'two' => 2
];
echo $_associative['one'] . PHP_EOL;
echo $associative['two'] . PHP_EOL;
$_associative['three'] = 3;

// push method is not recommended to use with associative array
// because array_push add only a value to end of array without a key
array_push($associative, 30);
print_r($associative);

// to add values to associative array is recommended use:
$_associative['five'] = 5;
print_r($_associative); // this is most visualy confortable
var_dump($_associative);
```
