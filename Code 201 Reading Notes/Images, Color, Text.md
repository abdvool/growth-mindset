# Images, Color, Text


## Image
----------
There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.

There are several things to consider when selecting and
preparing images for your site, but taking time to get them
right will make it look more attractive and professional.
In this chapter you will learn how to:

* include an image in your web pages using HTML
* Pick which image format to use
* Show an image at the right size
* Optimize an image for use on the web to make pages
load faster

------------
### Adding Images
--------------
* **< img >**
To add an image into the page
you need to use an < img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:


* **src**
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images 

* **alt**
This provides a text description
of the image which describes the
image if you cannot see it.

* **title**
You can also use the title
attribute with the < img> element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.

![img](/img/img.JPG)

-----------------------------

## Height & Width of Images

You will also often see an < img>
element use two other attributes
that specify its size:

* **height**
This specifies the height of the image in pixels.

* **width**
This specifies the width of the
image in pixels.
Images often take longer to
load than the HTML code that
makes up the rest of the page.
It is, therefore, a good idea to
specify the size of the image
so that the browser can render
the rest of the text on the page
while leaving the right amount of
space for the image that is still
loading.

![img](/img/img2.JPG)

------------
## HTML5: figure and figure Caption


* **< figure >**
Images often come with
captions. HTML5 has introduced
a new < figure> element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the < figure>
element as long as they all share
the same caption.

* **< figcaption >**
The < figcaption> element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.
 
 ![img](/img/img3.JPG)

 --------------------

 ## Color
 -----------
 ### Foreground Color

 ![img](/img/img4.JPG)

----------
 ### Background Color

  ![img](/img/img5.JPG)
  -------------

  ### Understanding Color

  Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.

 ![img](/img/img6.JPG)

 -----------------


## Text

-------------
The properties that allow you to control
the appearance of text can be split into
two groups:

* Those that directly affect t ●● he font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)
* Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)



-------------
### Size of Type

![img](/img/img7.JPG)

-------------

### Bold font-weight

The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:

normal
This causes text to appear at a
normal weight.
bold
This causes text to appear bold.
In this example, you can see
that the element whose class
attribute has a value of credits
has been bolded.

![img](/img/img8.JPG)

-------------

### Italic font-style

![img](/img/img9.JPG)

------------


### UpperCase & LowerCase
text-transform

---------
* uppercase

```
h1 {
text-transform: uppercase;}

 ```

 * lowercase
```
h2 {
text-transform: lowercase;}
```

--------------
### Underline & Strike
text-decoration

![img](/img/img10.JPG)

------------

### Leading
line-height

Leading (pronounced ledding) is
a term typographers use for the
vertical space between lines of
text. In a typeface, the part of
a letter that drops beneath the
baseline is called a descender,
while the highest point of a letter
is called the ascender. Leading
is measured from the bottom of
the descender on one line to the
top of the ascender on the next.


```
p {
line-height: 1.4em;}
```
------------


### Letter & Word Spacing
letter-spacing, word-spacing

![img](/img/img11.JPG)

------

### Alignment
text-align

![img](/img/img12.JPG)

-------------

### Vertical Alignment
vertical-align


![img](/img/img13.JPG)
------------

### Indenting Text
text-indent


![img](/img/img14.JPG)
---------
### CSS3: Drop Shadow
text-shadow


![img](/img/img15.JPG)

----------

### First Letter or Line
:first-letter, :first-line

![img](/img/img16.JPG)


-----------

### Responding to Users
:hover, :active, :focus

![img](/img/img17.JPG)
----------

### Attribute Selectors


![img](/img/img50.JPG)
----------

## Example

```
<!DOCTYPE html>
<html>
<head>
<title>Text</title>
<style type="text/css">
body {
padding: 20px;}
h1, h2, h3, a {
font-weight: normal;
color: #0088dd;
margin: 0px;}
h1 {
font-family: Georgia, Times, serif;
font-size: 250%;
text-shadow: 2px 2px 3px #666666;
padding-bottom: 10px;}
h2 {
font-family: "Gill Sans", Arial, sans-serif;
font-size: 90%;
text-transform: uppercase;
letter-spacing: 0.2em;}
h3 {
font-size: 150%;}
p {
font-family: Arial, Verdana, sans-serif;
line-height: 1.4em;
color: #665544;}
p.intro:first-line {
font-weight: bold;}
.credits {
font-style: italic;
text-align: right;}
a {
text-decoration: none;}
a:hover {
text-decoration: underline;}
</style>
</head>

```

```
<body>
<h1>Briards</h1>
<h2>A Heart wrapped in fur</h2>
<p class="intro">The <a class="breed" href="http://en.wikipedia.org/wikiBriard">
briard</a>, or berger de brie, is a large breed of dog traditionally used as a
herder and guardian of sheep.</p>
<h3>Breed History</h3>
<p>The briard, which is believed to have originated in France, has been bred for
centuries to herd and to protect sheep. The breed was used by the French Army as
sentries, messengers and to search for wounded soldiers because of its fine sense
of hearing. Briards were used in the First World War almost to the point of
extinction. Currently the population of briards is slowly recovering.
Charlemagne, Napoleon, Thomas Jefferson and Lafayette all owned briards.</p>
<p class="credits">by Ivy Duckett</p>
</body>
</html>
```