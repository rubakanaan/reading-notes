# LAYOUT 
### Key Concepts in Positioning Elements:

#### Building Blocks
*CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks
of any layout, while inline boxes flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.* 

#### Containing Elements
*If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.
It is common to group a number of elements together inside a \<div>
(or other block-level) element. For example, you might group together
all of the elements that form the header of a site (such as the logo and
the main navigation). The \<div> element that contains this group of
elements is then referred to as the containing element.*

### NORMAL FLOW 
1. position:static
2. position:relative
3. position:absolute
4. position:fixed

![flow](https://www.csssolid.com/images/csspositions/css-position-all.png)


### Clearing Floats:
*The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand sides of a box. It can take
the following values:*
1. left:
    * The left-hand side of the box
should not touch any other
elements appearing in the same
containing element.
2 .right:
    * The right-hand side of the
box will not touch elements
appearing in the same containing
element.
3. both
    * Neither the left nor right-hand
sides of the box will touch
elements appearing in the same
containing element.
4. none :
    * Elements can touch either side.

![float](https://miro.medium.com/max/540/1*gL79pBRvVlMjX0Ovevz96w.png)