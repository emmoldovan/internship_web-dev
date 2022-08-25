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