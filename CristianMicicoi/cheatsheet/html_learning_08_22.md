- ##### _08.16.2022_

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

- ##### _08.17.2022_

> ## HTML - strong and emphasis

```
<strong> (the text inside <strong>) indicates that it is of strong importance; browsers make this text bold);
```

```
<em> (the text inside <em></em> has stress emphasis, browsers make this text italic);
```

- ## They are inline elements

  - use <"strong"> and <"em">(I write like this with quotation marks, because otherwise it appears as a line of code) ;
  - you must close a <"strong"> or <"em"> before the end of your paragraph

  ```
  <p><strong>Warning:</strong> it's very cold outside</p>

  ```

```
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
  <html>
```

> ## File naming and organization

- ## File naming: keep file names short; they should be descriptive(e.g. "page2.html" vs. "about us .html"); no spaces, use underscores or hyphens instead; use lower case("About-us.html" vs "about-us.html");
- ## File organization: the main folder is called our **root folder**; the homepage **must be _index.html_** ; **_index.html_** must be in the root folder , and not a sub-folder; other pages can be in subfolder, depending on how you want to stay organized; images should be placed in a sub folder for better organization.

> ## HTML - anchors and attributes

```
  <a> (short for "anchor") used to link either to a different location within the current page or to another page; we tell the anchor to link to with ATRIBUTES;
```

- atributes are normally followed by an equal sign and quotation marks; a link will not work without an **_href_** attribute:

```
<a>href="https://google.com">google</a>
```

- If the page you are linking to is not part of your website, it must start with _http://_ or _https://_ to let the browser now it is an external site that you are linking to.

```
<a href="https://google.com">google</a>
```

- ##### _08.18.2022_

```
<html>
    <head>
        <title>Anchors and Attributes</title>
    </head>
    <body>
        <h1>Anchors</h1>
        <p>We use the anchor tag to setup hyperlinks. When a user clicks on the hyperlink, it will bring them to the specified location, which could be within the same page, or to another page.</p>
    </body>
</html>
```

> ## Introduction to CSS - _it's all about style!_

- CSS is all about **property: value** pairs: _properties_ are what we want to change(color, font-size, font-weight); _values_ are what we want to set that property to (font-size: 21px;)
- **The syntax** : there must be a colon (:) between the property and value: font-size: 21px'; the _value_ is always followed by a semicolon(;) ;
- **The style attribute**: one way to add CSS is through the _style_ attribute `<p style= "">` and write CSS inside the quotation marks: `<p style="font-size: 21px">`
