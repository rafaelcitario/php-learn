# Structures of decision in php

[return to list](https://github.com/rafaelcitario/php-learn/blob/master/Readme.md)

```php
$boolean = true;

if ($boolean) {
  print "is true";
}

if ($boolean) {
  print 'I don\'t';
} else {
  print 'I get printed';
}

if ($boolean === false) {
  print 'Does not get printed';
} elseif ($boolean === true) {
  print 'Does';
}

print($boolean === false ? 'Does not get printed' : 'Does');

/*
 if this is false return false, but this is true return string 'Does'
 this is a shorthand ternary
*/
print($boolean ?: 'Does');

// coalesce operator
$notExists = null;
$exists = 'this exists!';

print $exists ?? 'this not exists'; // this variable exist so this return the content value
print $notExists ?? 'this not exists'; // this variable not exists, so return the second opt 'this not exists' message
echo $notExists ?? "\n this variable is null";


// switch
$isRedInside = 'water mellon';
switch ($isRedInside) {
  case ('water mellon'):
    print('the fruit is a water mellon');
    break;
  case ('apple'):
    print('this fruit is an apple');
    break;
  default:
    print('tf man, what the fruit do you choose?');
    break;
}

/**
 * if at echo message put "$i".PHP_EOL does print 1 ... 10
 * if at echo message put "\n $i" does print 0...10
 * if at echo message dont put \n or php_eol, does print 012345678910
 */

$i = 0;
while ($i <= 10) {
  echo "\n";
  echo "$i";
  $i++;
}

$j = 0;
do {
  echo "\n";
  echo "$j";
  $j++;
} while ($j <= 10);

for ($k = 0; $k <= 10; $k++) {
  echo "\n";
  echo "$k";
}

$books = [
  'Gestão do conhecimento',
  'Estrutura de dados e algoritmos em Javascript',
  'Código Limpo',
  'Biblia',
  'Devocional'
];

foreach ($books as $book) {
  echo $book . PHP_EOL;
}


$l = 0;
while ($l < 5) {
  if ($l === 3) {
    break; // Exit out of the while loop
  }
  echo $l++;
} // Prints "012"

for ($m = 0; $m < 5; $m++) {
  if ($m === 3) {
    continue; // Skip this iteration of the loop
  }
  echo $m;
} // Prints "0124"
```
