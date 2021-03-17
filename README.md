# Frontend Crash course

Frontend roughly means all of the code that goes into making a visual layer for your users, like a website. The standard way of making a web interface is by using HTML, then optionally some combination of CSS, javascript, and a backend that inserts relevant information into your HTML to make it more interactive and pretty.

### The DOM (Document-Object Model)
The DOM is the standard for thinking about frontend. The main idea of the DOM is that every webpage is represented by a HTML document that gives the basic structure, such as titles, paragraphs, tables of information, lists, forms, and so on. Any other code that wants to add interactivity to the page or make it more pretty can edit the document object to meet that goal. 


### HTML: The Bread and Butter of Frontend 
HTML is at the core of everything. It is the Document that forms the Document Object. It gives all of the structure to your webpage. A minimal webpage in HTML would look like,
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
  <!--Your HTML code goes here-->
  <h1>This is my website!</h1>
</body>
</html>
```

Note that everything in HTML uses tags as building blocks. Tags look like, 

```html
<tag_name> This is wrapped by the tag called tag_name. </tag_name>
```

Many useful tags with examples can be found at [W3Schools' website.](https://www.w3schools.com/html/default.asp) 

Here is a HTML document with some common tags,

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
  <!--This is a comment-->
  <h1>This is a type of (big) heading</h1>
  <h6>This is  S M A L L heading</h6>

  <p> This is a paragraph
  
      but going to a new line doesn't add a line break. HTML isn't sensitive to whitespace</p>
      
  <p> You need a separate paragraph to capture a new block</p>
  
  <a href="https://www.google.com">This is an anchor tag. They create links to wherever the href attribute is pointing.</a>
  
  
<div class="myClass">
    <p>divs and classes are very useful!</p>
</div>
  
  </body>
</html>
```

`div` tags create a container that isolates the inner HTML. This can be useful if you want to treat a section of your website in a special way - say coloring all of the inner text red. The `class="myClass"` attribute of the div tag can be used to locate this particular section since the name "myClass" is arbitrary. You can name classes whatever you'd like. We'll come back to this when we talk about CSS.


### Viewing HTML in the browser
To view HTML on your computer, you need to open the file in your browser. To do this, copy the full path to your html file and paste it in your browser. For example, the above HTML snippet is saved in `html_basics/common_tags.html`, which has the full path `/Users/mlawrence/Documents/GitHub/frontend-crashcourse/html_basics/common_tags.html` on my computer. We can paste this full path in Firefox or Chrome to look at our HTML file. 

After doing this, you should see something like the following:
![html in browser](./images/html_view.png)