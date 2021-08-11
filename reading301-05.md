# [React Docs - thinking in React](https://reactjs.org/docs/thinking-in-react.html)
### How would you break a mock into a component heirarchy?
* by drawing boxes around components and subcomponents
### What is the single responsibility principle and how does it apply to components?
*it means that each component should have one thing to do, otherwise it needs to be broke down to smaller components.
### What does it mean to build a ‘static’ version of your application?
* it meands to have the ui ready but with no interaction.
### Once you have a static application, what do you need to add?
* the minimal but complete representation of us state

### What are the three questions you can ask to determine if something is state?
* Is it passed in from a parent via props? If so, it probably isn’t state.
* Does it remain unchanged over time? If so, it probably isn’t state.
* Can you compute it based on any other state or props in your component? If so, it isn’t state.
### How can you identify where state needs to live?
* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.


## Things I want to know more about
how to avoid new comers challenges.
