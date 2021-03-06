# "Functions" vs. "Methods" in JavaScript...

```javascript
function hello(name) {
  return `Hello ${name}!`
}
````

`hello` is a **"function"** in the [typical sense](https://www.cs.utah.edu/~germain/PPS/Topics/functions.html). `hello` also happens to be a **"method"**.

### "How can this be?" you might ask...

Semantically, the only difference between a **"method"** and a **"function"** is that a **method** is defined as being associated with an **"object"** where it inherits data. This is also where the term *"Object-Oriented Programming"* is derived ([you can read more on wikipedia](https://en.wikipedia.org/wiki/Method_(computer_programming))); From there you can start to understand the differences between *"classical"* and *"prototypal"* *inheritence*, but that's a whole other discussion, and I digress... 

**tldr;** if you get nothing else from this, just know that... it's all **semantics** 😑

### Now the fun part...

Although not explicit, in JavaScript, any **variable** or **function** *declaration* (ie. `var ...` or `function ...`), found in the *global scope* gets hoisted, **automagically™**, and a reference is bound to the `window` object. Furthermore, your definition *inherits* properties from it's corresponding type, such as `Function`, which ultimately *inherits* properties from the base `Object`.

**See hoisting & inheritence in action...**

```javascript
console.dir(hello)
console.dir(window.hello) // show hoisting
console.log(window.hello === hello) // show strict equality, just 'cause
console.dir(hello.constructor.prototype) // show prototypal inheritence from `Function`
console.log(hello.constructor.prototype === Function.constructor.prototype) // show strict equality, just 'cause
````

> **Note:** Hoisting objects to `window` only happens when it is the *global scope*. If you're scratching your head, it's valid. There are actually instances where you'll find that `window` is not the *global scope*. A good example of this would be when you inject one web page into another using an `iframe`. The `window` object of the code running inside the `iframe` is no longer the *global scope*. **Huzzah!** *[The more you know...](https://www.youtube.com/watch?v=GD6qtc2_AQA)*

### So you're telling me...

So, what this means is that `hello` derives/inherits from a base type object... and is, therefore, both a **"function"** and a **"method"**. That said, there's a ton more you should read about [hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting), [context/closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this) & [inheritance](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Inheritance).

### But ultimately, this means...

And this means that the next time someone asks you whether `x` is a **"function"** or a **"method"**, feel free to retort *how pedantic & insignificant that question is - you cheeky developer you! :wink:*
