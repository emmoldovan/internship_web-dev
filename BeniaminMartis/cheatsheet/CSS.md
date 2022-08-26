## `CSS`
- `C`ascading `S`tyle `S`heets
- Hoe our websites look <br>
    *Fonts, Colors, backgrounds, layouts and more*


- `properties` are what we want to change. (Color, font-size, font-weight)
- `Values` are what we want to set that property to: font-size:21px;

- `Style attribute` we can write CSS inside the quotation marks.
<p style="">
<style ="font-size:21px">

<html>
    <head>
        <title>Introduction to CSS</title>
    </head>
    <body>
        <h1 style="font-size: 70px; color: red;">Cascading Style Sheets</h1>
        <p>We use CSS to add style to our HTML documents.</p>
        <p style="color: blue">There are a few different ways to add CSS to a document, but for time being we'll be using <em>inline</em> CSS.</p>
        <h2 style="background-color: purple; color: white;">Inline CSS</h2>
        <p>Inline CSS is written directly in our HTML using a style attribute.</p>
        <p>We can style any element using inline styles, from the body to headings and paragraphs, <a href="#">as well as links</a> and strong and em tags too!</p>
    </body>
</html>

- CSS is always separated by a colon `:`
- The value is always followed by a semicolon `;`
- we can write CSS inside a style attribute `<em>inline</em>`

`Basic Styles`
- `font-size` - sets the font size. px (pixels)
- `color` - Changes the color of the text
- `background-color` - sets the background color 
- `text-align` - Align the text to the left, center, or right

- Colors can be set with keywords, hex codes, rgb and hsl values
- `keywords` - "red", "steelblue", "hotpink"
- `hex` - hexadecimal values: #7ab0fb; 
- `rgb` - Red, Green, Blue rgb(0,255,0)
- `hsl` - Hue, Saturation, Lightness hsl (240, 100%, 75%) (hue 240, saturation 100%, lightness hsl 75%)

<!-- we can use an internal style sheet that is placed in the head of our pages -->

<head>
    <style>
        CSS goes here
    </style>
</head>

<!--How do we chose what we want to style?-->
- selectors
- `If you want to select the whole body of the text to add a change on it you do it like this.`

    body {
        color: #323232;
    }

- `Rule:` selector and property value declarations all of that together is the rule.

- `Selecting elements`: 
<ul>
- Write the element (what is inside the tag), but without the tag itself <> <br>
- Do NOT include ~~attributes~~ (if your doing an image your just putting img your not putting ~~img and src etc..~~)(same with links you are not putting ~~`href`~~ in there you are just putting `a` since that is the anchor tag)<br>
- a{ write CSS inside here }
- p{ ... }
- h2{ ... }
</ul>

- With an `External CSS` file, we can have one stylesheet controlling all of our pages at the same time. you just have to link that CSS file with every file you would like to be changed. Be very careful with this because you can lose a ton of work.
One file controls ALL the styles, not the page you are on. If you delete something from the stylesheet, or change something, it is changing for all the pages.  

- How do you connect your External CSS file to your pages?<br>
Use a `link`, which links to your CSS file. <br>
In the head of our document, we add: <br>
```html 
<link href="css/style.css"> rel="stylesheet">
```
```
body {
    background-color: #333; 
    color: #f4f4f4;
}

a {
    color: darksalmon;
}

h1 {
    color: aquamarine;
}
```

- do not mix External CSS files with Internal CSS files, because if you do than you will not know where to look when you need to make a change. 


- `The three primary ways to select something is` :
<ul>
 
- Element selector<br>
- Class Selector <br>
- ID selector <br>

</ul>

`Element Selector` simply write the element's tag, without the <> <br>
Also, do NOT include any attributes.
```
body {
    background-color: #333; 
    color: #f4f4f4;
}

a {
    color: darksalmon;
}
```

