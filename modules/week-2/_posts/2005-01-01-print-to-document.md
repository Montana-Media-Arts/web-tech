---
title: Print to Document
module: 2
jotted: true
---

# Printing to the Document

You will use the `console.log()` function often throughout this semester and beyond. Printing information to the web console is an easy way to _debug_ code and verify whether your programs are working.

However, for the moment, we also want to be able to see the output in our browser window. We will learn a couple ways of effecting the [DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model) in the coming weeks, but one of the simplest methods, and the one we will employ this week is the [`document.write()` function](https://developer.mozilla.org/en-US/docs/Web/API/Document/write).

The `document.write()` function takes a single input parameter; a string, of properly formatted markup (HTML). This is then placed on the HTML page in the browser.

The `document.write()` function, in some ways, could be likened to a sledge-hammer approach to placing markup in a browser window. If the function is called _after_ the page loads, then it replaces all existing markup in the document. This will not be an issue for us at the moment, but know, that if you use this function in the future, that you will need to be careful of when you call it.

## "Hello World!" Example

The following example places a level 1 header in an HTML document using the `document.write()` function. This function is placed in a separate JavaScript file, with the string of formatted markup text. As with before, this _script_ is called from the HTML document, using the script tag.

<div id="code-heading">JS</div>

```js
document.write("<h1>Hello World!</h1>");
```

<div id="code-ruler"></div>
<div id="code-heading">HTML</div>

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Using document.write</title>
        <style>
            body{ background-color: red;}
        </style>
    </head>
    <body>
        <script src="./script.js"></script>
    </body>
</html>
```

<div class="displayed_jotted_example">
    <div id="jotted-demo-1" class=""></div>
</div>
<script>
    new Jotted(document.querySelector("#jotted-demo-1"), {
    files: [
        {
            type: "js",
            url:"https://raw.githubusercontent.com/Montana-Media-Arts/441-WebTech/master/lecture_code/02/03-document-write/script.js"
        },
        {
            type: "html",
            url:"https://raw.githubusercontent.com/Montana-Media-Arts/441-WebTech/master/lecture_code/02/03-document-write/index.html"
    }],
    // plugins: [ "codemirror", "console" ]
    plugins: [ "codemirror" ]
});
</script>

| [**[Code Download]**](https://github.com/Montana-Media-Arts/441-WebTech/raw/master/lecture_code/02/03-document-write/03-document-write.zip) | [**[View on GitHub ]**](https://github.com/Montana-Media-Arts/441-WebTech/raw/master/lecture_code/02/03-document-write/) | [**[Live Example]**](https://montana-media-arts.github.io/441-WebTech/lecture_code/02/03-document-write/) |
