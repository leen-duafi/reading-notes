**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

 ‘render’ happens **before** ‘componentDidMount’

**What is the very first thing to happen in the lifecycle of React?**

Mounting is the first phase of the component lifecycle of react.

**Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates**

* constructor
* render
* React Updates
* componentDidMount
* componentWillUnmount

**What does componentDidMount do?**

componentDidMount()
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.

**What types of things can you pass in the props?**

things that you passed as a function// you want to inzalize your compoenet to // what you want your component to render like 

**What is the big difference between props and state?**

* **state** is inside of the component // handaled inside of a component and you can update it inside of it // handling information inside a component and no where outside of it 


* **prpos** you pass into a component // handaled outside  of a component and must be  update it outside  of it // handling information outside  a component // static information and not going to change ((passed from parent and not going to change inside of it ))

**When do we re-render our application?**

when you change the state inside of an application but props you can not change them (( as you have to do it outside an component ))


**What are some examples of things that we could store in state**

* re-render and update you aplication based on something the user has done 
* counter application 
* inside of form ((input element / check box))
