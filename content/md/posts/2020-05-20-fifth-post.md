{:title "Functional programming explained. Higher order functions"
:layout :post
:tags ["Higher order functions", "Functional programming"]}

>     If debugging is the process of removing software bugs, then programming must be the process of putting them in. - Edsger Dijkstra

<div style="text-align: justify">
What is a **higher order function(HOF)**?  If a function receives as its input one or more functions or/and returns the function we can called it HOF. On the contrary, a single order function does not receive the function as an input. Functions that are passed as an argument to another function are what we refer to as **callback functions.** Functions in JavaScript are variadic, that means that you can pass more or less arguments then is specified to the function and it still will run.<br/> 
You as a **functional programmer** should be comfortable making your own higher order functions. When you see two pieces that are not completely fit together you should be able to write an adapter/utility function to make them work jointly.<br/>
We can take function that expects multiple parameters and reduce it shape to receive only one parameter, unary. Function that has one shape can be adapted to have another one. An example could be a "flip" HOF that receives another function, flips its parameters and returns it with parameters flipped. Another possible implementation would a "reverse" HOF that receives a function, reverse its parameters, and returns it with parameters reversed.<br/> 
It is a good practice to get yourself familiar with existing functional programming libraries and tools and use patterns that are familiar to a larger community of programmers. That helps readability of your code. But when you can’t, make your own, document it well and make it available to others to use.
</div>
