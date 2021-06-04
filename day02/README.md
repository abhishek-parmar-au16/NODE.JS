<h2>What is a Module in Node.js?</h2>
Consider modules to be the same as JavaScript libraries.

A set of functions you want to include in your application.

Built-in Modules
Node.js has a set of built-in modules which you can use without any further installation.

Look at our Built-in Modules Reference for a complete list of modules.

Include Modules
To include a module, use the require() function with the name of the module:

-->var http = require('http');


Create Your Own Modules
You can create your own modules, and easily include them in your applications.

The following example creates a module that returns a date and time object:

Example
Create a module that returns the current date and time:

-->exports.myDateTime = function () {
-->  return Date();
-->};
Use the exports keyword to make properties and methods available outside the module file.

Save the code above in a file called "myfirstmodule.js"