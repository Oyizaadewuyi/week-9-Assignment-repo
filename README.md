W3 SCHOOL (JAVASCRIPT ARRAY METHODS)
below is the list of Javascript Array Methods
1. Array length
2. Array toString()
3. Array pop()
4. Array push()
5. Array shift()
6. Array unshift()
7. Array join()
8. Array delete()
9. Array concat() 
10. Array flat()
11. Array splice()
12. Array slice()
  
Explanation with examples

1. Array length

The length property returns the length (size) of an array.

Syntax(array.length)
Return the length of an array:

(array.length = number)
Set the length of an array:

example
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let length = fruits.length;

2. Array toString()

The JavaScript method toString() converts an array to a string of (comma separated) array values.
Every JavaScript object has a toString() method.
The toString() method is used internally by JavaScript when an object needs to be displayed as a text (like in HTML), or when an object needs to be used as a string. it has no parameters.

Syntax(array.toString)

example 
Convert an array to a string:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let text = fruits.toString();

3. Array pop()

the pop method removes the lastelement from an array

Syntax (array.pop)
no parameters

Example
Remove (pop) the last element:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();

pop() returns the element it removed:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();

4. Array push()

the push method adds a new element to an array (at the end)

Syntax (array.push)
parameters (item1, item2, ..., itemX)
The item(s) to add to the array.
Minimum of one item is required.

example 
Add a new item to an array:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi");

Add two new items to the array:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi", "Lemon");
Popping and Pushing
When you work with arrays, it is easy to remove elements and add new elements.
This is what popping and pushing is:
Popping items out of an array, or pushing items into an array.

5. Array shift()

the shift array method removes the first array element and shift other element in to the index, it returns the value that was shifted out

Syntax (array.shift)
example 
Shift (remove) the first element of the array:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();

The shift() method returns the shifted element:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();

6. Array unshift()

The unshift method adds a new element to an array (at the beginning), and "unshifts" older elements. this method returns a new array length.
Syntax (array.unshift)
Parameters; item1,item2,itemX

example 
Add new elements to an array:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon","Pineapple");

7. Array join()

this method joins all array elements into a string. it behaves like the toString() method but you can specify the saperator. it does not change the original array. 

Syntax (array.join)
Parameter; Saperator
example 
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let text = fruits.join();
any saperator can be defined but comma is the default saperator.

8. Array delete()

the array delete operator method can be used to delete array of element but they leave undefined holes in the array. it is better to use the pop() or shift() methods.

9. Array concat()

the concat method creates a new array by merging existing arrays. it does not change the existing arrays but always returns a new array,it can take strings as arguments and it can take any number of array arguments.

Syntax
array1.concat(array2, array3, ..., arrayX)
Parameters
Parameter; array1,...	Required.
The array(s) to be concatenated
example 
const arr1 = ["Raihan", "Annah"];
const arr2 = ["Emem", "Tobias", "Ebere"];
const children = arr1.concat(arr2);
merging strings and numbers
const arr1 = ["Cecilie", "Lone"];
const arr2 = [1, 2, 3];
const arr3 = arr1.concat(arr2);

10. Array flat()

the array flat is a method that reduces the dimension of an array.
it creates a new array with a sub array element merged(concateneted) together to a specified depth.

Syntax (array.flat(depth))
the parameter is depth
depth is Optional.
How deep a nested array should be flattened.
Default is 1.

example
Create a new array with the sub-array elements concatenated:
const myArr = [[1,2],[3,4],[5,6]];
const newArr = myArr.flat();

11. Array splice()

this method is used to add new items to an array. it overrides the original array.

Syntax (array.splice(index, howmany, item1, ....., itemX))
the parameters are 
1. index; Required. The position to add/remove items.
Negative value defines the position from the end of the array.
2. howmany	Optional.   Number of items to be removed.
3. item1, ..., itemX	Optional. New elements(s) to be added.
examples..
At position 2, add 2 elements:
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 0, "Lemon", "Kiwi");

At position 2, remove 2 items:
const fruits = ["Banana", "Orange", "Apple", "Mango", "Kiwi"];
fruits.splice(2, 2);

12. Array slice()

The slice() method returns selected elements in an array, as a new array. This method selects from a given start, up to a (not inclusive) given end.
The slice() method does not change the original array.

Syntax(array.slice(start, end))
Parameters
Start	Optional.
Start position. Default is 0.
End	Optional.
End position. Default is last element....


JAVASCRIPT FUNCTIONS
W3SCHOOLS and Mdn web docs(FUNCTION)

w3school defines function as the following
A function is a block of code designed to perform a particular task.
A function is executed when "something" invokes it (calls it).

JavaScript Function Syntax
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().
Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

Function Return
When JavaScript reaches a return statement, the function will stop executing.
If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.
Functions often compute a return value. The return value is "returned" back to the "caller"

With functions 
you can reuse code
You can write code that can be used many times.
You can use the same code with different arguments, to produce different results.

The () Operator
The () operator invokes (calls) the function
Functions Used as Variable Values
Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

Mdn define functions 
As a subprograms that can be called by code eith external or internally. a function is composed of a sequence of statements called the function body. Values can be passed to a function as parameters, and the function will return a value.
In JavaScript, functions are first-class objects, because they can be passed to other functions, returned from functions, and assigned to variables and properties. They can also have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called.

javascript has 4 types of function
1. Regular function; can return anything, always runs to completion after being called or invoked
2. Generator function; returns a Generator object, it can be paused and resumed with the yield operator
3. Async function; returns a Promise; can be paused and resumed with the await operator
4. Async generator function; returns an AsyncGenerator object; both the await and yield operators can be used.
for every kind of function, there are tree ways to define it 
1. declaration
2. expression
3. constructor

