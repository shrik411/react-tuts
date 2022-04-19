# react-tuts
React prep help


## UseReducer

useReducer(reducer, initialState)

nweState = reducer(currentState, action)

Example

```
const initialState = 0;

const reducer = (state, action) => {
    switch(action) {
        case 'increment':
            return state + 1;
        case 'reset':
            return initialState
        break
    }
}

const [count, dispatch] = useReducer (reducer, initialState)

{ () => dispatch('increment') }
```

1. What are Pure Components?
React.PureComponent is exactly the same as React.Component except that it handles the shouldComponentUpdate() method for you. When props or state changes, PureComponent will do a shallow comparison on both props and state. Component on the other hand won't compare current props and state to next out of the box. Thus, the component will re-render by default whenever shouldComponentUpdate is called.

2. What are synthetic events in React?
SyntheticEvent is a cross-browser wrapper around the browser's native event. Its API is same as the browser's native event, including stopPropagation() and preventDefault(), except the events work identically across all browsers.



