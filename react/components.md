# React components

This is a quick note about React components with comments.

A note about managing data flow:
- `top down` / `Unidirectional` data flow - pass the parent component's state (`prop`) to its child component

There are 2 types of react components:
- class-based components
- functional components

## class-based components
- uses `this` keyword when referring to  state + regular methods
- lifecycle methods (`componentDidMount()`, `componentWillMount()`, etc.)
- use the `bind` keyword when passing an argument to current component

```
class DoctorWho extends React.component {
   // local/encapsulated state and constructor
   // lifecycle methods
   // regular component methods
   // render() method
      // directives
      // return() method
}

## functional components
- no `this` keyword when referring to state + regular methods

```
const DoctorWho = props => {
   // hooks, such as useState
   // regular component methods
   // return() method
}
```


```
