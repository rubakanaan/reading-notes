# Introduction to React and Components
<br>
<br>

## Component-Based Architecture:
<br>
<br>

### What is a Component?
* A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

* A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

* A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties.

<br>
<br>

### Characteristics of Components
* **Reusability** − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

* **Replaceable** − Components may be freely substituted with other similar components.

* **Not context specific** − Components are designed to operate in different environments and contexts.

* **Extensible** − A component can be extended from existing components to provide new behavior.

* **Encapsulated** − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

* **Independent** − Components are designed to have minimal dependencies on other components.

<br>
<br>

### Advantages

1. Ease of deployment
2. Reduced cost 
3. Ease of development 
4. Reusable 
5. Modification of technical complexity 
6. Reliability 
7. System maintenance and evolution 
8. Independent 

<br>
<br>

![comp](https://www.hebergementwebs.com/image/f7/f7ff2ce429c26c468e6e16a6f3e9f7c8.jpg/component-based-architecture.jpg)
<br>
<br>

# What is “Props” and how to use it in React?
<br>
<br>

![react](https://csharpcorner.azureedge.net/article/what-and-why-reactjs/Images/React%20Properties.jpg)
<br>

## What is Props?
*React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.*

***“Props”** is a special keyword in React, which stands for properties and is being used for passing data from one component to another.*

*But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)
Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.*


## Using Props in React
1. Firstly, define an attribute and its value(data)
2. pass it to child component(s) by using Props
3. Finally, render the Props Data

