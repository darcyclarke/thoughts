# thoughts...

they are my own... if that's not glaringly obvious...

## "Functions" vs. "Methods" in JavaScript

```javascript
function foo () {};
````

`foo` is a **"function"** in the typical sense. `foo` also happens to be a **"method"**.

### "How can this be?" you might ask. 

Semantically, the only difference between a **"method"** and a **"function"** is that a **method** is defined as being associated with an **"object"** where it inherits data/attributes. This is where the term *"Object-Oriented Programming"* is derived; From there you can start to understand the differences between *"classical"* and *"prototypical"* *inheritence* (but that's a whole other thought, I digress...). 

#### Now the fun part...

Although not explicit, in JavaScript, any **variable** or **function** *declaration* (ie. `var ...` or `function ...`), found in the *global scope* gets hoisted, automatically, and bound to the `window` object* **like magic!**

#### See for yourself...

```javascript
console.dir( window );
console.dir( window.foo );
console.log( window.foo === foo ); // operation to show equality
````

> * **Note:** This only happens when `window` is the *global scope*. If you're scratching your head, it's valid. There are actually instances where you'll find that `window` is not the global scope. A good example of this would be when you inject one web page into another using an `iframe`. The `window` object of the code running inside the `iframe` is no longer the global scope. Huzzah!

#### So...

So, what this means is that `foo` derives/inherits from the `window` object... and is both a **"function"** and a **"method"**   
#### And...

And the next time someone asks you whether `x` is a **"function"** or a **"method"**, feel free to explain *how pedantically incorrect that sentiment is - you cheeky developer you! :)*.
