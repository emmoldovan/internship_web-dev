index.html
<h1> Hello World </h1>

## `HTML`<br>
- `H`yper `T`ext `M`arkup `L`anguage <br>
`Hyper Text` = it has links in it. <br>
`Markup Language` = Language where you can write something that convanes meaning to the processor or browser or PC.
- The content of websites. <br>

- `<`cover`>`  `</`cover`>` an opening and closing tag is called an *element*. 

<cover>
    <page> Eu sunt Beni </page> <br>
    <page> Eu sunt Beni </page> <br>
    <page> Eu sunt Beni </page> <br>
</cover>

<br>

<page>
    <heading>Chapter 3  </heading> <br>
    <subheading>The light </subheading>
    <p>The clouds are shining </p>
</page>

- Tags are inside the of `<>`
- CLosing tags include a forward slash `</>`
- Everything from the opening and closing tag is called an `element`.

- The very first thing at the top of every document, tells the browser that this is an HTML 5 document.
`<!DOCTYPE>`
<html>
<head>
<title> (shows up in the tab of the browser and in search results)




<!DOCTYPE html>
<html>
  <head>

<title> My first website </title>

  </head>

   <body>
this is where the content goes. 
<p>are your regular text that you use. 

<h1>My very first webpage</h1>
<h2>I have learned that < p > is a paragraph tag</h2>
<h3> h1 is the tytle always, h6 is the least of fonts </h3>

   </body>

</html>

- text inside <strong> browser makes </strong> this text bold. 
- <em>the text makes the text italic</em>
we use those inside the paragraphs.
<p><strong>Worning:</strong> It's very cold out</p> 

<h2>`File Naming and  organization`</h2>

- Name the file that is describing the page. "about-us.html"
- No spaces in your names, use underscores or hyphens.
- Use lower case always.
- The main folder is called our `root folder`
- The homepage must be `index.html`
- `index.html must be in the root folder`, and not a sub-folder
- Other pages can be in subfolders, depending on how you want to stay organized. 
- Images should be placed in a sub folder for better organization.


<h2>HTML - Anchors and attributes </h2>

- <a> is used to make links, a= anchor
- <a>google</a>
- Elements can have `attributes`. `Attributes` are always within the opening tag. 
- `attributes` are normally followed by an equal sign and quotation marks
<a href="https://google.com">google</a>

- `some elements require an attribute` a link will not work without an `href` attribute.
- <a href="https://google.com">google</a>

- `Absolute paths` if the page you are linking to is NOT part of your website, `it MUST start with http:// or https://` to let the browser know it is an external site that you are linking too. if you dont add that in there and you just pus www.something.com its not going to work. you really need to have that in the beginning. 
- `Relative Paths` you can link to other pages within your site by simply putting their file name. 
- visit our <a href="about-us.html">about us</a> page!
- or if something is in a sub folder you put the folder name forword slash and than the file name. 
- visit our <a href="team/john.html">about us</a> page!

