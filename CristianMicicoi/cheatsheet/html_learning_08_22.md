##### _08.16.2022_

# HTML & CSS Crash Course

> ## The building blocks of the web

- HTML (if you only have HTML, you have a functioning web page,but would be really boring) ;

  - _HyperText Markup Language_
  - _The content of websites is view in_
  - _Relatively straight forward_

- CSS (is what makes a site look much more interesting) ;

  - _Cascading Style Sheets_
  - _How our websites look (fonts, colors, backgrounds, layouts and more)_

- JavaScript
  - _Programming language_
  - _Can manipulate HTML and CSS_
  - _Use for simple manipulations to create full web apps_

> ## HTMl is a very simple language

### Tells the browser what the content we are writing actually is

- Heading or a regular paragraph
- A link, bold or italic text
- A navigation, footer, the main content of the page

> ## Basic syntax

## **_Tags_** (We wrap everything in "tags" to tell the browser what is what)

- ### Think of a book

```
<cover>
    <page>
        <heading>Chapter 3</heading>
        <subheading>The light of justice</subheading>
        <p>The clouds started rolling away...</p>
    </page>
    <page> </page>
    <page> </page>
</cover>
```

_Tags are inside of "<>"; closing tags include a forward slash</>; everything from the opening and closing tag is called an element; elements define our content to the browser._

> ## HTML basic file structure

```
<!DOCTYPE html> (the very first thing at the top of document; tells the browser that is an HTML5 document)
```

```
 <html> (we're telling the browser we're starting to write HTML, acts as the "roof" of our document; might seem redundant, but we can actually write HTML, CSS and JavaScript inside an HTML document)
```

```
    <head>(it's more like a brain then a head, it contains essential information; nothing here is visible to the visitor)
```

```
        <title> (in the head of the document, not visible in the page, but shows up in the tab of the browser and in search results)
```

```
<body> (contains the content that will be visible to the user when they visit a page)
```

```html
heading
<h1>
  ,
  <h2>
    ,
    <h3>
      ,
      <h4>
        ,
        <h5>
          and stops at
          <h6></h6>
        </h5>
      </h4>
    </h3>
  </h2>
</h1>
```

```html
paragraphs is regular text
<p>
  , they are not numbered, there is no
  <p1
    >, <p2>, <p3>...</p3></p2></p1
  >
</p>
```

```html
<!DOCTYPE html>
<html>
  <head>
    <title>page title</title>
  </head>
  <body>
    <h1>heading1</h1>
    <p>paragraph</p>
    <h2>heading 2</h2>
    <p>paragraph</p>
  </body>
</html>
```

##### _08.17.2022_

> ## HTML - strong and emphasis

```html
<strong>
  (the text inside
  <strong
    >) indicates that it is of strong importance; browsers make this text
    bold);</strong
  ></strong
>
```

```html
<em>
  (the text inside <em></em> has stress emphasis, browsers make this text
  italic);</em
>
```

- ## They are inline elements

  - use <"strong"> and <"em">(I write like this with quotation marks, because otherwise it appears as a line of code) ;
  - you must close a <"strong"> or <"em"> before the end of your paragraph

  ```html
  <p><strong>Warning:</strong> it's very cold outside</p>
  ```

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Storng and emphasis</title>
  </head>
  <body>
    <h1>Strong and amphasis</h1>
    <p>Strong and emphasis elements help put important on our text</p>

    <h2>The strong tag</h2>
    <p>We use the strong tag to put strong importance on text</p>

    <h3>An example</h3>
    <p><strong>Warning:</strong>watch out for the guard dog</p>

    <h2>The emphasis tag</h2>
    <p>We use the emphasis tag to put stress emphasis on our text</p>

    <h3>An example</h3>
    <p>It is <em>really</em> hot outside</p>
  </body>
  <html></html>
</html>
```

> ## File naming and organization

- ## File naming: keep file names short; they should be descriptive(e.g. "page2.html" vs. "about us .html"); no spaces, use underscores or hyphens instead; use lower case("About-us.html" vs "about-us.html");
- ## File organization: the main folder is called our **root folder**; the homepage **must be _index.html_** ; **_index.html_** must be in the root folder , and not a sub-folder; other pages can be in subfolder, depending on how you want to stay organized; images should be placed in a sub folder for better organization.

> ## HTML - anchors and attributes

```h
  <a> (short for "anchor") used to link either to a different location within the current page or to another page; we tell the anchor to link to with ATRIBUTES;
```

- atributes are normally followed by an equal sign and quotation marks; a link will not work without an **_href_** attribute:

```html
<a>href="https://google.com">google</a>
```

- If the page you are linking to is not part of your website, it must start with _http://_ or _https://_ to let the browser now it is an external site that you are linking to.

```html
<a href="https://google.com">google</a>
```

##### _08.18.2022_

```html
<html>
  <head>
    <title>Anchors and Attributes</title>
  </head>
  <body>
    <h1>Anchors</h1>
    <p>
      We use the anchor tag to setup hyperlinks. When a user clicks on the
      hyperlink, it will bring them to the specified location, which could be
      within the same page, or to another page.
    </p>
  </body>
