# javascript-html-to-rtf-browser

Process the `html-to-rtf-browser` npm package to build a simple script for the browser.


## Depenedencies ##    
    npm / nodeJs
    npm install browserify
    npm install html-to-rtf-browser

## Bundle the package and it's dependcies ##
    browserify wrapper.js -o html-to-rtf-browser.js


## Minify ##
Additionally you can minify the result.

Install minifier.

    npm install uglify-js -g
    uglifyjs --compress --mangle --comments -o html-to-rtf-browser.min.js -- html-to-rtf-browser.js

Now you have the result the 
[html-to-rtf-browser.min.js](https://github.com/geraphl/javascript-html-to-rtf-browser/blob/main/html-to-rtf-browser.min.js) file.

## Uasage ##
The script can now be included to your page by adding

    <script src="~/js/html-to-rtf-browser.min.js"></script>
to your html.

Then you can convert `html` to micrsosofts rtf format by adding
    
    var htmlToRtfLocal = new window.htmlToRtf();
    var rtfContent = htmlToRtfLocal.convertHtmlToRtf(htmlContent);

to you javascript. 