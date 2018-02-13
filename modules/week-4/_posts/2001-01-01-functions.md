---
title: Functions
module: 4
jotted: true
---

# Functions

_Functions_ are one of the basic building blocks of programming. As you will learn, functions _do something_ in code. Whether that is compute some value that is returned to the main program, or do something else as a side-effect to the main program.

The Mozilla Developer Network (MDN) defines functions as follows;

> Generally speaking, a function is a "subprogram" that can be called by code external to the function. Like the program itself, a function is composed of a sequence of statements called the function body. Values can be passed to a function, and the function may return a value.

You have already been using functions. These include;

```js
console.log("something to print");

prompt("something to say in a popup box");

window.write("print something to the DOM");
```

There are many "builtin" functions to JavaScript, which you will learn about and use as you progress.

JavaScript also allows you to define and use _your own custom_ functions. This is a critical technique for writing easily maintainable code that is well structured. As such, you will spend a lot of time this week learning about writing your own functions and how they can be used.

## Basic Invocation

#### Calling Functions

As you will learn about in more detail below, functions are called through the invocation of their name, followed by the _function operator_ (`()`).

```js
someFunction();
```

#### Supplying Function Parameters

Within in the function operator, you can supply _parameters_ to the function.

```js
someFunction( param1, param2 );
```

Function _parameters_ are pieces of data that the function uses towards computations or as information to do something with.

## Defining Functions

There are generally three ways to define your own functions in JS.

#### Function Declaration

The first is to call the `function` keyword, followed by;

- the function name
- a list of parameters (comma separated) to be used
- a series of JS statements, within curly brackets (`{}`) to execute when the function is invoked.

<div id="jotted-demo-2" class="jotted-theme-stacked"></div>

<script>
    new Jotted(document.querySelector("#jotted-demo-2"), {
    files: [
        {
            type: "js",
            hide: false,
            content:
`function myFirstFunction( inParam1, inParam2 ) {
    console.log( "a statement of something to do." );
    return inParam1 * inParam2;
}

let val = myFirstFunction( 4, 2 );
// -> returns 8 to 'val'
// -> and prints "a statement of something to do." in the console

// print val to ensure accuracy
console.log(val);
`
        }
    ],
    showBlank: false,
    showResult: false,
    plugins: [
        { name: 'ace', options: { "maxLines": 50 } },
        { name: 'console', options: { autoClear: true } },
    ]
});
</script>


#### Function Expression

The second way of defining functions is through _function expressions_, these assign a function to a binding namespace (i.e. a variable).

<div id="jotted-demo-3" class="jotted-theme-stacked"></div>

<script>
    new Jotted(document.querySelector("#jotted-demo-3"), {
    files: [
        {
            type: "js",
            hide: false,
            content:
`let multFunc = function( inParam1 ) {
    return inParam1 * inParam1;
};

let result = multFunc(3);
// -> result would equal 9
console.log( result );
`
        }
    ],
    showBlank: false,
    showResult: false,
    plugins: [
        { name: 'ace', options: { "maxLines": 50 } },
        { name: 'console', options: { autoClear: true } },
    ]
});
</script>


_Function Expressions_ work the same as _Function Definitions_, the primary difference is that _Function Expressions_ must be defined **before** they are called. _Function Definitions_ are **hoisted** to the top of the JS interpreter and can be placed anywhere in the code, even after their initial call, as they will be compiled first.

#### Arrow Function

The last type of definition you will learn about is _Arrow Functions_. This technique allows for the concise definition of functions, typically in a single line. This is useful when trying to write concise and clear code.

<div id="jotted-demo-4" class="jotted-theme-stacked"></div>

<script>
    new Jotted(document.querySelector("#jotted-demo-4"), {
    files: [
        {
            type: "js",
            hide: false,
            content:
`let a = [
  'Hydrogen',
  'Helium',
  'Lithium',
  'Beryllium'
];

let a2 = a.map(function(s) { return s.length; });

console.log(a2); // logs [8, 6, 7, 9]

let a3 = a.map(s => s.length);

console.log(a3); // logs [8, 6, 7, 9]
`
        }
    ],
    showBlank: false,
    showResult: false,
    plugins: [
        { name: 'ace', options: { "maxLines": 50 } },
        { name: 'console', options: { autoClear: true } },
    ]
});
</script>


## Reading

To get started, please read the following, which cover the usage and definition of functions in great detail;

- Haverbeke, Marijn. **Eloquent JavaScript: A Modern Introduction to Programming.** 3rd Edition. N.p., 2018. Web.
    - [_Chapter 3; Functions_](http://eloquentjavascript.net/3rd_edition/03_functions.html)
- **JavaScript Guide.** MDN web docs. 2018. Web.
    - [_Functions_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

## Videos

Videos on the basic of _Functions_!

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/R8SjM4DKK80" frameborder="0" allowfullscreen></iframe></div>

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/C1PZh_ea-7I" frameborder="0" allowfullscreen></iframe></div>


## Interactive JS Console

While you work on this chapter, you should use the following interactive JS console to test.

<div id="jotted-demo-1" class="jotted-theme-stacked"></div>

<script>
    new Jotted(document.querySelector("#jotted-demo-1"), {
    files: [
        {
            type: "js",
            hide: false,
            content: "// Your test code here!\n\n\n"
        }
    ],
    showBlank: false,
    showResult: false,
    plugins: [
        { name: 'ace', options: { "maxLines": 50 } },
        { name: 'console', options: { autoClear: false } },
    ]
});
</script>
