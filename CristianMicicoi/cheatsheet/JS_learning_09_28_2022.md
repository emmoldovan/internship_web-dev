## _**JavaScript** Keywords_:

  - _var_     -->    Declare a variable;
  - _let_     -->    Declare a block variable;
  - _const_	  -->    Declare a block constant;
  - _if_      -->    Marks a block of statements to be executed on a condition;
  - _switch_  -->    Marks a block of statements to be executed in different cases;
  - _for_     -->    Marks a block of statements to be executed in a loop;
  - _function_-->   Declares a function;
  - _return_  -->   Exits a function;
  - _try_     -->    Implements error handling to a block of statements;

Always declare JavaScript variables with _var, let, or const_. 

The _var_ keyword is used in all JavaScript code from 1995 to 2015.

The _let_ and _const_ keywords were added to JavaScript in 2015.

If you want your code to run in older browsers, you must use _var_.

If you want a general rule: always declare variables with _const_.

If you think the value of the variable can change, use _let_.

``` <script>
let x, y, z;   //statement1 or
var x, y, z;  // Declare 3 variables
x = 5;    // Assign the value 5 to x
y = 6;    // Assign the value 6 to y
z = x + y;  // Assign the sum of x and y to z

//"The value of z is " + z + ".";
</script>
```
## The _**Assignment** Operator_

In JavaScript, the _equal_ sign (=) is an _"assignment"_ operator, not an _"equal to"_ operator.

This is different from algebra. The following does not make sense in algebra: x = x + 5

In JavaScript, however, it makes perfect sense: it assigns the value of _x + 5_ to _x_.

(_It calculates the value of x + 5 and puts the result into x. The value of x is incremented by 5_.)

Note: 
**The _"equal to"_ operator is written like **==** in JavaScript**.

## _JavaScript_ **_Data Types_**

JavaScript variables can hold numbers like _100_ and text values like _"John Doe"_.

In programming, text values are called text **_strings_**.

JavaScript can handle many types of data, but for now, just think of _numbers_ and _strings_.

**_Strings_ are written inside double or single quotes. Numbers are written without quotes.**

**If you put a number in quotes, it will be treated as a text string.**

Example:
const pi = 3.14;
let person = "John Doe";
let answer = 'Yes I am!';

## **_Declaring_** a JavaScript Variable

Creating a variable in JavaScript is called _"declaring"_   a variable.

You declare a JavaScript variable with the _var_ or the _let_ keyword:

_var carName_ or _let carName_;