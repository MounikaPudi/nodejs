javascript is a case-sensitive language -- True
Scripting languages like javascript are based on the ECMA Script 
what is the result of 10 === '10' --> false
what are the pop up boxes available in javascript --> prompt,alert,confirm
which is not true about javascript --> javascript can detect if cookies are enabled in the browser
javscript can read/write files in the client's hard disk directly
what is the value of x?
var x = "100" + y
100undefined
javascript is a loosely typed language -- True
what is the type of null? -- object
javascript supports automatic type conversion --> True
Assumes the functions are called in the order given. what will the alert box show?
var a = 5;
function first() {
a = 6;
}
function second() {
alert(a);
}
o/p: 6 

primitive values are passed by reference --> False

nesting of functions is allowed in javascript --> true/false -- true
name of the function for string-to-integer conversion in javascript-- parseInt
A callback is a plain javascript function passed to some method as an argument or option
The scope of variables declared outside all functions - global
object is a primitive type -- false
The javscript object used to perform mathematical operations -- math
var x = typeof new String("abc") 
what is the value of x?
object
Name any 2 functions to delete an element in an array - delete,splice
How will you create a date object --> new date()
AJAX stands for --> Asynchronous Javacript and XML 
The object used by browsers to request data from server without reloading the page?
XMLHttpRequest
Although X in AJAX is XML ,the response for AJAX request is usually in JSON format
The XMLHTTPREQUEST once sent cannot be cancelled -- false
The property of XMLHttpRequest 
object that tells the current state of 
request -- readystate
I am a collection of 
properties, and a property is 
an association between a 
name (or key) and a value.
Who am I? -- object

FUNCTIONS
Block of code that performs predefined task.
Helps in achieving modularity.
Creates reusable code.
Executed when it is called/invoked or when an event is triggered.
Declared using ‘function’ keyword
Return Values:
• Functions always return a value.
• Functions can return other objects including other functions.
• If a function doesn’t return a value explicitly, it returns 
‘undefined’.
FUNCTION DEFINITION
function definition --> function statement
                    ---> function expression 
                    ---> Arrow function(=>)
function statement 

declare to use later
executes when called/invoke
functions are treated as objects
can have properties and methods

function definition and function statement 
function functionName ([param0,[param1,[...paramn]]])
{
statements
}
starts with the function keyword
function name:
  --> provide a meaningful name
  --> follow camelcase notation


function parameters
contains the data passed to the functions
A function can have up to 255 arguments

Function body goes here

Function Definition: Function statement example

function addNumbers(num1,num2) {
var result = num1+num2;
return result;
}


Function expression -->
 var addNumbers = function(a,b) {
 var result = a + b;
 Console.log("Sum = " + result)); --> function definition
 }

 addNumbers(11,22); -- 

 output 
 sum = 33


 Function definition: Arrow functions

 Arrow functions are anonymous 
 provides a newer way of defining functions
 was introduced in ES6
 They reduce the amount of code

 Syntax

 ([param [,param ]]) => {
 statements
 }

Arrow Functions

FUNCTION EXPRESSION

var addNumbers = function(num1,num2) {
return (num1+num2);
}

Arrow function

var addNumbers = (num1,num2) => num1+num2

FUNCTION STATEMENT VS FUNCTION 
EXPRESSION VS ARROW FUNCTIONS
Function Statement                   

Defined using function keyword, 
followed by function name, a list of 
parameters (param1, ..., 
paramN) and a pair of curly 
braces {...} that contains the function 
body.

function add(a, b) {
return (a+b);
}

Function Expression

A function expression is defined 
using function keyword, followed by a 
list of parameters in a pair of 
parenthesis (param1, ..., paramN) and 
a pair of curly braces { ... } .
add = function (a, b) {
return (a+b);
}

Arrow Functions

An arrow function is defined using a 
pair of parenthesis that contains the 
list of parameters (param1, ..., 
paramN), followed by a fat arrow => 
and a pair of curly braces {...} .
• When the function has only one 
parameter the parenthesis can be 
omitted.
• The curly braces can be omitted if 
the function contains only a single 
statement.
• this refer to the values of this in 
the environment the arrow function 
is defined.
var add = (a, b) => (a+b)

 FUNCTION STATEMENT VS FUNCTION 
