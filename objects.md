# OBJECT 
## WHAT IS AN OBJECT?
*Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.*

* IN AN OBJECT:
    *  VARIABLES BECOME
KNOWN AS PROPERTIES
If a variable is part of an object, it is called a
property. Properties tell us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.
* IN AN OBJECT:
    * FUNCTIONS BECOME
KNOWN AS METHODS
If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms. 


* ![obj](https://res.cloudinary.com/practicaldev/image/fetch/s--rJeH0yGE--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/t52ni02srb8688lh3eh8.png)

* ![objAccess](https://dmitripavlutin.com/static/50a87420915de18f26da616865fe9825/05127/access-object-properties-2.png)


# DOCUMENT OBJECT MODE

*The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.*

![dom](https://cf.ppt-online.org/files/slide/l/lG6hjyFR8carDYH7oVAtPW3exEOg0sSpQ1JKfm/slide-4.jpg)



## WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 

## CATCHING DOM QUIERIES
1. getElementById(' id'):
    * Selects an individual element given the value of its i d attribute .The HTML must have an id attribute in order for it to be selectable.
2. querySelector('css selector'):
    * Uses CSS selector syntax that would select one or more elements .
This method returns only the first of the matching elements. 
3. getEl ementsByClassName('class'):
    * Selects one or more elements given the value of their cl ass attribute.
The HTML must have a cl ass attribute for it to be selectable.
This method is faster than querySe 1ectorA11 () . 
4. getEl ementsByTagName( 'tagName') :
    * Selects all elements on the page with the specified tag name.
This method is faster than querySe 1ectorA11 (). 
5. querySelectorAll ( 'css selector'):
    * Uses CSS selector syntax to select one or more elements and returns all
of those that match. 