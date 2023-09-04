# php-Arrays

### To create Simple or Numerical Arrays

- Using array() or [].

```
<?php
//Create array with Array construct
$a = array(5, 4, "Web", "Database");

//Create array with short array syntx
$b = ['MySQL', 'JavaScript', 'PHP'];

// Print the third element from the array
echo $a[2]; //Web
echo $b[2]; //JavaScript

// Print the first element from the array
echo $a[0]; //5
echo $b[0]; //MySQL
```

- next method placing square brackets after variable name $newArray[].

```
<?php
$newArray[] = "Potatoes";
echo $newArray[0]; //Potatoes
```

### Debug array and objects with print_r() and var_dump()

- print_r() display just the index and values in human readable form.
- var_dump() variable dump used to debug in depth of its data type, length and values of nested elements.

### Heterogeneous arrays

- means mixed type

```
<?php
$mixedBag = array("cat", 42, 8.5, false);
var_dump($mixedBag);


array(4) { [0]=> string(3) "cat"
           [1]=> int(42)
           [2]=> float(8.5)
           [3]=> bool(false) }
```

### Associative Array

- An associative array can use string indexes (or keys) to access values stored in the array.

```
<?php
$a = ['website' => 'brainbell.com', 'Tutorial' => 'PHP'];
echo $a['website']; //brainbell.com

```

### Multidimensional or Nested Arrays

- Arrays can also be nested, when an array element itself is an array.

```
<?php
$a = array(
  'Roman' =>
    array('one' => 'I', 'two' => 'II', 'three' => 'III'),
  'Arabic' =>
    array('one' => '1', 'two' => '2', 'three' => '3')
);

echo $a['Roman']['one'];  //I
echo $a['Arabic']['two']; //2;
```
