---
title: Using External Libraries
module: 8
jotted: false
---

# Using External Libraries

As you learned through the Khan Academy information, in order to use a JS Library, you need to link in into your web application via a script tag in your HTML file. This is similar to how you link to the JavaScript files you write for these web apps.

Generally, there are two ways of linking to and using a library.

1. You can download the library to your project directory, then link to it using relative URL's.
    - i.e. `<script src="./libs/downloaded-library-file.js"></script>`
    - This method presumes that you will also upload the file to wherever it is that your main source code will be served from.
2. The other option is to use a CDN or Content Distribution Network. CDN's are large collections of external libraries, with links that allow developers to pull in the library from someone else's server.
    - i.e. `<script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.6.0/p5.min.js"></script>`
    - There are numerous CDN providers. When you find a library you want to use, they will have typically chosen a CDN host to also deliver their library files. (The example above is for the p5.js lib files hosted on CloudFlare's cdn.)

When linking to the JavaScript library file in your HTML, your web application will load the library, as well as its associated functions or global variables. They are then ready for your use! This is what you saw this in the Khan Academy video on the second page. If you have taken MART120 - Creative Coding, you also have been using the p5.js library in this way. The `setup()` and `draw()` functions are both part of the p5.js library. When we call in p5, either via a file or CDN, these functions get exposed to the global environment for use by JS.

# Learning External Libraries

Obviously, there is slightly more to using an external JS library than just including it in your code. Somehow, you have to learn the available functions, tools, classes, and such that make up the library. To do this you will rely usually on 2-3 sources.

1. Official documentation and reference pages.
    - For almost every decent library, there is also a decent documentation or reference page/s. This resource will tend to be more technical in nature. Usually, it will list all of the available functions or classes that make up the library, along with technical information about what they do and how to implement them.
2. Official examples.
    - As with documentation, most decent libraries will include at least one, if not multiple, well commented examples of the library in a project.
3. Unofficial examples or tutorials.
    - Popular libraries that have garnered a large user-base or following will also often have unofficial tutorials and examples of the library. For developers, creating these types of resources allows them to practice using the library and gain a deeper understanding of it. It may also increase the ability to get other jobs or work on specific projects. As with anything on the internet, these types of resources can be "hit and miss", with some providing great content, and others not.

    