EXPRESSION VS ARROW FUNCTIONS

Function Statement  

The function variable is hoisted up 
to the top of the current scope, 
which means that the function can 
be invoked before the declaration
var x = add(10,20); 
function add(a, b) {
return (a+b);
}
console.log("SUM = "+x);
The above code works


Function expression
Functional expressions are not 
hoisted to the top, so they can 
only be executed, if they have 
already been loaded into the 
context.

var x = add(10,20); 
add = function (a, b) {
return (a+b);
}
console.log("SUM = "+x);
The above code does not work



Arrow Functions are not hoisted to 
the top, so they can only be 
executed, if they have already 
been loaded into the context.



Arrow Functions
var x = add(10,20); 
var add = (a, b) => (a+b);
console.log(“ SUM = “ +x);
The above code does not wor

IMMEDIATELY INVOKED FUNCTION 
EXPRESSION ( IIFE )

Function expressions can be invoked right away by having a 
pair of parentheses at the end.
This pattern is called as “Immediately Invoked Function 
Expression(IIFE)”

IMMEDIATELY INVOKED FUNCTION 
EXPRESSION ( IIFE ) 
Example:
( function (){
console.log("**********Function 1 Executed *************“);
})();
Output:
**********Function 1 Executed************

IMMEDIATELY INVOKED FUNCTION 
EXPRESSION ( IIFE )
Any variable declared within the IIFE cannot be accessed by the 
outside world
Example:
(function () {
var company = "Accenture";
// Outputs: "Accenture"
console.log(company);
} ) ();
// ReferenceError: company is not defined
console.log(company);

IMMEDIATELY INVOKED FUNCTION 
EXPRESSION ( IIFE )  -- IFEE can take arguments
Example:
(function (num1,num2)
{
var sum = num1 + num2;
console.log("**********Function 1 
Executed*************");
console.log("SUM = "+sum);
})(10,20);

IFEE can take arguments
Output:
**********Function 1 Executed*************
SUM = 3

Summary
• Functions definition and its type. 
• Function Statement, expression
arrow
• Difference between statement, 
expression and arrow
• Immediately Invoked Function 
Expression.

Object oriented 
JavaScript

• Understand JavaScript Objects 
• Create objects using different methods


AGENDA
►Object Oriented Programming in JavaScript
►Objects in JavaScript. 
►Built-in objects
►Custom objects 
►Creating an object
►Using constructors function

Object Oriented JavaScript
• JavaScript supports creation of object 
oriented applications.
• It supports the key OO concepts.

Object
• Objects are entities that serve as the basic 
building blocks of an object-oriented 
programming (OOP) application.
• They have their own properties and 
attributes and can be grouped into 
categories.
• Since program entities often describe realworld entities, the object-oriented approach 
makes designing applications much easier.

Objects in JavaScript.
• JavaScript can be used to create objects.
• It uses a prototype based programming approach
• Prototype-based programming is a style of object-oriented programming in which classes are 
not present, and behavior reuse is accomplished through a process of decorating existing 
objects which serve as prototypes
• Objects in JavaScript can be classified into two types.
1) built-in objects
2) Custom objects

Built-in objects 
• Built-In objects are pre-existing objects
▪ Examples: Object, String, Array, RegExp, Date, Math etc. 
• These Objects can be instantiated and used in JavaScript without having to create a class. 
• Once these are instantiated using the new operator all its pre defined properties and member 
functions can be invoked .

