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

```
heading <h1>, <h2>, <h3>, <h4>, <h5> and stops at <h6>
```

```
paragraphs is regular text <p>, they are not numbered, there is no <p1>, <p2>, <p3>...
```

```
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
