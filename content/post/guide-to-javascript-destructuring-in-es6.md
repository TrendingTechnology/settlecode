+++
categories = ["Javascript"]
date = 2019-12-14T16:00:00Z
description = "The JavaScript destructuring assignment is a more readable compact and expressive syntax that allows us to destructured values from arrays or properties from objects"
featuredimage = "https://res.cloudinary.com/diqqalzsx/image/upload/v1576400964/content/settlecode/javascript_xs0wig.png"
slug = ""
tags = ["ES6"]
title = "Guide to Javascript Destructuring in ES6"

+++
The JavaScript destructuring assignment is a more readable compact and expressive syntax that allows us to destructured values from arrays or properties from objects, into different variables. JavaScript destructuring was a new addition to ES6 which took inspiration from languages like Python. Let's see a simple example of JavaScript destructuring:

Without destructuring assignment, we need to access the items in an array like this:

    var firstItem = someArray[0];
    var secondItem = someArray[1];
    var thirdItem = someArray[2];
    

With destructuring assignment, it is more concise and readable:

    var [first, second, third] = someArray;
    

As we see in our example above, we can use JavaScript destructuring in so many different ways.

## Object destructuring

Let’s see how we can do object destructuring, starting from the beginning. We use an object literal on the left-hand-side of an assignment expression for object destructuring. Let's start with the basic assignment example.

### Basic assignment

    const user = {
        firstname: 'John',
        lastname: 'Doe',
        nickname: 'jDoe'
    };
    
    // Object Destructuring
    const { firstname, lastname, nickname } = users;
    console.log(firstname, lastname, nickname); // John Doe jDoe
    

We are here using object destructuring syntax to assign values to three variables: `firstname`, `lastname`and `nickname`using the values from their keys on the user object. This is the simplest example of object destructuring. Now let's see more interesting examples of object destructuring.

### Assignment without declaration

We can assign variable value with destructuring without separate from its declaration.

    let a, b;
    
    ({a, b} = {a: 1, b: 2});
    

> Note: It is required to have parentheses ( ... ) around the assignment statement when using object literal destructuring assignment without a declaration.

### Assigning to new variable names

We can also assign property from unpacked object to a variable with a different name than the object property.

    let o = {p: 22, q: true};
    let {p: foo, q: bar} = o;
     
    console.log(foo); // 22 
    console.log(bar); // true
    

In the example above, const {p: foo} = o takes from the object o the property named p and assigns it to a variable named foo.

### Default values

We can also set a default value if the unpacked object value is undefined

    let {a = 10, b = 5} = {a: 3};
    
    console.log(a); // 3
    console.log(b); // 5
    

### Assigning to new variables names and providing default values

A property can be:

* unpacked from an object and assigned to a different variable.
* assigned a default value if the unpacked value is undefined.

    const {a: aa = 10, b: bb = 5} = {a: 3};
    
    console.log(aa); // 3
    console.log(bb); // 5
    

### Unpacking fields from objects passed as a function parameter

    const user = {
      id: 42,
      nickName: 'jdoe',
      fullName: {
        firstName: 'John',
        lastName: 'Doe'
      }
    };
    
    function userId({id}) {
      return id;
    }
    
    function whois({displayName, fullName: {firstName: name}}) {
      return `${displayName} is ${name}`;
    }
    
    console.log(userId(user)); // 42
    console.log(whois(user));  // "jdoe is John"
    

In this example, we unpack the id, nickName, and firstName from the user object and we simply output them with `console.log`.

### Nested object and array destructuring

We can also use nested array destructuring where the item must be an array to use a nested destructuring array literal to assign items to local variables.

    const metadata = {
      title: 'Scratchpad',
      translations: [
        {
          locale: 'de',
          localization_tags: [],
          last_edit: '2014-04-14T08:43:37',
          url: '/de/docs/Tools/Scratchpad',
          title: 'JavaScript-Umgebung'
        }
      ],
      url: '/en-US/docs/Tools/Scratchpad'
    };
    
    let {
      title: englishTitle, // rename
      translations: [
        {
           title: localeTitle, // rename
        },
      ],
    } = metadata;
    
    console.log(englishTitle); // "Scratchpad"
    console.log(localeTitle);  // "JavaScript-Umgebung"
    

### Combined Array and Object Destructuring

There are some cases when we are working with a complex array or object structure and we need to assign values from it to variables. In the next example, we will see that it is possible to combine array and objects in destructuring.

    const props = [
      { id: 1, name: 'Fizz'},
      { id: 2, name: 'Buzz'},
      { id: 3, name: 'FizzBuzz'}
    ];
    
    const [,, { name }] = props;
    
    console.log(name); // "FizzBuzz"
    

## Array destructuring

Array destructuring is very similar to object destructuring. In array destructuring, we use an array literal on the left-hand-side of an assignment expression. Each variable on the array literal maps to the item at the same index on the destructured array. Here is a basic example.

### Basic variable assignment

    const rgb = ['one', 'two', 'three'];
    
    const [red, yellow, green] = rgb;
    console.log(red); // "one"
    console.log(yellow); // "two"
    console.log(green); // "three"
    

Here we have assigned the items in the rgb array to three local variables: red, green and blue using array destructuring. You may notice that every variable is mapped to the item at the same index on the rgb array.

### Assignment separate from declaration

We can assign a variable value via destructuring separate from the variable's declaration.

    let a, b;
    
    [a, b] = [1, 2];
    console.log(a); // 1
    console.log(b); // 2
    

### Default values

We can set a default value to a variable. In this case that the value unpacked from the array will be undefined.

    let a, b;
    
    [a=5, b=7] = [1];
    console.log(a); // 1
    console.log(b); // 7
    

### Swapping variables

We can swap two variables values in one destructuring expression. If we want to swap variables without a destructuring assignment, swapping two values requires a temporary variable (in low-level languages, the XOR-swap trick).

    let a = 1;
    let b = 3;
    
    [a, b] = [b, a];
    console.log(a); // 3
    console.log(b); // 1
    
    const arr = [1,2,3];
    [arr[2], arr[1]] = [arr[1], arr[2]];
    console.log(arr); // [1,3,2]
    

### Parsing an array returned from a function

As we know it has been possible to return an array from a function, but with destructuring, we can make more concise the array return value.

    function f() {
      return [1, 2];
    }
    
    let a, b; 
    [a, b] = f(); 
    console.log(a); // 1
    console.log(b); // 2
    

In the example above, the f() function returns the values \[1, 2\] as its output, which can be parsed in one line with JavaScript destructuring.

### Ignoring some returned values

We can ignore or skip return values that we are not interested in.

    function f() {
      return [1, 2, 3];
    }
    
    const [a, , b] = f();
    console.log(a); // 1
    console.log(b); // 3
    

It is also possible to ignore all return values:

    [,,] = f();
    

### Assigning the rest of an array to a variable

When we destructuring an array, we can unpack and assign the parts of it to a variable using the rest:

    const [a, ...b] = [1, 2, 3];
    console.log(a); // 1
    console.log(b); // [2, 3]
    

> Note: If a trailing comma is used on the left-hand side with a rest element a SyntaxError will be thrown.

### Nested Array Destructuring

We can also do nested destructuring with arrays.

    const color = ['#FF00FF', [255, 0, 255], 'rgb(255, 0, 255)'];
    
    // Use nested destructuring to assign red, green and blue
    const [hex, [red, green, blue]] = color;
    
    console.log(hex, red, green, blue); // #FF00FF 255 0 255
    

As we can see in this article ES6 destructuring is useful in many cases. I hope you can understand how the destructuring in JavaScript works if you find this article useful please share it.