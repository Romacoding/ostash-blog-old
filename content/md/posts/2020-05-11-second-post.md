{:title "A note to myself #1"
:layout :post
:tags ["JavaScript", "Functional programming", "Pure functions"]}

### Functional purity in JavaScript

>     Object oriented programming makes code understandable by encapsulating moving parts. Functional programming makes code understandable by minimizing moving parts. – Michael Feathers

What is a function? For the function to be a function it has to return something, otherwise is a procedure. Function is the semantic relationship between input and computed output.
In a JavaScript we cannot completely sure if a function is pure unless we look on how the function was called.<br/>
Every time we execute the pure function with same inputs we absolutely and positively know that it will always return the same output. We want our function calls to behave as pure: every time we give it a same input we expect to receive the same output. The function call needs to avoid using side effects.<br/>
Impurity is about side effects. Minimize them. They impurify functional programming. Avoid them where possible or make them obvious in your code. How, you would ask? By taking away the impurity and writing a pure function that does computations and then a procedure to do the rest.<br/>
The degree of functional purity in JavaScript shows in how confident a programmer is in function’s behavior. Higher degree of confidence relates to the higher level of purity in the function.<br/>
Making pure functions might not always be possible or practical but we should strive to extract impurity (side effects) and leave functions as pure.
It is possible that for whatever reason we cannot change or modify the impure function. Another option would be to contain the impurity so it doesn’t leek out to the rest of the scope.<br/>
We can do that by wrapping an impure function inside a pure function. By doing that we reduce the surface area of that impurity and improve the overall program readability and maintainability.

To be continued…
