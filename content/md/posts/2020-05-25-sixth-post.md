{:title "Functional programming explained. A value mutability"
:layout :post
:tags ["Value mutability", "Functional programming"]}

>     Programming is like sex. One mistake and you have to support it for the rest of your life. - Michael Sinz

<div style="text-align: justify"> 
**Mutating a value**. When you receive a data structure that is in its identity **mutable**, like an array or object, the best thing to do is to always assume that it is a read-only data structure and that you are not allowed to mutate it. Make a copy of the object/array (ex. spread operator) and then mutate it locally, so you don’t create a **side effect** on the outside program.<br/>
**Preventing a value mutation**. If you are calling a function and you are going to pass to it a data structure like an array or object, make it clear to the reader that you don’t want it to be changed. Use something like Object.freeze method in JavaScript. Create a helper function that you can use to **“freeze”** an object so no new properties can be added, changed or removed.
</div>