</html>
```

> ## Introduction to CSS - _it's all about style!_

- ## CSS is all about **property: value** pairs: _properties_ are what we want to change(color, font-size, font-weight); _values_ are what we want to set that property to (font-size: 21px;)
- ## **The syntax** : there must be a colon (:) between the property and value: font-size: 21px'; the _value_ is always followed by a semicolon(;) ;
- ## **The style attribute**: one way to add CSS is through the _style_ attribute `<p style= "">` and write CSS inside the quotation marks: `<p style="font-size: 21px">`

##### _08.19.2022_

- ## Some basic styles:

  - _font-size_ - sets the font size, for now we stick to pixels (px) ;
  - _color_ - change the color of the text ;
  - _background-color_ - sets the background color ;
  - _tex-align_ - align the next to the **left, center or right** ;

- ## **Colors** can be set with keywords, hex codes, rhg and hsl values:
  - _keywords_ - "red", "steelblue", "hotpink" etc.
  - _hex_ - hexadecimal values: **#7ab0fb** etc.
  - _rgb_ - Red, Green, Blue: \*\*rgb(0,255,0) etc.
  - _hsl_ - Hue, Saturation, Lightness: hsl(240, 100%, 75%) etc.

##### _08.22.2022_

> ## HTML lists

- Two tipes of list:
  - ordered lists -> (ol)0 - each bullet or numbered item is a **list item** or li -> <>
  ```html
  <ol>
    <li>list item</li>
    1. list item
    <li>list item</li>
    2. list item
    <li>list item</li>
    3. list item
  </ol>
  ```

```html
<ul>
  <li>list item</li>
  <li>list item</li>
  <li>list item</li>
</ul>
```

> ## Images

- Images are like links, in that **they require an attribute to work** and this is _src_ attribute, wich is sort for _**source**_
- Images are different from other elements, in that they are **self-closing**.

```html
<img src="image.jpg" />
```

or

```html
<img src="image.jpg" />
```

- Like links, we can point to external images by including the entire URL of the image, or we can point to images within our site by listing the file name.

```html
<img src="image.jpg" /> <img src="https://website.com/image.jpg" />
```

- Images are not valid without an **alt** attribute. The **alt** attribute is used to describe the image, to describe the intent of the image:

```html
<img src="cute-cat.jpg" alt="a very cute cat" />
```

- If it is a decorative element or logo, it doesn't need alt text(but it _does_ still require the _alt_ attribute):

```html
<img src="logo.jpg" alt="" />
```

```html
<img src="decorative-red-ball.jpg" alt="" />
```

- Practice in _practice_ folder of the lists and images inserting in html.

##### _08.23.2022_

- ## Practice more with HTML that I have learned until now, creating three new pages about Earth an Mars in _practice_ folder and linking all the three pages together.

> ## Internal CSS

- Integrate internal style sheet :

```html
<head>
  <style>
    CSS goes here
  </style>
