# Component-Based Architecture

* A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

* A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

* A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties.

-----------------------

## Characteristics of Components

**Reusability** − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

**Replaceable** − Components may be freely substituted with other similar components.

**Not context specific** − Components are designed to operate in different environments and contexts.

**Extensible** − A component can be extended from existing components to provide new behavior.

**Encapsulated** − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

**Independent** − Components are designed to have minimal
dependencies on other components.

------------------------------------

## the advantages of using component based architecture

**Ease of deployment** − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

**Reduced cost** − The use of third-party components allows you to spread the cost of development and maintenance.

**Ease of development** − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

**Reusable** − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

**Modification of technical complexity** − A component modifies the complexity through the use of a component container and its services.

**Reliability** − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

**System maintenance and evolution** − Easy to change and update the implementation without affecting the rest of the system.

**Independent** − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

----------------------------

# Props

React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.

“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

### how to use Props step by step

 -----------
1- Firstly, define an attribute and its value(data)

2- Then pass it to child component(s) by using Props

3- Finally, render the Props Data

1st Step: Defining Attribute & Data
We already know that we can assign attributes and values to HTML tags:

``` <a href="www.google.com">Click here to visit Google</a>; ```

Likewise, we can do the same for React components. We can define our own attributes & assign values with interpolation { }:

``` <ChildComponent someAttribute={value} anotherAttribute={value}/> ```

2nd Step: Passing Data using Props

Passing props is very simple. Like we pass arguments to a function, we pass props into a React component and props bring all the necessary data.

Arguments passed to a function:

```
 const addition = (firstNum, secondNum) => {  
  return firstNum + secondNum; 
}; 
```

Arguments passed to a React component:

```
const ChildComponent = (props) => {  
  return <p>I'm the 1st child!</p>; 
};

```

Final Step: Rendering Props Data

Alright so far, we have created an attribute and its value, then we passed it through props but we still can’t see it because we haven’t rendered it yet.
