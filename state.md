# State and Props

What are component lifecycle events?
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.
Mounting, Updating, and Unmounting are the three phases of the component lifecycle.
![lif](https://miro.medium.com/max/1200/1*EnuAy1kb9nOcFuIzM49Srw.png)
![life](https://cdn-media-1.freecodecamp.org/images/1*_drMYY_IEgboMS4RhvC-lQ.png)

1. constructor():
    * The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance.
2. render():
    * Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false. 


## **What types of things can you pass in the props?**

**props enable you to pass variables from one to another component down the component tree.**

## **What is the big difference between props and state?**
 **the difference is that state is something like attributes in OOP : it's something local to a class (component), used to better describe it. Props are like parameters - they are passed to a component from the caller of a component (the parent) : as if you called a function with certain parameters.**

## **What are some examples of things that we could store in state?**

 **whenever we are working with any data, we always use state for storing that data which may be a string , number or any complex object .**