var currentDate = new Date();
console.log("Current Year is : “ + currentDate.getFullYear() );
OUTPUT
Current Year is : 2017

“ this ” Keyword
• Global Context 
• In the global execution context this refers to the global object. In web browsers window is a global object
• Function Context 
• In a function execution context the value of this depends on how the function has been called.
• Common Functions
• The value of this depends on how the function is called.
• Arrow Functions
• The value of this depends on the enclosing lexical context's
• Object Method
• this is set to the object the method is called on.
• Constructor Function
• If a function is used as a constructor its this is bound to the new object being constructed.

this keyword in JS behaves a little differently
compared to other languages.

Custom Objects
• Unlike other Object Oriented Programming Language like C++, C#, Java, etc., which uses a 
‘class’ keyword to create Objects, JavaScript does not provide a class keyword. 
• JavaScript provides multiple ways of defining an object. They can be defined using
– Object literal
– Use Object constructor
– Constructor functions


Object 
Literal , Constructor 
functions,Object 
constructor ------------->    JavaScript 
provides multiple 
ways of defining 
an object. They 
can be defined 
using

Create Objects : Object Literal
• Literals are shorter way to define objects which allows creation of instance immediately.
• The objects created using literal notation are singletons

var emp1 = {
empNo : 1231,
empName : “John",
displayEmployeeDetails : function ()
{
return "Emp No = “ + this.empNo + "\n" + "Emp Name = “ + this.empName;
}
};
console.log("\n\n\nEmployee Details\n“ + emp1.DisplayEmployeeDetails() );
Output
Employee Details
Emp No = 1231
Emp Name = John

Create Objects : Object Constructor
• The Object() constructor can be used to create a new object.
• It generates an empty object.
• Use the dot (‘ . ‘) operator to add newer properties and methods.
• To create an object use the new keyword.

var employee1 = new Object(); //Object Created
employee1.empNo = 1231;
employee1.empName = ‘John’ ;
employee1.displayEmployeeDetails = function ()
{
return "Emp No = “ + this.empNo + "\n“ + "Emp Name = “ + this.lastName;
}
console.log("\n\n\nEmployee Details\n“ + employee1.DisplayEmployeeDetails() );

Create Objects : Constructor 
Functions

• The constructor are methods in a class which initialize an object
• In JavaScript, the function serves as the constructor of the object; therefore, there is no need to 
explicitly define a constructor method. 
• Every action declared in the class gets executed at the time of instantiation.


function Employee(empNo, empName)
{
this.empNo = empNo;
this.empName = empName;
this.displayEmployeeDetails = function ()
{
return "Emp No = “ + this.empNo + "\n" + "Emp Name = “ + this.lastName;
}
}
var emp1 = new Employee("1231", "Accenture"); //Object Created
console.log("==============Employee Details======================");
console.log("Employee No = "+emp1.empNo);
console.log("Employee Name = "+emp1.empName);
console.log("\n\n\nEmployee Details\n"+emp1.displayEmployeeDetails());
Output
==============Employee Details======================
Employee No = 1231
Employee Name = Accenture
Employee Details
Emp No = 1231
Emp Name = undefined

Introduction ES6
INTRODUCTION TO ES6 (ECMA SCRIPT6)
ES6 is also known as 
ES2015
Is the latest javascript 
specifications.
Developed by a company 
ECMA
Released in June 201

NEW FEATURES OF ES6
Lexical scoping using let and 
const keywords 
Classes and Inheritance
Arrow function
Default value for function
Destructuring 
Spread operator

ES6 NEW FEATURE - VARIABLE
There are two new keywords 
which would be used to declare 
variables
let 
Used when variable should 
be scoped within the block

Syntax: let variable = value

const
Used when variable should 
be scoped within the block
Used to create constant 
variables scoped within the 
block
Syntax : const variable = value

DEMO - LET 
index.js

function display() {
let oldvalue = 10;
if(oldvalue <= 5) {
let newValue = 10;
document.write('old value of a variable='+oldvalue);
document.write('New value of a variable='+newvalue);
}
else
{
document.write('old value of a variable='+oldvalue);
document.write('New value of a variable='+newvalue);
}}
display();

new value only accessible in if function and it is not accessible in else function

DEmo - let
function display() {
let radius = 30;
const PI = 3.14;
if(oldvalue <= 5) {
const newValue = 10;
document.write('old value of a variable='+oldvalue);
document.write('New value of a variable='+newvalue);
}
else
{
document.write('old value of a variable='+oldvalue);
document.write('New value of a variable='+newvalue);
}}
display();

const value is not accessible in else block

ES6 NEW FEATURE – CLASS AND INHERITANCE
Class in ES6 can be created using 
“class” keyword
Class definition can include 
constructor and methods
Class definition in ES6 cannot have 
data properties directly in the class 
body, however these can be inside 
constructor

Syntax
class Classname
{
constructor() {
data properties;
}
method() { 
}
}

Instantiation 
let obj=new Classname(); 





Demo - class
class Employee {

constructor(name,age) {
this.name = name;
this.age = age;
}

displayEmployee() {
console.log('Employee Name = ' + this.name);
console.log('Employee Age = ' + this.age);
}
}
let obj = new Employee('Mack',27);
obj.displayEmployee();


ES6 NEW FEATURE – CLASS AND INHERITANCE

Inheritance in ES6 can be achieved 
using “extends” keyword
Inheritance is a concept of creating new 
class using existing class definition
 
The main class is referred as “parent or 
super” class and the newly created 
class is referred as “child or sub” class
The sub class can inherit data and 
methods from the super class
The sub class cannot inherit constructor 
from the super class
Whenever there is need to invoke 
parent class members, this could be 
achieved using “super” keywor

Syntax
class Parentclassname
{
constructor() {
data properties;
}
method() { 
}
}
class Childclassname extends Parentclassname{
constructor() {
data properties;
}
method() { 
}
}
Instantiation 
let obj=new Childclassname();

DEMO – CLASS INHERITANCE


class Employee  {
constructor(name,age) {
this.name = name;
this.age = age;
}
displayEmployee() {
console.log('Employee   Name = ' +  this.name);
console.log('Employee age = ' + this.age);
} }
class AccentureEmployee extends Employee {
constructor(name,age,sapNum) {
super(name,age);
this.sapNum = sapNum;
}
displayEmployee() {
onsole.log('Employee   Name = ' +  this.name);
console.log('Employee age = ' + this.age);
console.log('Employee sapNum = ' + this.sapNum);
} } 

let obj = new AccentureEmployee('Mack',27,102423423);
obj.displayAccEmployee();

super keyword is used here to invoke base class constructor

ES6 NEW FEATURE – ARROW FUNCTION

ES6 provide this type of arrow “=>” 
which is also known as “Fat” Arrow 
Benefit of using fat arrow is, it will 
shorten the code with respect to 
function body

Variable or 
function name
= () =>
Calculate and 
return value
let result = () => 2+3


Syntax Right side of fat arrow is used 
to either calculate or return 
some value and left side of fat 
arrow will capture the returned 
or calculated value

ArrowFunction Or FAT Arrow

let helloFunction = function() {
console.log('hELLO FROM FUNCTION');
}
helloFunction();


let helloFunction = () => {
console.log("Hello from function")
}

Function keyword is not used

DEMO – ARROW FUNCTION WITH ARGUMENTS

let Total = function(a,b,c) {
return a+b+c;
}
console.log(Total(4,5,6));

Same function when created using Arrow function
let Total = (a,b,c) => a+b+c;

console.log(Total(2,3,4));

ES6 NEW FEATURE – DEFAULT VALUE IN 
FUNCTION
Function can have parameters, but 
some parameters may have default 
value assigned
Function can have parameters, but 
some parameters may have default 
value assigned
Syntax
function function_name(arg1,arg2=defaultValue)

DEMO – DEFAULT VALUE IN FUNCTION

function sum(a,b=20) {
return a+b;
}
console.log(sum(2,4)); --> sum of 2 numbers = 6;


Demo - default value in function

function sum(a,b=20) {
return a+b;
}
console.log(sum(10))
output -> 20


ES6 NEW FEATURE – DESTRUCTURING 
Destructuring is a way of unpacking 
the values. It could be from array or 
returned value from a function etc.
Unpacked elements could be 
assigned to other variables
Syntax
var Variable_name= array[elements]


DEMO – DESTRUCTURING
let days = ['Monday','Tuesday','Wednesday'];
let [firstDay,secondDay] = days
console.log(firstDay);
console.log(secondDay);

Elements from array(days) are 
unpacked and assigned to 
individual variables(firstDay
and secondDay). This is 
known as Destructuring

DEMO 2 – DESTRUCTURING WITH RETURNED 
VALUE FROM FUNCTION 
index.js

let result = function() {
return ([(2+7),(2*3)])
}
let [sumOfNumber,multOfNumber] = result();
console.log(sumOfNumber);
console.log(multofOfNumber);


Spread Operator

This operator is used expand or spread the values into different arguments
It can represent zero or more atrguments based on the program logic


Demo -- spread Operator

let listOfAnimals = ['Lion','Tiger','Elephant'];
let zoo = ['Birds', ...listOfAnimals];

console.log(zoo);

spread operator  is used here which will expand or spread elements of listofElements array.
['Lion','Tiger','Elephant'}

DEMO 2 – SPREAD OPERATOR

let listofAnimals = ['Lion','Tiger','Elephant'];
let birds = ['peacock','pigeon','Parrot']
let zoo = [...birds,..listofAnimals];
console.log(zoo);

spread operator in function Argument

let params = [2,3,4]
function calculateTotal(num1,num2,num3) {
return num1+num2+num3;
}
console.log((...params));


Understand Node.js as a server-side JavaScript runtime
List the features of Nodejs

javascript runtime for high-performance , low latency applications,powering 
everything from enterprise applications , robots ,API engines ,cloud stacks ,
IoT,and mobile websites

It uses an event-driven , non-blocking I/O  model it lightweight ,effecient and highly performant under extreme load

Reasons to use NODEJs

it is very lightweight and fast 
fast implementation
Lots of modules available for free
Good fit for real-time applications
javascript end to end
Event-driven scalability
Extensibility
Works well NOSQL


How the single threaded non blocking IO model works in NodeJS ?
Last Updated : 05 Feb, 2021
Node.js is a JavaScript runtime environment that runs on the Chrome V8 engine and is used for server-side scripting. It takes requests from users, processes those requests, and returns responses to the corresponding users.

Some important Node.js features are:

It is based on single-threaded architecture: Since node.js gets multiple requests from multiple users it executes one command at a time. Due to this it can handle concurrent client requests very effectively and has good performance.
It uses an event-driven non-blocking-based IO model: Whenever the node server is started, it initiates certain variables and functions and then waits for events to occur, whenever an event is detected a callback function is assigned to that particular event. Event-driven architecture makes the server highly scalable and it does not wait for an API to return data, it moves to the next API immediately for the next request. Non-blocking operation means the server will not block itself for one request. Non-blocking call only initiates the operation and the response is provided later, meanwhile, it can continue with other client requests.
Example: If we get requests from two users A and B. With non-blocking IO we can initiate the request for A and then immediately for B without waiting for the response to the request of A. Hence we can say with the help of non-blocking IO we can eliminate the use of multi-threading since the node server can handle multiple requests simultaneously.

Working of single-threaded non-blocking IO:



When the client sends a request to the server, this request is called an event. These all requests get stored in an event queue. The single thread present in the event loop assigns this request to one of the threads present in the internal thread pool.
This thread reads the client request, processes the request, performs any blocking IO operations if needed, and prepares the final response to be sent back to the server. The event loop sends this response back to the respective client.
The event loop infinitely receives requests and processes them.
There is no need for multiple threads because of Event Loop. Because of this event loop and concept of single threading, node.js uses lesser resources and memory.
Reference: https://www.geeksforgeeks.org/introduction-to-nodejs/


Never before seen offer on GeeksforGeeks Courses! Get up-to 75% off on all premium courses such as Full Stack Web Dev, Backend Dev, DSA for Interview and more. Avail discount now!
Want to be a Software Developer or a Working Professional looking to enhance your Software Development Skills? Then, master the concepts of Full-Stack Development. Our Full Stack Development - React and Node.js Course will help you achieve this quickly. Learn everything from Front-End to Back-End Development with hands-on Projects and real-world examples. This course enables you to build scalable, efficient, dynamic web applications that stand out. Ready to become an expert in Full-Stack? Enroll Now and Start Creating the Future!

Features 

single threaded
Non blocking 
fast
event driven
Asynchronous

Architeture
javascript --> node standered library
C/C++ --> Node Bindings
        (socket,http,file system,etc)

        chrome V8(js engine)
        Async I/O (libuv)
        Event loop (libuv)


  Libuv

  libuv is a high performance evented I/O library
  It enforces an asynchronous,event-driven style of programming
  It core jobs is to provide an event loop and call back based notifications of I/O and other activites
.offers core utilites like timers,non-blocking networking support,aysnchronous file system access,child process etc
Projects that use libuv  are Luvit,julia,pyuv and others

javascript v8 engine

V8 engine is an open source high-performance javascript
engine developed by chromium project for the google chrome web browser
It is written in C++.
It compiles and executes JavaScript source code, handles memory 
allocation for objects, and garbage collects objects it no longer need


Performance
Under high load (high concurrency), Node.js maintains high throughput 
and low latency
• At least three factors contribute to Node.js’s high performance:
1. V8 JavaScript engine, upon which Node.js is based, is highly 
optimized for performance by Google
2. Node.js events are lightweight, while threads are heavyweight. 
Consequently, Node.js is inherently more performant under load
3. Node.js is container-ready, which simplifies the move to cloud and 
microservices architectures

potential Node.js Application Areas

media 
Social media
Ecommerce
Enterprise web apps
Bckend/Api for mobile apps
payment gateways

use case 

netflix --> node.js makes it easy to implement features end to end 
reducing context switches and handsoff between frontend,backend and IOT

prior to replacing java with node.js on the server side, the netflix UI team had to write many times and maintain seperate toolchains

PROS 
• Asynchronous event driven IO helps 
concurrent request handling.
• It's great to have common language on 
both client and server.
• NPM, the Node packaged modules 
have already become huge, and still 
growing.
• Clean, Functional API.
• Active and vibrant community, with 
lots of code shared via github, etc.
• Can stream big files.

CONS
• Any CPU intensive computation will 
block Node.js responsiveness, so a 
threaded platform is a better 
approach. 
• Every time using a callback ends up 
with tons of nested callbacks.
• Using Node.js with a relational 
database is still quite a pain. Pick up 
any other environment like Rails, 
Django, or ASP.Net MVC if trying to 
perform relational operations


Verify installation and node installation using
..)node –version and npm --version  Node.js provides with a REPL (readevaluate-print-loop) 
► Test arbitrary JavaScript and 
experiment and explore solutions to the 
problem.
► At each step, the REPL prints the 
outcome of the last statement executed. 
► The REPL does not execute input code 
until all brackets have been balanced.

REPL COMMANDS
► .break - When in the process of inputting a multi-line expression, entering 
the .break command (or pressing the <ctrl>-C key combination) will abort 
further input or processing of that expression.
► .clear - Resets the REPL context to an empty object and clears any multi-line 
expression currently being input.
► .exit - Close the I/O stream, causing the REPL to exit.
► .help - Show this list of special commands.
► .save - Save the current REPL session to a file: > .save ./file/to/save.js
► .load - Load a file into the current REPL session. > .load ./file/to/load.js
► .editor - Enter editor mode (<ctrl>-D to finish, <ctrl>-C to cancel

var date=new Date().getHours();
console.log(date +':00 is a good time to learn

Understand that Node.js is a JavaScript runtime primarily used for creating scalable network 
application

 Modules types
 ► Core modules 
 o fs module 
 o util module 
 o process modules 
 o cluster modules
 ► Publishing the package
 
Modules are node libraries that helps us to use code of one file as part of another file.
► Module then acts as an api injected in to the bootstrap file.
► A module encapsulates related code into a single unit of code. 
► When creating a module, this can be interpreted as moving all related functions into a 
file. 
► Node modules run in their own scope so that they do not conflict with other modules. 
Node relatedly provides global access to help facilitate module interoperability. 
► Node.Js has a simple module loading system. In node.Js, files and modules are in one-toone correspondence (each file is treated as a separate module).
require is an importer of 
code from other locations
exports bundles the code 
in an object and allows it 
to be reused

const readline = require('readline'); 

Importing read line module to read 
input from console

const prompt = readline.createInterface({
 input: process.stdin,
 output: process.stdout
});
interface for reading data from a stream one 
line at a time

prompt.question('What do you think of Node.js? ', (answer) => {
 console.log(‘Thank you for your valuable feedback:’+ answer);
 A statement or query to write to output, prepended to 
the prompt and a callback function that is invoked 
with the user's input in response to the query.

prompt.close();
});
readline.Interface is closed because the interface 
waits for data to be received on the input stream.


$ node readline_demo.js
What do you think of Node.js? good
Thank you for your valuable feedback: good























        


























