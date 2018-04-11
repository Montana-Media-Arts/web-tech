---
title: The jQuery Object
module: 8
jotted: false
---

# Basics of jQuery

## The jQuery Object

jQuery works from a simple idea that all elements should be easily accessible and manipulatable. To accomplish this, jQuery utilizes a CSS-like selection process for elements. To select an element, a developer needs to pass CSS-like selections to the jQuery selector. The jQuery selector is `$()`, with the CSS selectors being placed within, typically in quotes.

For example, to select all of the `h1` elements on a page, a developer would call the following;

```js
$( "h1" )
```

This will return a jQuery object containing a reference to the all of the matching `h1` elements in the DOM.

As you will learn it is from this object that most of your work will occur for jQuery.

## Document Ready

Another common thing with jQuery is the encouragement that developers use a "document ready" function. This function should wrap any other statements or functions that will effect the DOM. The "document ready" function only executes _after_ the web page and DOM are loaded and ready for manipulation, but before things like images may fully be loaded. You should also get in practice of doing this.

The document ready function looks like one of the following;

```js
// long document ready object
$( document ).ready(function(){
    // your jQuery and DOM related code here
});

// short hand document ready function
$(function(){
    // your jQuery and DOM related code here
});
```