The Function() constructor, function expression, and function declaration syntaxes create full-fledged function objects, which can be constructed with new. However, arrow functions and methods cannot be constructed. Async functions, generator functions, and async generator functions are not constructible regardless of syntax.

For function expressions, there is a distinction between the function name and the variable the function is assigned to. The function name cannot be changed, while the variable the function is assigned to can be reassigned.The function name can be used only within the function's body. Attempting to use it outside the function's body results in an error.

A function declaration also creates a variable with the same name as the function name. Thus, unlike those defined by function expressions, functions defined by function declarations can be accessed by their name in the scope they were defined in, as well as in their own body.

A function defined by a function expression or by a function declaration inherits the current scope. That is, the function forms a closure. On the other hand, a function defined by a Function constructor does not inherit any scope other than the global scope (which all functions inherit).

FUNCTIONS PARAMETERS
Each function parameter is a simple identifier that you can access in the local scope.

There are three special parameter syntaxes:

Default parameters: allow formal parameters to be initialized with default values if no value or undefined is passed.
The rest parameter: allows representing an indefinite number of arguments as an array.
Destructuring: allows unpacking elements from arrays, or properties from objects, into distinct variables.

We can pass arbitrary data to functions using parameters.
In the example below, the function has two parameters: from and text.

function showMessage(from, text) { // parameters: from, text
  alert(from + ': ' + text);
}
showMessage('Ann', 'Hello!'); // Ann: Hello! (*)
showMessage('Ann', "What's up?"); // Ann: What's up? (**)

When the function is called in lines (*) and (**), the given values are copied to local variables from and text. Then the function uses them.

When a value is passed as a function parameter, it’s also called an argument.
In other words, to put these terms straight:
A parameter is the variable listed inside the parentheses in the function declaration (it’s a declaration time term).

An argument is the value that is passed to the function when it is called (it’s a call time term).
We declare functions listing their parameters, then call them passing arguments.

NAMING A FUNCTION
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

Function starting with…
"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.

RETURNING A VALUE
A function can return a value back into the calling code as the result.
The simplest example would be a function that sums two values:

function sum(a, b) {
  return a + b;
}

let result = sum(1, 2);
alert( result ); // 3
The directive return can be in any place of the function. When the execution reaches it, the function stops, and the value is returned to the calling code (assigned to result above).

LOCAL VARIABLES
A variable declared inside a function is only visible inside that function.
Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.
Local variables are created when a function starts, and deleted when the function is completed.

GLOBAL VARIABLES
Variables declared outside of any function, such as the outer userName in the code above, are called global.
Global variables are visible from any function (unless shadowed by locals).

It’s a good practice to minimize the use of global variables. Modern code has few or no globals. Most variables reside in their functions. Sometimes though, they can be useful to store project-level data.



JAVASCRIPT CONTROL FLOW STATEMENTS

WHAT IS CONTROL FLOW STATEMENTS
Control Flow refers to the order in which statements are executed in a program. It's like a set of instructions that tell the computer what to do and in what order. In JavaScript, Control Flow is crucial for making decisions and repeating actions based on certain conditions.

There are two types of Control Flow: sequential and conditional. 
Sequential control flow executes statements one after another in the order they are written. 
Conditional control flow allows the program to make decisions based on certain conditions.

In JavaScript, there are three main types of control flow statements:

if/else statements
switch statements
loops.

1. The if statement is the most common way to write a conditional expression in JavaScript. It's used to execute a block of code if a condition is true.
For example, let's say we want to check if a number is even. We can use the if statement to execute a block of code if the number is indeed even.

const number = 4;
if (number % 2 === 0) {
  console.log("The number is even");
}
This will log "The number is even" to the console because 4 is actually an even number.

The else statement
The else statement is used in conjunction with the if statement. It's used to execute a block of code if the if statement's condition is false.
example
const number = 5;

if (number % 2 === 0) {
  console.log("The number is even");
} else {
  console.log("The number is odd");
}
This will log "The number is odd" to the console because 5 is not even number.

Switch Statements
Switch statements are used to execute a block of code based on the value of a variable or expression.

The switch statement is used to execute different blocks of code depending on the value of a variable or expression. It's like a multiple-choice question where each answer corresponds to a different block of code.

example
let's say we want to log a message depending on the day of the week. We can use the switch statement to execute different blocks of code depending on the day.

const day = "Monday";
switch (day) {
  case "Monday":
    console.log("It's Monday, let's conquer the week!");
    break;
  case "Friday":
    console.log("It's Friday, time to relax!");
    break;
  default:
    console.log("Just another day...");
}
This will log "It's Monday, let's conquer the week!" to the console because the day variable is set to "Monday"


Loops
Loops are used to execute a block of code multiple times, based on a certain condition, They will loop until a certain condition is met.

There are two main types of loops in JavaScript: 
1. for loops and
2. while loops.

The for loop
The for loop is used to repeat a block of code a specific number of times. It's like a countdown where you know how many times you need to repeat the code.

Here’s an example of a for loop that prints the numbers 1 through 5 to the console:
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
In this example, the code inside the for loop will be executed five times, starting with i = 1 and incrementing i by 1 each time, until i is greater than 5.

While Loops
A while loop simply repeats itself while something is true. Theoretically a while loop can loop forever. It continues until the condition is false.

Here’s an example of a while loop that prints the numbers 1 through 5 to the console:
let i = 1;
while (i <= 5) {
  console.log(i);
  i++;
}
In this example, the code inside the while loop will be executed as long as the condition i <= 5 is true. The variable i is initialized to 1, and then incremented by 1 each time the loop runs, until i is greater than 5.

While and Do…While Loops
The while loop executes a specified statement as long as the test condition evaluates to true. The do…while loop will first execute the code, then continue while the condition remains true.



