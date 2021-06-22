# HTML



## list
------------
There are lots of occasions when we need to use lists. HTML provides us with three different types:

* **Ordered lists●** are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number

* **Unordered lists●** are lists that begin with a bullet point (rather than characters that indicate order).

* **Definition lists●** are made up of a set of terms along with the definitions for each of those terms.
-------------

### Ordered Lists

 < ol >
 The ordered list is created with the < ol > element




 < li >
 Each item in the list is placed between an opening < li > tag and a closing < /li > tag. (The listands for list item.)


  ```
 <ol>
   <li>Chop potatoes into quarters</li>
   <li>Simmer in salted water for 15-20        minutes until tender</li>
   <li>Heat milk, butter and nutmeg</li><li>Drain potatoes and mash</li>
   <li>Mix in the milk mixture</li>
</ol>
 ``` 
 result 
  <ol>
   <li>Chop potatoes into quarters</li>
   <li>Simmer in salted water for 15-20        minutes until tender</li>
   <li>Heat milk, butter and nutmeg</li><li>Drain potatoes and mash</li>
   <li>Mix in the milk mixture</li>
</ol>

-------------

### Un Ordered Lists

< ul >
The unordered list is created with the < ul > element.

< li >

````
<ul> 
    <li>1kg King Edward potatoes</li> 
    <li>100ml milk</li> 
    <li>50g salted butter</li> 

    <li>Freshly grated nutmeg</li> 
    <li>Salt and pepper to taste</li>
     </ul>
````

result 

<ul>  <li>1kg King Edward potatoes</li>  <li>100ml milk</li>  <li>50g salted butter</li>  <li>Freshly grated nutmeg</li>  <li>Salt and pepper to taste</li></ul>

-------------------

### definition Lists


< dl >

The definition list is created with the < dl > element and usually consists of a series of terms and their definitions.Inside the < dl > element you will usually see pairs of < dt > and < dd > elements.

< dt >

This is used to contain the term being defined (the definition term)

< dd >This is used to contain the definition.Sometimes you might see a list where there are two terms used for the same definition or two different definitions for the same term

```
<dl> 
    <dt>Sashimi</dt>
    <dd>Sliced raw fish that is served with condiments such as shredded daikon radish or ginger root, wasabi and soy sauce</dd> 
    <dt>Scale</dt> 
    <dd>A device used to accurately measure the weight of ingredients</dd>

    <dd>A technique by which the scales are removed from the skin of a fish</dd> 
    <dt>Scamorze</dt> 
    <dt>Scamorzo</dt> 
    <dd>An Italian cheese usually made from whole cow's milk (although it was traditionally made from buffalo milk)</dd>
       
</dl>
```
result 

<dl>  <dt>Sashimi</dt>  <dd>Sliced raw fish that is served with condiments such as shredded daikon radish or ginger root, wasabi and soy sauce</dd>  <dt>Scale</dt>  <dd>A device used to accurately measure the weight of ingredients</dd>  <dd>A technique by which the scales are removed from the skin of a fish</dd>  <dt>Scamorze</dt>  <dt>Scamorzo</dt>  <dd>An Italian cheese usually made from whole cow's milk (although it was traditionally made from buffalo milk)</dd></dl>

-----------------

# ARRAYS

An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 

You should consider using an
array whenever you are working
with a list or a set of values that
are related to each other. 

----
## CREATING AN ARRAY 
![img](/img/arr1.JPG)

----
## VALU ES IN ARRAYS 
![img](/img/arr2.JPG)


---
## ACCESSING & CHANGING VALUES IN AN ARRAY
![img](/img/arr3.JPG)

----------

# JS
------
## If.. else statement 

the if ... else statement checks a condition
if it resolves to true the first code block is executed
if the condition resolves to false the second code black is run instead

![img](/img/j1.JPG)


-----

## using if else statements

![img](/img/j2.JPG)

---------

## switch statements


![img](/img/j3.JPG)

-------

## USING SWITCH STATEMENTS 


![img](/img/j4.JPG)


----------
# TRUTHY & FALSY VALUES

Due to type coercion, every value in JavaScript
can be treated as if it were true or false; and
this has some interesting side effects.


![img](/img/j5.JPG)
