# What will be covered
1. What are HTML and CSS
    * Basic structure and syntax
1. Creating and controlling our content
1. Placing images
1. Creating and linking pages together
1. Creating basic layouts

---

## 1. What are HTML and CSS
	
`The building blocks of the web`
> * HTML
> * CSS
> * JavaScript
	
## HTML

`HTML is a markup language, it tells the browser what the content we are writing actually is (for example):`

> * Heading
> * Regular paragraph
> * A link
> * Bold or italic text
> * A navigation
> * Footer
> * The main content of the page

## Basic syntax of HTML
`- Using Tags <-- the browser identifies the content wrapped in tags and know what is what`

> \<tag> Opening tag

> \</tag> Closing tag

An opening and a closing tags forms together an Element

## Recap:
	- Tags are inside of <> 
	- Closing tags include a forward slash </>
	- Everything from the opening to closing tag is called an Element
	- Elements define our content to the browser 


## Basic file structure

> \<!DOCTYPE html>

Tells the browser that this is a HTML5 document

> \<html> 

Tells the browser that we are starting to write HTML - Acts as a "root" of out document

> \<head> Metainformation
* Is not visible to the visitor
* It contains essential information
* It's more like a "brain" than a "head"

> \<title> 
* It is part of the <head> </head> element
* Not visible in the actual page, but can be seen when hovering over page's tab in the browser, and shows up in the search results

> \<body>
* Contains the content that will be visible to the user when visiting the website

### Example:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>My first website</title>
    </head>
    <body>
        
    </body>
</html>
```

## Heading and paragraphs

`- Headings - denote hierarchy and page structure`
    
* Six levels of headings: 
> \<h1>,\<h2>,\<h3>,\<h4>,\<h5>,\<h6>

### Example:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>My first website</title>
    </head>
    <body>
        <h1>My very first webpage</h1>
        <h2>Learning headings: this is heading h2</h2>
        <h3>Heading 3</h3>
        <h4>Heading 4</h4>
        <h5>Heading 5</h5>
        <h6>Heading 6</h6>
    </body>
</html>
```

`- Paragraphs are the regular text`
> * \<p>

### Example:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>My first website</title>
    </head>
    
    <body>
        <h1>My very first webpage</h1>
        <h2>Websites are built with HTML</h2>
        <p>HTML is a markup language that tells the browser what everything is</p>
        <p>Awesome</p>
    </body> 
</html>
```

## Recap:

```html
<!DOCTYPE html>
<html>
	<head>
		<title> write page title here </title>
	</head>
	<body>
	
	Content goes here
	
	</body>
</html>
```

* Remember to always close a heading or paragraph before starting another one
* \<h1> to \<h6> only, there is no \<h7> and beyond
* \<p> only, there is no \<p1>, \<p2>, etc.

## Strong and emphasis

> \<strong>
* Text inside this tag indicates that it is of strong importance
* Browsers makes this text **bold**

> \<em>
* The text inside this tag has stress emphasis
* Browsers makes this text *italics*

This tags are inline elements, are used inside paragraphs

\<strong> and \<em> needs to be closed before a new paragraph

### Exercise:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>This is my first website</title>
    </head>
<body>
    <h1>This is my first website</h1>
    <p>I'm learning HTML from scratch</p>
    <h2>I'm looking forward for exciting times</h2>
    <p><strong>Today</strong><em> I'm writing</em> first line of code</p> 
</body>
</html>
```


## File naming and organization

### File naming unwritten rules
* Keep file name short
* Use descriptive names

    (e.g. bad: "page1.html" vs good: "index.html")
* No spaces, use underscores or hyphens instead
* Use lower case ("About-Us.html" vs "about-us.html")

### File organization

* The main folder is called **root folder**
* The homepage **must be** `index.html`
* `index.html` **must be in the root folder**, and not a subfolder
* Other pages could be in subfolders
* Images should be placed in a subfolder

