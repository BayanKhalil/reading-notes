# error handling and debugging

in JS you aloways make wrong steps by mistake and theres aways that can help you to find these errors
 at the first how js work :
  its work as the concept of STACK which it's read one line of code at atime.
  and when when it need any data fromany other function it stack the function on the top.and for the error If a Js statement generates an error, then it throws an exception at that point, the interpreter stops and looks for exception-handling code.

  you can deal with errors by :
  1. debug the script
  2. handle errors by Throw and Try to Catch.
    * The try statement lets you test a block of code for errors.

    * The catch statement lets you handle the error.

    * The throw statement lets you create custom errors.

    * The finally statement lets you execute code, after try and catch, regardless of the result.



 ### Tools
JavaScript console it will tell you when there is a problem with a script,
 where to look for the problem, and what kind of issue it seems to be.
 by using `console.log();` in the code and  you can typing on it whatever the browser you use it and `console.group()`use it to write a set of related data to the console by `console.groupEnd ()`  method at the end of code.`console.table ()` method to output a table.
 * You can pause the execution of a script on any line using breakpoints by  click on line number you want  in source option to stop on and when you run it will stop and You can indicate that a breakpoint should be triggered if a condition that you specify is met by Right-click on a line number,Select Add Conditional Breakpoint,then enter a condition into the popup box.
 * If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them using 
 `throw new Error('message);`