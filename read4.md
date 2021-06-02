# Dictionary
### - 1 - JavaScript
### - 2 - User Input and Output in JavaScript
### - 3 - What are Variables in JavaScript?


  ----------------
## what is JavaScript

JavaScript (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions. While it is most well-known as the scripting language for Web pages, many non-browser environments also use it, such as Node.js, Apache CouchDB and Adobe Acrobat. JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles. Read more about JavaScript.

This section is dedicated to the JavaScript language itself, and not the parts that are specific to Web pages or other host environments. For information about API specifics to Web pages, please see Web APIs and DOM.

The standards for JavaScript are the ECMAScript Language Specification (ECMA-262) and the ECMAScript Internationalization API specification (ECMA-402). The JavaScript documentation throughout MDN is based on the latest draft versions of ECMA-262 and ECMA-402. And in cases where some proposals for new ECMAScript features have already been implemented in browsers, documentation and examples in MDN articles may use some of those new features.

Do not confuse JavaScript with the Java programming language. Both "Java" and "JavaScript" are trademarks or registered trademarks of Oracle in the U.S. and other countries. However, the two programming languages have very different syntax, semantic, and use.
  ----------------

## User Input and Output in JavaScript

Working with any dynamic language requires the ability to read, process and output user data. JavaScript is especially useful when you want to take user information and process it without sending the data back to the server. JavaScript is much faster than sending everything to the server to process, but you must be able to read user input and use the right syntax to work with that input.  This article will focus on retrieving user input and displaying it on the screen through HTML elements or prompts. 

Displaying Prompts and Retrieving User Responses

JavaScript has a few window object methods that you can use to interact with your users. The prompt() method lets you open a client-side window and take input from a user. For instance, maybe you want the user to enter a first and last name. Normally, you can use an HTML form for user input, but you might need to get the information before sending the form back to your server for processing. You can use the window.prompt() method for small amounts of information. It's not meant for large blocks of text, but it's useful when you need information before the user continues to another page.

The following code is an example of the window.prompt method. 

var customerName = prompt("Please enter your name", "<name goes here>");

if (customerName!= null) {

    document.getElementById("welcome").innerHTML =

    "Hello " + customerName + "! How are you today?";

}

  ----------------

### What are Variables in JavaScript?

What are Variables in JavaScript?
* Variables as the name suggest are anything whose values vary.
* You can assume a variable as a container or box which is used to hold values.
* A JavaScript variable is a name given to a memory location that is used to store values.
 *Memory is allocated to a variable used in the program and is given some name.

 ----------------
@ Anas Ahmad 