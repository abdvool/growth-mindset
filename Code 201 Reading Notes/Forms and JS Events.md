# Forms

HTML borrows the concept of a form to refer to different
elements that allow you to collect information from visitors to
your site.

----------------
### Why Forms?
------------------
The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage

-------------

## Form Controls


![img](/img/f1.JPG)


--------

## Form Structure


![img](/img/f2.JPG)


------------

## Text input



![img](/img/f3.JPG)


------------


## Password Input


![img](/img/f4.JPG)


-----------


## Text Area


![img](/img/f5.JPG)


---------

## Check box

![img](/img/f6.JPG)







--------
## Drop Down List Box


![img](/img/f7.JPG)



--------------
## File Input Box




![img](/img/f8.JPG)



----------

## Example
```
<html>
<head>
<title>Forms</title>
</head>
<body>
<form action="http://www.example.com/review.php" method="get">
<fieldset>
<legend>
Your Details:
</legend>
<label>
Name:
<input type="text" name="name" size="30" maxlength="100">
</label>
<br />
<label>
Email:
<input type="email" name="email" size="30" maxlength="100">
</label>
<br />
</fieldset>
<br />
<fieldset>
<legend>
Your Review:
</legend>
<p>
<label for="hear-about">
How did you hear about us?
</label>
<select name="referrer" id="hear-about">
<option value="google">Google</option>
<option value="friend">Friend</option>
<option value="advert">Advert</option>
<option value="other">Other</option>
</select>
</p>
<p>

```