---
title: Types & Values
module: 3
jotted: true
---

# Values, Data Types, & Operators

Please read the following;

- Haverbeke, Marijn. **Eloquent JavaScript: A Modern Introduction to Programming.** 3rd Edition. N.p., 2018. Web.
    - [_Chapter 1; Values, Types, and Operators_](http://eloquentjavascript.net/3rd_edition/01_values.html)
- **JavaScript Guide.** MDN web docs. 2018. Web.
    - [_Grammar and Types_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_Types)
    - [_Expressions and operators_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)



## Goals

At the end of the chapter you should have an understanding for;

- **Values**
    - Regular Values
    - Empty Values
        - `null`
        - `undefined`
- **Data Types**
    - Numbers
        - Regular Numbers
        - Special Numbers
    - Strings
        - regular strings (`"Hello World!"`, `'single quote string'`)
        - special characters (i.e., `\n`, `\t`)
        - template literal strings (``these use backticks and have special properties``)
    - Booleans
- **Operators**
    - Basic mathematical operators
        - addition/subtraction on numbers (`+`/`-`)
        - multiplication/division on numbers (`*`/`/`)
        - modulo on numbers (`%`)
    - String operators
        - String concatenation (`+`)
    - Unary Operators
        - `typeof`
    - Comparison Operators
        - `<`, `>`,`<=`, `>=`, `==`, `!=`
    - Logical Operators
        - or - `||`
        - and - `&&`
        - not - `!`
    - Type Conversion


## Interactive JS Console

While you work on this chapter, you should use the following interactive JS console to test out values, types, and operators.

<div id="jotted-demo-1" class="jotted-theme-stacked"></div>

<script>
    new Jotted(document.querySelector("#jotted-demo-1"), {
    files: [
        {
            type: "js",
            hide: false,
            content: "// try out operators, values, etc, here...\n\n// as an example\nconsole.log( typeof \"Hello World!\");\nconsole.log( 5*10 == 50 );\n\n\n"
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



## Videos

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/808eYu9B9Yw" frameborder="0" allowfullscreen></iframe></div>

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/Vd_Z1bYGrCM" frameborder="0" allowfullscreen></iframe></div>
