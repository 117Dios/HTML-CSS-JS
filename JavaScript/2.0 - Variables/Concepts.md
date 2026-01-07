# Initializing variables
- ```var```: initialize a variable, and a variable can be re-declared with the same name.

- ```let```: initializes a variable. Throws a SyntaxError if another variable is declared with the same name.

```let``` is the most used.

# Strict interpreter
Always start a JavaScript document with:

```"use strict;"```

So that it behaves according to modern standards.

### Example

Without use strict:

<pre>height  =  180;
console.log(height);  //  ->  180</pre>

With use strict:

<pre>"use  strict";
   
height  =  180;  //  ->  Uncaught  ReferenceError:  height  is  not  defined
console.log(height);
</pre>