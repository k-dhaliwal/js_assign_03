closure is a kind of  inner function  which can access to the   function variable which we  declare inside(local variable- which are only define within the  function body)

useable only in that function or outside (global variable-their defination outside the mainfunction and accessed by all function ) from the  the main function.

This inner function has access to not only outer function's variables but also  to their outer  function's  parameters.however, it can call the outer function 
parameters directly.
properties:
closure can make code more compact,concise ,readable and enhance the functional resuseability.
 -closures  are functions that refer to  independent variables
 -environment dependent



for example
  
  
  function showname(firstname,lastname)   // this is a function 
   {
   var nameIntro= 'your name is ';  //inner function has access to the outer function's variables including parameters
   
   function makefullname()   // another function within a function
   {
       return nameIntro+ firstname+" "+ lastname(); }
       return makefullname();
       }
       showname("kamal","dhaliwal");
       
   
 
   
  links
  
   https://javascriptweblog.wordpress.com/2010/10/25/understanding-javascript-closures/
   http://www.w3schools.com/js/js_function_closures.asp
   https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures