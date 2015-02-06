#Intermediate HTML & CSS
--

##Installation
- Install [Sublime Text](http://www.sublimetext.com/)
	- Sublime Text is a text-editor for code.

## Review
- Explain the difference between front-end and back-end web development.
- What does HTML stand for? And what does it do?
- What does CSS stand for? And what does it do?
- What is a tag? How is it used?
- How do you link your HTML to your CSS?

##Element Alignment
- Inline elements can be aligned as text, so with the 'text-align' CSS property. 
- Block elements can be aligned using the space around them, so with 'margin.' A margin set to auto for both left and right will center the element. 

##The Grid Layout
- Most layouts operate on a 12-column grid system.
- Each column in the grid can contain nested grids itself.
- If you want a larger box, you need a greater column offset. 

![](http://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2013/05/960-12-col-grid.jpg
)
## Grouping (CSS)
- You can give the same properties to various selectors without having to repeat them. 
- To do this separate selectors with commas in one line and apply the same properties to all of them.

CSS:

```
h1, .paragraph, # aboutme {
	color: blue;
}

``` 
## Nesting(CSS)
- This means you have a selector within another selector. 

HTML:

```
<div id="top">
    <h1>Apple Pie</h1>
    <p>This is the recipe for my nonna's famous apple pie.</p>
    <p>The ingredients are: ....</p>
</div>

```
CSS:

```
#top {
    background-color: #ccc;
    padding: 1em
}

#top h1 {
    color: #ff0;
}

#top p {
    color: red;
    font-weight: bold;
}

```

##CSS Positioning
- There are four main types of positioning that you will see most often -static, relative, absolute, and fixed. 
- Turn to a partner and look these up and discuss the differences. 

## Twitter Bootstrap
- "Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web."
- To use it you can add the CDN (content delivery network) in the head tag of your HTML file:

```
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">

<!-- Optional theme -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap-theme.min.css">

<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>

```
------
- Another option is to integrate the bootstrap and jquery libraries in your code base and then add this snippet in your head tag:

	```
	<link rel="stylesheet" type="text/css" href="libraries/bootstrap-3.1.0/css/bootstrap.css" />

	```

- And this snippet before your closing body tag:
	
	
	```
	<script type="text/javascript" src="libraries/jquery-2.1.0/jquery-2.1.0.js"></script>
<script type="text/javascript" src="libraries/bootstrap-3.1.0/js/bootstrap.min.js"></script>
	
	```
	

## Linking JavaScript with HTML
- JavaScript enables interactivity with the page through animations and dynamic loading of the page. 
- In order to run an external JavaScript file, you need to link it to the HTML file. This usually goes before the closing body tag:
` <script src="js/script.js"></script>`
- Just like with CSS, you can also simply add a script tag directly in your HTML file (this is what we will be doing today). 

###Variables
- Allow program to remember values for a later time. 
- Entity in which value is stored. 
- Getting the value from a variable = accessing the variable. 
- Variables start with a lower case letter, use camel case if the variable name consists of many words. 

```
var price1 = 11;
var price2 = 4;
var total = price1 + price2;

```

###Alerts
- The alert() method displays an alert box with a specified message and an ok or cancel button.
- You set up an alert by placing a script tag before the closing body tag. 

```
 <script>
    alert("Hello, world. Welcome to our cool new site!");
  </script>

```

###Methods
- The actions that can be performed on objects. 
- There are many built-in methods in JavaScript. 

Ex:

```
var message = "Hello world!";
var x = message.toUpperCase();

```