## HTML Anchors and Attributes

> \<a>
* It is short from anchor
* It is used to link to a different location whitin the current page, or to another page

### Example:
> \<a>google\</a>

Attributes are added to elements, *always in the opening tag*, and it gives **extra information** to the browser about that element. (e.g. where the link goes, the location of an image file)

Attributes are normally followed by equal sign and quotation marks

### Example:

> \<a href="http://google.com">Google\</a>

### Absolute vs relative paths

> \<a href="http://duckduckgo.com">This is the absolute path\</a>

> \<a href="about-us.html">This is the relative path\</a>

## CSS Introduction and Basics

* CSS is written in property:value pairs
* They are always separated by a colon **:**
* The value is always followed by a semicolon **;**
* We can write CSS inside a *style* attribute

```html
<h1 style="background-color: blue; font-size: 30px;">My first website</h1>
<p style="font-size: 20px; color: red;">Today I'm learning how to create websites and how to use CSS</p>
```

> style="background-color: red;"

> style="color: blue;"

> style="font-size: 30px;"

> style="text-align: left / center / right;"

## About Colors

`Colors can be set with keywords, hex codes, rgb and hsl values`

> kewords: "red", "steelblue", "hotpink", "lightgreen", etc.

> hex - hexadecimal values: start with a **#**, use numbers from **0** to **9** and letters from **a** to **f** : e.g. **#7ab0fb**

> rgb - Red, Green, Blue: **rgb(0, 255, 0)**

> hsl - Hue, Saturation, Lightness: **hsl(240, 100%, 75%)**

---

## Practice

index.html
```html
<!-- 
HTML
  - h1 (the title of the page)
  - An introductory paragraph
  - Two h2s, each followed by a few paragraphs
  - Inside the paragraphs, use strong and emphasis tags
  - If you are feeling adventorus add a second page and link to it
  
CSS
  - Change the color of the h1
  - Change the text alignment of the h1
  - Change the color of the h2s
  - Change the font-size of the paragraphs
  - If you added a link, change the color of it
 -->
 
 <!DOCTYPE html>
 <html>
     <head>
         <title>Green webpage</title>
     </head>
     <body>
         <h1 style="text-align: center; color: green;">This is the Green webpage</h1>
         <h2 style="text-align: left; color: darkblue; background-color: lightblue;">First Chapter of the story</h2>
         <p style="text-align: left; color: grey;">The <strong>story</strong> of <em>Green</em> begins with...</p>
         <p style="font-size: 20px;">This is the <em>second paragraph</em> of first section</p>
         <h2 style="text-align: right; color: white; background-color: purple;">Second Chapter of the story goes on...</h2>
         <p>To continue reading go to <a href="second-chapter.html"; style="color: red">next</a> page</p>
     </body>
 </html>
 ```
second-chapter.html
```html
<html>
    <head>
        <title>Second Chapter...???!!!</title>
    </head>
    <body style="background-color: cyan;">
        <h1 style="color: darkblue;">Here should be the Second Chapter</h1>
        <p style="color: grey;">But it isn't...</p>
        <p>You might want to go <a href="index.html" style="font-size: 30px; color: brown;">back</a> to homepage</p>
    </body>
</html>
```

## HTML lists

`There are two different type of lists:`

* Order lists

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
```
* Unorder lists

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

## Images

`For images we are using the following tag`

> \<img>

The image tag is self-closing, you don't need to use a closing tag like: \</img>

`Images use the "src" attribute, short for source` 

The syntax:
```html
<img src="image.jpg">

<img src="https://static01.nyt.com/images/2016/07/26/science/Obsscitake/Obsscitake-videoSixteenByNineJumbo1600.jpg">
```

`The second mandatory attribute is "alt" (images are not valid without it) - it describes the image, helpfull for accesibility`

The syntax:
```html
<img src="image1.jpg" alt="This is image 1">
```