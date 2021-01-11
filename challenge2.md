# PHP Syntax Guide
## PHP Comments
PHP comments are like HTML and JS comments, they are there to remind you of what you have done and to communicate to others what you have done when they are looking at the code.
```
<?php
// single line comment

# also a single line comment

/*
multiple line comment 
*/
?>
```
## PHP Variables
Variables in PHP are symbols and names that represent a value and are created to store characters, strings, memory addresses and numeric values for use in the program that you are creating.

* Start the PHP variable with a dollar sign ($) and then the name of the variable

* Variable names begin with a letter or an underscore (_)

* Follow the $ and letter or underscore with letters, underscores and numbers in any amount

* You can create a variable name with more than one word by separating the words with an underscore

* You cannot use $ as an assigned value 

```
<?php
$txt = "hey";
$t = 6;
$c = 9;
?>
```
## PHP Echo / Print
Echo is used to pull data and show it on the screen. Echo does not have a return value, it is not going to output the answer and it has the capacity to take more than one parameter. Echo is a bit faster than the PHP print.

Print is slower than echo however, print will return a value. Print can only accept one argument.

```
<?php
echo "<h2>I like to ski</h2>";
echo "sking is good<br>";
echo "I have fun ", "sking ", "with ", "my ", "friends";
?>
```
```
<?php
print "<h2>I like to ski";
print "sking is good<br>";

?>
```
## PHP Data Types
There are different kinds of data and you can use variables to store each type. The data types perform different operations based on what the programmer needs them to do. The data types that you can use in PHP include: string, constants operator, integer, array, boolean, float, object, resource, and NULL.
```
echo "hey";
```
## PHP Strings
A PHP supported data type, strings are an arrangement of characters that are inside either single or double quotes.
```
<?php
echo "Zack";
echo 'Torin';

?>
```
## PHP Numbers
When assigning an integer value to a variable it will automatically be an integer.
```
<?php
$x = 23;
$y = 6;
?>
```
## PHP Constants
Just like variables, constants are symbols and names that represent a value. Unlike variables however, constants remain the same after they have been defined. You can’t change or redefine them.
* Constants start with either a letter or an underscore but never a dollar sign ($)

```
<?php
define("INSULT", "You big dumb dumb");
echo INSULT;
?>
```
## PHP Operators
Variables and values need operators assigned to them so that they can perform the operations that have been coded if you are using them. In PHP there are a variety of operator groups categorized by the type of operation they do.
* Arithmetic operators
* Array operators
* Assignment operators
* Conditional assignment operators
* Comparison operators
* Increment/Decrement operators
* Logical operators
* String operators
```
<?php
echo $t == $g;
?>
```
## PHP If & Else & Elseif
When you want the program to perform specific actions in specific order based on the conditions you have set then you will use if & else or Elseif statements. These are conditional statements that allow you to perform different actions for different conditions.

You can use conditional statement for one or more conditions:
* If - one condition

* If & else - if condition is true run this code, if it is not true run this code

* If & else repeated - will run code for more than one condition being met or not being met

```
<?php
$t = date("H");

if ($t < "10") {
  echo "your early";
} elseif ($t < "20") {
  echo "You're on time";
} else {
  echo "You're late";
}
?>
```
## PHP Functions
PHP has the ability to use built in functions and custom functions that you can create for your own program.

A function surrounds code and makes it possible to call the function to run the code that is inside of it. A function can be called repeatedly, as often as you need it.
* Function names have to start with either a letter or an underscore (_)

* Help yourself and others that use your coding by naming the function by what it does

* When the user defines the function, start the declaration with the word function:

```
<?php
function myFunction() {
  echo "hey";
}

myFunction();
?>
```
## PHP Arrays
One variable can have more than one value in a shortened format by creating an array. Arrays allow you to assign the variable more than one value so that you can offer a list of options for the variable.

```
<?php
$carCo = array("Mercedes", "BMW", "Audi");
echo " German companies " . $carCo[0] . ", " . $carCo[1] . " and " . $carCo[2] .;
?>
```
## PHP Loop
When conditions are true, a loop can be used to run the code repeatedly for a specific number of times. This eliminates the need to write similar code over and over. PHP uses four loop types: while, do - while, for - loops, foreach.

```
<?php
for ($x = 0; $x <= 20; $x++) {
  echo "Seconds left: $x <br>";
}
?>
```