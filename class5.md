# Class 05

## React Docs - Thinking in React

### What is the single responsibility principle and how does it apply to components?
  only do one thing, to map on correct way
### What does it mean to build a ‘static’ version of your application?
  that renders your data model without using state
### Once you have a static application, what do you need to add?
   The components will only have render()
### What are the three questions you can ask to determine if something is state?
* Is it passed in from a parent via props? If so, it probably isn’t state.
 * Does it remain unchanged over time? If so, it probably isn’t state.
* Can you compute it based on any other state or props in your component? If so, it isn’t state.
  
### How can you identify where state needs to live?
* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
---
## Higher-Order Functions

### What is a “higher-order function”?
functions that operate on other functions, either by taking them as arguments or by returning them
### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
return boleen value depends on the expretion

### Explain how either map or reduce operates, with regards to higher-order functions.
 The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.

---
## Things I want to know more about

clear the idea of using the state on many js files