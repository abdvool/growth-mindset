# HTML 

**HTML** (Hypertext Markup Language) it's a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on.  For example, take the following line of content:

**My cat is very grumpy**

If we wanted the line to stand by itself, we could specify that it is a paragraph by enclosing it in paragraph tags:


> **<p>My cat is very grumpy</p>**




## Anatomy of an HTML element

Let's explore this paragraph element a bit further.

![img](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)


#### The main parts of our element are as follows:

1.**The opening tag**: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.

2.**The closing tag**: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.

3.**The content**: This is the content of the element, which in this case, is just text.

4.**The element**: The opening tag, the closing tag, and the content together comprise the element


#### Elements can also have attributes that look like the following:

![elements](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-attribute-small.png)

Attributes contain extra information about the element that you don't want to appear in the actual content. Here, ``class`` is the attribute name and ``editor-note`` is the attribute value. The ``class`` attribute allows you to give the element a non-unique identifier that can be used to target it (and any other elements with the same ``class`` value) with style information and other things.



## Anatomy of an HTML document

That wraps up the basics of individual HTML elements, but they aren't handy on their own. Now we'll look at how individual elements are combined to form an entire HTML page. Let's revisit the code we put into our index.html example  


```

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image">
  </body>
</html>

```

# Semantics

In programming, Semantics refers to the meaning of a piece of code 


In HTML, for example, the <h1> element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."


``` 
<h1> This is a top level heading </h1>.
 ```





#  Wireframe

Wireframing is a practice used by UX designers which allows them to define and plan the information hierarchy of their design for a website, app, or product. This process focuses on how the designer or client wants the user to process information on a site, based on the user research already performed by the UX design team.

When designing for the screen you need to know where all the information is going to go in plain black and white diagrams before building anything with code. Wireframing is also a great way of getting to know how a user interacts with your interface, through the positioning of buttons and menus on the diagrams.

Without the distractions of colors, typeface choices or text, wireframing lets you plan the layout and interaction of your interface. A commonly-used argument for wireframing is that if a user doesn’t know where to go on a plain hand-drawn diagram of your site page, then it is irrelevant what colors or fancy text eventually get used. A button or call to action needs to be clear to the user even it’s not brightly colored and flashing.

## Examples of wireframes


Before you start designing the wireframes of your own app or product, take a look at some examples of wireframes. This will give you some inspiration for your own wireframes, as well as giving you an idea of the variety of ways of creating them. Some people like to draw their wireframes by hand, others feel more comfortable using software like Invision, or Balsamiq to create theirs. We’ll go through some of the tools you can use to create wireframes shortly, but it’s important to emphasize that how you make yours is up to you: some people feel more creative when sat at their computer, while others prefer to have a pen and paper in hand.

That said, for complete beginners, bear in mind the following when deciding on your wireframe creation process:


* Wireframes drawn with paper and a pencil, or at a whiteboard, have the advantage of looking and being very easy to change, which can help tremendously in early conversations about your website or product.

* With the help of paper-prototypes, you can test with end users at every stage of ideation and design. Changes at these stages are much easier—and therefore cheaper—than changes deemed necessary after coding is under way.

*It’s likely to be to your advantage to start off hand-drawing your wireframes before executing more detailed versions using an online app or software. The following wireframes should give you a good idea of how information can be organized on the screen.

![img](https://d33wubrfki0l68.cloudfront.net/dbb80f2f6a5dafa25f702ad00bc429057fb59cec/52716/en/blog/uploads/versions/samuel-student-wireframe---x----972-715x---.png)




