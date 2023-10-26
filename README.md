# react-training-guide

# React Training

## React Component Lifecycle

React components go through a series of events, from mounting to unmounting, which can be summarized as follows:

- **Mounting**: Birth of the component
- **Updating**: Growth of your component
- **Unmounting**: Death of your component

### Methods in React Component Lifecycle

1. `Render()`
   - The `render` method is used to render the HTML of your React component. It is required for a class-based component to render the DOM.
   - It runs during both mounting and updating of the component.
   - `render()` should be pure, meaning you cannot modify the state inside it.

2. `componentDidMount()`
   - Runs after the component has been rendered on the DOM.

3. `componentDidUpdate()`
   - Invoked as soon as updating happens. The most common use case for this method is updating the DOM in response to prop or state changes.

4. `componentWillUnmount()`
   - Invoked just before the component is being unmounted and destroyed. This method is usually used for cleanups.

## Component

To create a class component, you need to do the following:

1. Extend the class with the base class of `Component`:

   ```javascript
   import { Component } from 'react';

   class Welcome extends Component {
   }

```
