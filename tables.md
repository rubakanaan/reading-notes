# TABLES
*There are several types of information
that need to be displayed in a grid or
table. For example: sports results, stock
reports, train timetables.*

## What's a Table?
*A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.*

## Basic Table Structure:
![table](https://www.programmersought.com/images/293/b6fbb1c243d343d19d8e11cc65bc8035.png)


# OBJECT , FUNCTIONS AND METHODS

![obj](https://flaviocopes.com/how-to-inspect-javascript-object/looping-properties.png)

### THIS (IT IS A KEYWORD) :
*The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates.*

### A METHOD OF AN OBJECT
When a function is defined inside an object, it
becomes a method. In a method, this refers to the
containing object. <br>
In the example below, the getArea () method
appears inside the shape object, so t his refers to
the shape object it is contained in:<br>

var shape = { <br>
width : 600; <br>
height : 400; <br>
 getArea : function() { <br>
     return this.width * this.height; <br>
} <br>
}; <br>


## THE BROWSER OBJECT MODEL: THE WINDOW OBJECT 
![BROM](https://image.slidesharecdn.com/ch13javascript6-150930234153-lva1-app6892/95/javascript-objects-50-638.jpg?cb=1443657692)
![BRO](https://image.slidesharecdn.com/javascript-200121065050/95/java-script-9-638.jpg?cb=1579589609)