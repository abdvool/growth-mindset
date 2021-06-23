# HTML

-----------------------
## Links
* Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.

* Links are created using the < a > element. Users can click on anything
between the opening < a > tag and the closing < /a> tag. You specify
which page you want to link to using the href attribute.


![img](/img/h1.JPG)


`````
<p>Movie Reviews:
<ul>
<li><a href="http://www.empireonline.com">
Empire</a></li>
<li><a href="http://www.metacritic.com">
Metacritic</a></li>
<li><a href="http://www.rottentomatoes.com">
Rotten Tomatoes</a></li>
<li><a href="http://www.variety.com">
Variety</a></li>
</ul>
</p>
`````
the result 
<p>Movie Reviews:
<ul>
<li><a href="http://www.empireonline.com">
Empire</a></li>
<li><a href="http://www.metacritic.com">
Metacritic</a></li>
<li><a href="http://www.rottentomatoes.com">
Rotten Tomatoes</a></li>
<li><a href="http://www.variety.com">
Variety</a></li>
</ul>
</p>

------------

## Relative URLs

* Relative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.


* When you are linking to a page on your own website, you do not need to specify the domain name. You can use relative URLs which are a shorthand way to tell the browser where a page is in relation to the current page.

* This is especially helpful when creating a new website or learning about HTML because you can create links between pages when they are only on your personal computer (before you have got a domain name and uploaded them to the web).


![img](/img/h2.JPG)

-----------------
## Opening Links in a new window

target If you want a link to open in a new window, you can use the target attribute on the opening < a > tag. The value of this attribute should be _blank. 


One of the most common reasons a web page author might want a link to be opened in a new window is if it points to another website. In such cases, they hope the user will return to the window containing their site after finishing looking at the other one.

```
<a href="http://www.imdb.com" target="_blank">
Internet Movie Database</a> (opens in new window)
```
result 

<a href="http://www.imdb.com" target="_blank">
Internet Movie Database</a> (opens in new window)

----------------

# Java

---------

## Function


FUNCTION DECLARATION is the easiest one to creates a function that you can call later in your code. 

It is the type of function you have seen so far in this book. In order to call the function later in your code, you must give it a name, so these are known as named functions. Below, a function called area() is declared, which can then be called using its name.


```

function area (width, height){
return width * height;
};
var size= area(3, 4) ;

````

------------------
