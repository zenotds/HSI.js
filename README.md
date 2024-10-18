# HSI.js

**HTML Snippet Includes**

## Overview

HSI.js is a simple client-side solution for including external HTML snippets into your web pages. It fetches and replaces designated elements with the contents of external HTML files, making it easier to modularize your HTML structure.

## Usage

To use HSI.js, just include `hsi.min.js` in your project. Then, add a `data-include` attribute to any valid HTML element, specifying the URL of the HTML file to include. HSI.js will fetch the external file and **replace** the element with the fetched content.

For example, if the `snippet.html` file contains:

`<h1>Great Scott!</h1>`

And your main HTML document has this structure:

`<body>` 
    `<div data-include="snippet.html"></div>` 
`</body>`

After HSI.js runs, the result will be:

`<body>`
    `<h1>Great Scott!</h1>`
`</body>`

# File System Support

HSI.js can also be used from the local file system, making it ideal for front-end developers working on HTML snippets without needing to run a local web server. This allows easy testing and implementation of server-side includes locally.