</head>
```

- We choose what we want to style with **selectors**:
  - to change all text color from body:
  ```html
  body { color: #323232; }
  ```
  - the property _value pair_ is also called _declaration_;
  - to select an element, write the element but without <> (a{...}), do not include attributes (p{...}), (h2 {...}); for image use: img without src, for link just using a, without <>;
- Practicing on the 3 pages I made above.

##### _08.24.2022_

> # External CSS

- ## With an external CSS file, we can have one stylesheet controling _all_ of our pages at the same time.
- ## **_Be careful_!** One file controls ALL styles, not the page you are on. If you delete something from the stylesheet, or change something, **it is changing for _all_ the pages!**
- ## Instead of a style element, where we can write the CSS, we can use a **link**, wich links to our CSS file. In the head of our document, we add:

```html
<link href="css/style.css" rel="stylesheet" />
```

#where "rel" is the relationship with my current html page.

> ## The relationship between HTML & CSS

## The three primary ways to select something:

- Element selector- learned in external CSS (write the element tag without the <>, and **do not** include any attributes);
- Class selector- classses are a type of attribute we can add to an HTML element:

```html
<p class="intro">...</p>
- will select any paragraph that has "intro" class on it.
```

#### In CSS the class attribute is referenced by using a full stop(.); used in paragraph like ex above, will select any paragraph that has "intro" class on it.

ex:

```html
.intro { font-size: 18px; color: #2b5dad; } .sidebar { padding:1em; background:
#f4f4f4; } .button { text-decoration: none; background:#ff3300; padding: .5em
1.5em; }
```

- ID selector: IDs are a type of attribute we can add to an HTML element

```html
<p id="intro">...</p>
```

An ID is represented by a hashtag.
Ex:

```html
#intro { font-size: 18px; color: #2b5dad; } #main { background: #f4f4f4 }
#carousel { max-height: 75vh; }
```

## **ID vs Class**

- I can't have the same ID twice in one page.
- a class can be used over and over again and _only once if you want_.
- ID will owerwrite a class if they are both selecting the same thing.

## Naming classes and IDs

- spaces can cause problems:

```html
<div class="a box">
  'is not'=/= .a box {...}
  <div class="a-box">'it is'== .a-box {...}</div>
</div>
```

- there are a lot more ways to select stuff!

> ## Comments

A useful way to leave notes to yourself, or others if you're working on a large project.
Two different ways to write them, but they use the same shortcut (_ctrl_ + _/_) :

- In HTML : `<!-- comment here -->`
- In CSS : `/*comment here */`

They are vey useful:

- reminding yourself why you did something or how something is working and where you are on the page
- creating sections, or making things more clear in your HTML
- leaving "TODO" notes to yourself (or others)

> ## The only tags you need to know (for now)

- The tags that i've seen so far have mostly been related to placing text or content on the page :

  - h1->h6
  - p
  - strong and em
  - a
  - ul, ol, and li
  - img

- This all just put content in the page, they not building layouts or controlling our layouts.

- There are several "layout" related HTML elements. All they function in the same way,so once you understand how one works, you understand how they all work.
- The difference between them is that they denote **different parts** of your website:
  - header
  - main
  - section
  - footer
  - nav
  - div (**generic**)

##### _08.25.2022_

> ## Intro to the box model

- Most elements are "block level" elements by default
  - they have a width of 100% of their parent
  - they have a height of 0
  - the height grows to match the content
  - they stack one on top of the other
  - !!! _Try to avoid setting height_ !!! to avoid text problems (written one over the other)
- Margins & Padding
  - margins are used to control the position of an element relative to those around it (margin-left, margin-right, margin-top, margin-bottom)
  - we also have a shorthand margin property:
  ```html
  margin: 10px(top) 20px(right) 30px(bottom) 40px(left) margin: 50px(top-bottom)
  50px(left-right) margins: 50px(all margins)
  ```
  - padding is used to control the positioning of content _inside_ our element; it works just like margin in terms of the long form and shorthand properties
  - margin= empty space; padding= more background(add space)
- Borders- add a border around your element. **It takes three properties to set a border** :

  - border-width
  - border-style
  - border-color
    (we need to do all three of this properties to actually get a border to work properly).
  - We can also use the border shorthand (the prder you put them it doesn't mattter);
    Ex:

  ```html
  .example { border-width: 2px; border-style: solid; border-color: pink; } =
  .example { border: 2px solid pink; }
  ```

- you can also control the border of the different sides independently :

  ```html
  .example { border-left: 2px solid red; border-right: 5px dotted blue;
  border-bottom: 10px double green; border-top: 1px dashed purple; }
  ```

- Box wrap up: the total width an height of an element is calculated by adding all the different part of the element together.

  **The four parts of an element**:

  - the content itself (what you set the width & height on)
  - the padding
  - the border
  - the margin

    _Don't forget that margin, padding, and borders add width to the left & the right_!

##### _08.26.2022_

> ## A basic layout (header-main-footer)

- The header(changes to make in practice lesson):
  - contains the `<h1>`
  - has a dark background color
  - has a light text color
  - text is center alligned
  - has a padding top anf bottom of 25px
  - has a margin bottom of 25px
- The main(changes to make in practice lesson):
  - place the provided imaged in here
  - place the text here using headings, paragraph and lists
  - give it light background color
  - give it a width of 600px
  - give it equal padding on all sides
  - give it a solid red border that is a 5px thick
- The footer(changes to make in practice lesson):
  - place the provided text in a paragraph
  - give it a dark background color
  - give it a light text color
  - center align the text
  - give it a padding top and bottom of 25px
  - give it a margin of 25px on the top only
- Centering and element on the page

  Margins accept a set width, but you can also use the **auto** keyword. **Auto** will automatically place all the avaible space on that side: ` margin-left: auto; margin-right: auto; margin: 0(top-bottom) auto(left-right);` -this will not work on the top and bottom to get this "auto" works on vetical, it works just on left-right sides; you must have width on the element;

  ## **When I have that little margin left-right that is default set by browser, I cand get rid of if I go on _body_ section and set first element `margin: 0;`**

- ## Creating columns- _for the longest time, we had to use something called **floats** to make block level elements go next to one another. It involves things sliding under each other and clears. It was not fun._ \*By default, when setting **display:flex** on a element, all the children will become columns.

- ## Creating the layout from scratch - the HTML
- ## Creating the layout - the CSS

> ## I have completed this HTML & CSS crash course and practice, by Kevin Powell!
