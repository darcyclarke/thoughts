# "Functions" vs. "Methods" in JavaScript...

```javascript
function foo () {};
````

`foo` is a **"function"** in the typical sense. `foo` also happens to be a **"method"**.

### "How can this be?" you might ask...

Semantically, the only difference between a **"method"** and a **"function"** is that a **method** is defined as being associated with an **"object"** where it derives/inherits data/attributes. This is also where the term *"Object-Oriented Programming"* is derived; From there you can start to understand the differences between *"classical"* and *"prototypal"* *inheritence* (but that's a whole other thought, I digress...).

### Now the fun part...

Although not explicit, in JavaScript, any **variable** or **function** *declaration* (ie. `var ...` or `function ...`), found in the *global scope* gets hoisted, **automagically™**, and bound to the `window` object.

### See for yourself...

```javascript
function foo () {};
console.dir(window);
console.dir(window.foo);
console.log(window.foo === foo); // operation to show strict equality, 'cause I wanted to
````

> **Note:** This only happens when `window` is the *global scope*. If you're scratching your head, it's valid. There are actually instances where you'll find that `window` is not the *global scope*. A good example of this would be when you inject one web page into another using an `iframe`. The `window` object of the code running inside the `iframe` is no longer the *global scope*. **Huzzah!** *[The more you know...](https://www.youtube.com/watch?v=GD6qtc2_AQA)*

### So you're telling me...

So, what this means is that `foo` derives/inherits from the `window` object... and is, therefore, both a **"function"** and a **"method"**
### And this means...

And this means that the next time someone asks you whether `x` is a **"function"** or a **"method"**, feel free to retort *how pedantically misguided that question is - you cheeky developer you! :wink:*
