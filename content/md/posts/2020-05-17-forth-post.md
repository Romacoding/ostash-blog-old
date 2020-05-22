{:title "Functional programming explained. Currying"
:layout :post
:tags ["Currying", "Functional programming"]}

>     Don’t worry if it doesn’t work right.  If everything did, you’d be out of a job. - Mosher’s Law of Software Engineering

<div style="text-align: justify">
**Currying** is an act of taking one function that receives more than one argument and refactoring it so it becomes **HOF**(a higher order function) that returns series of functions each accepting only one argument and only evaluating once we receive our final argument.<br/> 
The act of currying can be described as taking a multiary function and turning it into series of unary functions. Currying allows you to take an existing function that has one shape and specialized it in producing a new function that is more adapted to your needs and has a shape that you want.<br/> 
Functional programmers want everything to be currying because they like all functions to be unary, single input single output. All functional libraries methods that you will encounter are automatically doing currying under the hood.
</div>
