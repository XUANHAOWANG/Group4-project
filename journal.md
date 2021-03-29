### switch

First set the expression n (usually a variable). The value of the expression will then be compared with the value of each case in the structure. If there is a match, the code block associated with the case will be executed. Please use break to prevent the code from automatically running to the next case



### advantage
When the amount expressed by the variable expression matches the constant in one of the case statements, the statements following this case statement are executed, and all subsequent case statements are executed in turn, unless a break; statement jumps out of the switch statement. . If the amount of the constant expression does not match the constants of all the case statements, the statements in the default statement are executed.

### Disadvantage
The switch statement is very useful, but it must be used with caution. Any switch statement written must follow the following rules:
1. Switch can only be used for integer types in basic data types, including int, char, and so on. For other types, you must use the if statement.
2.The parameter type of switch() cannot be a real type.


### The main difference between if-else and switch
The expression in the if statement determines whether the statement is executed in the if block or under the else block. On the other hand, the expression in the switch statement determines which case is executed.
You can have multiple if statements to select multiple statements. In switch, you have only one expression for multiple choices.
If-else statement checks for equality and logical expression. On the other hand, switch only checks for equality.
The if statement calculates integers, characters, pointers or floating-point types or boolean types. On the other hand, the switch statement only counts character or integer data types.
The order of execution is similar to the statements under the if block or the statements under the else block. On the other hand, the expression in the switch statement determines which case is executed. If you do not apply the break statement after each case, the expression will be executed until the end of the switch statement.
If the result of the internal expression is false, the statement inside the else block will be executed. If the expression in the switch statement is false, the default statement is executed.
Editing the if-else statement is difficult because it is cumbersome to keep track of where corrections are needed. On the other hand, since it is easy to track switch statements, it is easy to edit them.


### loop
JavaScript loops are used to repeatedly run blocks of code-until certain conditions are met. When developers talk about iteration or iteration (such as arrays), it is the same as loop. JavaScript provides multiple options to run code blocks repeatedly, including while, do while, for and for-in.

This is an example of a JavaScript while loop:

var sum = 0;
var number = 1;
while (number <= 50 ){ //-condition
  And + = number; //-body
  Number++; //-updater
}
Alert (" Sum =" + sum ); // => Sum = 1275
Evaluate the conditions first. If it is true, the statement block after the while statement is executed. Repeat this process until the condition becomes false. This is called a pre-test loop because the conditions are evaluated before the block is executed.

This number++ statement is called update. Removing it will cause an infinite loop. You must always include a statement that guarantees the termination of the loop in the loop, otherwise you will encounter this problem (JavaScript Loops-Dofactory, 2021).

### Different types of loops in JavaScript
while — As long as the specified condition evaluates to true, loop through the code block.
do...while — loop through the code block once; then evaluate the condition. If the condition is true, the statement is repeated as long as the specified condition is true.
for — Loop through the code block until the counter reaches the specified number.
for...in — Traverse the properties of the object.
for...of — Iterate through iterable objects, such as arrays, strings, etc(JavaScript While, Do-While, For and For-In Loops - Tutorial Republic, 2021).

#### while
var i = 1;
while(i <= 5) {
    document.write("<p>The number is "+ i + "</p>");
    i++;
}

#### do ... while loop
var i = 1;
do {
    document.write("<p>The number is "+ i + "</p>");
    i++;
}
while(i <= 5);

#### for loop
for(var i=1; i<=5; i++) {
    document.write("<p>The number is "+ i + "</p>");
}

#### for...in...
// An object with some properties
var person = {"name": "Clark", "surname": "Kent", "age": "36"};
 
// Loop through all the properties in the object
for(var prop in person) {
    document.write("<p>" + prop + "=" + person[prop] + "</p>");
}

#### for... of loop
// Iterating over array
let letters = ["a", "b", "c", "d", "e", "f"];

for(let letter of letters) {
    console.log(letter); // a,b,c,d,e,f
}

// Iterating over string
let greet = "Hello World!";

for(let character of greet) {
    console.log(character); // H,e,l,l,o, ,W,o,r,l,d,!
}





### Reference
JavaScript Loops - Dofactory. (2021). Dofactory.com. https://www.dofactory.com/javascript/loops#:~:text=JavaScript%20loops%20are%20used%20to,%2C%20for%20and%20for%2Din.

JavaScript While, Do-While, For and For-In Loops - Tutorial Republic. (2021). Tutorialrepublic.com. https://www.tutorialrepublic.com/javascript-tutorial/javascript-loops.php
