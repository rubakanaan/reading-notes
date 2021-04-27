
# Transforms

*With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.
The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.*

![transform](https://www.vanamco.com/wp-content/uploads/2014/07/css-transition-tips.jpg)

## 2D Transforms
1. Rotate : transform: rotate(20deg);
2. Scale :   transform: scale(.75);
3. Translate : transform: translateX(-10px);
4. Skew :  transform: skewX(5deg);

![rot](https://miro.medium.com/max/1440/1*_NVMTnvHTM9teQxrVRlDeg.png)

## Combining Transforms
*It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.*
*  transform: rotate(25deg) scale(.75);
*  transform: skew(10deg, 20deg) translateX(20px);


# Transitions & Animations

*for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.*
![trans](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)

## 8 SIMPLE CSS3 TRANSITIONS
1. Fade in
2. Change color
3. Grow & Shrink
4. Rotate elements
5. Square to circle
6. 3D shadow
7. Swing
8. Inset border

