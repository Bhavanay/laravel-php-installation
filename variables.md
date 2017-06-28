### Variables:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A variable in PHP is a name of memory location that holds data. In PHP, a variable is declared using $ sign followed by variable name. <br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The main way to store information in the middle of a PHP program is by using a variable.
Here are the most important things to know about variables in PHP.
* All variables in PHP are denoted with a leading dollar sign ($).
* The value of a variable is the value of its most recent assignment.
* Variables are assigned with the = operator, with the variable on the left-hand side and the expression to be evaluated on the right.
* Variables can, but do not need, to be declared before assignment.
* Variables in PHP do not have intrinsic types - a variable does not know in advance whether it will be used to store a number or a string of characters.
* Variables used before they are assigned have default values.
* PHP does a good job of automatically converting types from one to another when necessary.

**Rules for PHP variables:**
- A variable starts with the $ sign, followed by the name of the variable
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive ($age and $AGE are two different variables)</br>
Syntax of declaring a variable is:<br/>
    ```$variablename=value;```<br/>
Example:
```
<?php
$x = 5;
$y = 4;
echo $x + $y;
?>
```
Output:9<br/>
1. **Local variables:**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A variable declared in a function is considered local; that is, it can be referenced solely in that function. Any assignment outside of that function will be considered to be an entirely different variable from the one contained in the function.
2. **Functional parameters:**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Function parameters are declared after the function name and inside parentheses. They are declared much like a typical variable.
3. **Global variables:**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In contrast to local variables, a global variable can be accessed in any part of the program. However, in order to be modified, a global variable must be explicitly declared to be global in the function in which it is to be modified. This is accomplished, conveniently enough, by placing the keyword GLOBAL in front of the variable that should be recognized as global. Placing this keyword in front of an already existing variable tells PHP to use the variable having that name. 
4. **Static variables:**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The final type of variable scoping that I discuss is known as static. In contrast to the variables declared as function parameters, which are destroyed on the function's exit, a static variable will not lose its value when the function exits and will still hold that value should the function be called again.
5. **Constant:**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A constant is a name or an identifier for a simple value. A constant value cannot change during the execution of the script. By default, a constant is case-sensitive.To define a constant you have to use define() function and to retrieve the value of a constant, you have to simply specifying its name.You can also use the function constant() to read a constant's value if you wish to obtain the constant's name dynamically.