`Class Selector` are a type of attribute we can add to an HTML element. 
```
<p class="intro"> ... </p>
```
In CSS I can select the class attribute by using a full stop. My full stop is the "." the dot before the intro
```
.intro {
    font-size: 18px;
    color: #2b5dad;
}
```
If it has a dot intro it selects a paragraph that has a class intro on it. <br>
Classes are type of attribute we can add to an HTML element<br>
The dot literally means class of intro
```
<p class="intro"> ... </p>
```
```
p.intro{
    font-size: 18px;
    color: #2b5dad;
}
```
```
.sidebar {
    padding: 1em;
    background: #f4f4f4;
}
.button {
    text-decoration: none;
    background: #ff3300
    padding: .5em 1.5em;
}
```
- IDs are a type of attribute we can add to an HTML element <br>
Instead of class it's ID <br>
An ID is represented by a hashtag (#)
```
<p id="intro"> ... </p>

#intro {
    font-size: 18px;
    color: #2b5dad;
}
```
- The ID selector
```
#main {
    background: #f4f4f4;
}
#carousel {
    max-height: 75vh;
}
```
- `ID` is an individual. (you can only have something with an ID once per page. so if you have an ID main, you can only have that main on one element in that page.)<br>
Id will overwrite a class if they are both selecting the same thing.

- `Class` is a group (class can be used over and over again on the same page)<br>
Use classes dont use IDs unless is necessary

- naming classes and IDs, Spaces cause problems! use a (-) instead of spacing.
```
<div class="a-box"> == .a-box { ... }
```
- How do you make a paragraph different in color than other paragraph? 
```
body {
    background-color: #333; 
    color: #f4f4f4;
}

a {
    color: darksalmon;
}

.intro {
    font-size: 24px;
}

#earth-title {
    color: lightgreen;
}

#mars-title {
    color: lightsalmon;
}
```
- The way to leave a coment in CSS is: `/* COMMENT HERE */` nothing that is shown up here will show up in the browser. 

- Margin = adding empty space around the text
- Padding = adding more background around the text
```
border-style
/* Keyword values */
border-style: none;
border-style: hidden;
border-style: dotted;
border-style: dashed;
border-style: solid;
border-style: double;
border-style: groove;
border-style: ridge;
border-style: inset;
border-style: outset;

/* top and bottom | left and right */
border-style: dotted solid;

/* top | left and right | bottom */
border-style: hidden double dashed;

/* top | right | bottom | left */
border-style: none solid dotted dashed;

/* Global values */
border-style: inherit;
border-style: initial;
border-style: revert;
border-style: revert-layer;
border-style: unset;

- The border-style property may be specified using one, two, three, or four values.

1. When one value is specified, it applies the same style to all four sides.
2. When two values are specified, the first style applies to the top and bottom, the second to the left and right.
3. When three values are specified, the first style applies to the top, the second to the left and right, the third to the bottom.
4. When four values are specified, the styles apply to the top, right, bottom, and left in that order (clockwise).

- Each value is a keyword chosen from the list below.

Values
<line-style>
Describes the style of the border. It can have the following values:

none
Like the hidden keyword, displays no border. Unless a background-image is set, the computed value of the same side's border-width will be 0, even if the specified value is something else. In the case of table cell and border collapsing, the none value has the lowest priority: if any other conflicting border is set, it will be displayed.

hidden
Like the none keyword, displays no border. Unless a background-image is set, the computed value of the same side's border-width will be 0, even if the specified value is something else. In the case of table cell and border collapsing, the hidden value has the highest priority: if any other conflicting border is set, it won't be displayed.

dotted
Displays a series of rounded dots. The spacing of the dots is not defined by the specification and is implementation-specific. The radius of the dots is half the computed value of the same side's border-width.

dashed
Displays a series of short square-ended dashes or line segments. The exact size and length of the segments are not defined by the specification and are implementation-specific.

solid
Displays a single, straight, solid line.

double
Displays two straight lines that add up to the pixel size defined by border-width.

groove
Displays a border with a carved appearance. It is the opposite of ridge.

ridge
Displays a border with an extruded appearance. It is the opposite of groove.

inset
Displays a border that makes the element appear embedded. It is the opposite of outset. When applied to a table cell with border-collapse set to collapsed, this value behaves like groove.

outset
Displays a border that makes the element appear embossed. It is the opposite of inset. When applied to a table cell with border-collapse set to collapsed, this value behaves like ridge.
```
```
Formal syntax
border-style = 
  <line-style>{1,4}  

<line-style> = 
  none    |
  hidden  |
  dotted  |
  dashed  |
  solid   |
  double  |
  groove  |
  ridge   |
  inset   |
  outset  
  ```
   - Example all property values. <br>
   `HTML`
   ```
   HTML
   <pre class="b1">none</pre>
<pre class="b2">hidden</pre>
<pre class="b3">dotted</pre>
<pre class="b4">dashed</pre>
<pre class="b5">solid</pre>
<pre class="b6">double</pre>
<pre class="b7">groove</pre>
<pre class="b8">ridge</pre>
<pre class="b9">inset</pre>
<pre class="b10">outset</pre>

```
`CSS`
```
CSS 

pre {
  height: 80px;
  width: 120px;
  margin: 20px;
  padding: 20px;
  display: inline-block;
  background-color: palegreen;
  border-width: 5px;
  box-sizing: border-box;
}

/* border-style example classes */
.b1 {
  border-style: none;
}

.b2 {
  border-style: hidden;
}

.b3 {
  border-style: dotted;
}

.b4 {
  border-style: dashed;
}

.b5 {
  border-style: solid;
}

.b6 {
  border-style: double;
}

.b7 {
  border-style: groove;
}

.b8 {
  border-style: ridge;
}

.b9 {
  border-style: inset;
}

.b10 {
  border-style: outset;
}
```
- `Borders` add a border around your element. 

_It takes three properties to set a border_
<ul>

- border-width
- border-style
- border-color
</ul>

- Shorthand border: [width] [style] [color] - they can be placed in any order
<ul>

_You can also control specific sides_

- `border-left` - shorthand for only the left border
- `border-right-width` only modifying the width of the right border
</ul>

border-style

* you can also use border shorthand (the order you put them in doesn't matter
* border: 2px solid pink;
* you can also control the border of the different sides independently 
```
border-left: 2px solid pink;
border-right: 5px dotted red;
border-bottom: 10px double green;
border-top: 1px dashed purple;
```
