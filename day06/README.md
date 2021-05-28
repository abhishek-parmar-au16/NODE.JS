<h3> Differentiate between callback functions and anonymous function. Give an example of both</h3>


Callback and Anonymous functions are used for passing to other functions like Array.prototype.map() 
for them to use. It’s a way to pass logic just as you would pass an object. Consider the example code below;

var Arr = [2,3,4,5]
<h4>Callback function</h4>
-->function myCallback(x){
--> return x+1;
-->}
-->console.log(Arr.map(myCallback));

From the code sample above, our callback function is myCallback() , 
which simply takes an argument x and returns an increment of the argument x+1. We see that our Array.prototype.map() takes as argument our callback function.
We could also write it as:

var Arr = [2,3,4,5]

<h4>Anonymous function goes directly</h4> 
-->console.log(Arr.map(function(x){ return x+1}));

The code above will also do the job, it uses an anonymous function. I.E, a 
function without a name function(x){return x+1}. Anonymous functions as the name might imply are 
functions without names. The function is only refered to once, so a variable name doesn’t need to be wasted on it.

The difference between anonymous and callback function is that;

1-Anonymous function doensn’t need to be named, while calback functions are named

2-Anonymous functions can’t be used anywhere outside the .map() function while callback functions are
 independent and can be used outside of .map() function above.

3-With anonymous functions, it is difficult to identify in call stacks, which makes debugging trickier.
 While with callback functions, there are identify in call stacks and easy to debug.

4-Callback function doesn’t take in an argument when called within another function while anonymous function can take in arguments.
