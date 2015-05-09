# thoughts...

they are my own... if that's not glaringly obvious...

## "Functions" vs. "Methods" in JavaScript

```javascript
function foo () {};
````

`foo` is a **"function"** in the typical sense. `foo` also happens to be a **"method"**.

### "How can this be?" you might ask. 

Semantically, the only difference between a **"method"** and a **"function"** is that a **method** is defined as being associated with an **"object"** where it derives data/attributes. This is where the term *"Object-Oriented Programming"*; From there you can begin to see and understand the differences between *"classical"* and *"prototypical"* *inheritence*. 

#### Now the fun part...

Although not explicit, in **JavaScript**, any *variable* or *function* *declaration* (ie. `var ...` or `function ...`), found in the *global scope* gets hoisted, automatically, and bound to the `window` object** * **. **Yay MAGIC!**

#### See for yourself...

```javascript
console.dir( window.foo );
console.log( window.foo === foo ); // operation to show equality
````

So the next time someone asks you whether `x` is a **"function"** or **"method"**, feel free to explain how pedantically incorrect that sentiment is.

> **Note:** This only happens when `window` is the gloabl scope. If you're scratching your head, it's valid. There are actually instances where you'll find that `window` is not the global scope. A good example of this would be when you inject one web page into another using an `iframe`. The `window` object of the code running inside the `iframe` is no longer the global scope. Huzzah!

