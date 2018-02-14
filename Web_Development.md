#Introduction
Useful website for web development: 
+ https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web

+ https://www.w3schools.com/js/default.asp

There are 3 main languages all web developers must learn:
+ **HTML** to define the content of web pages
+ **CSS** to specify the layout of webpages
+ **Javascript** to program the behaviour of webpages




# Languages

## HTML

+ HTML is not a programming language.  It is not an executable script, it is a 'markup' of the text for the browser to read and interpret as web page content. https://ischool.syr.edu/infospace/2012/04/05/why-html-is-not-a-programming-language/.

Webpages can be created and modified using professional HTML editors, but to start learning HTML, open up a simple text editor (i.e. Notepad++) and save it with  .htm suffix and set the encoding to UTF-8

#### HTML documents

All HTML docments must start wit a document type declaration:

The HTML document itself begins with <html > and ends with </html>

The visible part of the HTML document is between <body > and </body>

``` html
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html> 
```


#### HTML consists of TAGs

Several important tags:
+ HTML links are defined with the <a> tag, the **href** attribute specifies the link`s destination:  ``` <a href="https://www.w3schools.com">This is a link</a>```
+ HTML images are defined with the <img> tag, the source file (src), alternative text, widt and height are provided as attributes: ```<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">```
+ The <head> element is a container for metadata and is placed betzeen the <html> tag and the <body> tag. Metadata is not displayed and usually defines the document title, character set, styles, links, scripts and other meta information. https://www.w3schools.com/html/html_head.asp
  + <meta>: specify which character set is used
  + <title>: defines title of the document in the browser tab, search engines, favorite tabs
  + <link>: used to link to external style sheets
  + <script>: define client-side Javascripts




## CSS 

css = Cascading Style sheet. It is not a programming language nor a markup language, it is a style sheet language. Apply styles **selectively to elements in HTML documents**. 




## JavaScript

JavaScript comments:
+ Single line comments: //
+ multiline comments: start /* and end */

JavaScript funcitons:
``` JavaScript
function name(parameter1, parameter2, parameter3) {
    code to be executed
}
```
Meaning of the parentheses surrounding a function:

``` javascript
(function() {
    var Dom = YAHOO.util.Dom,
    Event = YAHOO.util.Event,
    layout = null,
        ...
})();
```

It is a self-executing anonymous function. The first set of parentheses contain the expressions to be executed, and the second set of parentheses executes those expressions. It is a useful construct when trying to hide variables from the parent namespace. All the code within the function is contained in the private scope of the function, meaning it can't be accessed at all from outside the function, making it truly private


#  How is it related to each other?
### Folder structure
Create a folder structure to connect all of the files above

Main_folder:
+ index.html
+ styles directory: holding CSS code, styling the content
+ script directory: contains all JavaScript code used to add interactive functionality to your site
+ images directory: contains the images you use on your website



### Development environment

There are some webapps allowing you to enter HTML, CSS an JvaScript and then display the result of that code when rendered as a website all in one browser tab.

https://jsfiddle.net/




