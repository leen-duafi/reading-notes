# Thinking in React

**How would you break a mock into a component heirarchy?**

* The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names


* Now that we’ve identified the components in our mock, let’s arrange them into a hierarchy. Components that appear within another component in the mock should appear as a child in the hierarchy


* Now that you have your component hierarchy, it’s time to implement your app. The easiest way is to build a version that takes your data model and renders the UI but has no interactivity.


* make your UI interactive, you need to be able to trigger changes to your underlying data model. 
React achieves this with state.


* Identify Where Your State Should Live


* Add Inverse Data Flow


**What is the single responsibility principle and how does it apply to components?**



 computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part. All of that module, class or function's services should be narrowly aligned with that responsibility




a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.


**What does it mean to build a ‘static’ version of your application?**

 you’ll want to build components that reuse other components and pass data using props

 don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.


**Once you have a static application, what do you need to add?**

figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand.

**What are the three questions you can ask to determine if something is state?**



* Is it passed in from a parent via props? If so, it probably isn’t state.
* Does it remain unchanged over time? If so, it probably isn’t state.
* Can you compute it based on any other state or props in your component? If so, it isn’t state.



**How can you identify where state needs to live?**


* Identify every component that renders something based on that state.

* Find a common owner component (a single component above all the components that need the state in the hierarchy).


* Either the common owner or another component higher up in the hierarchy should own the state.


* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.