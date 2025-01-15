# React useEffect Dependency Array Bug

This repository demonstrates a common mistake when using the `useEffect` hook in React: incorrectly specifying the dependency array, leading to unexpected behavior. 

## Bug Description
The `useEffect` hook is intended to perform side effects after a component renders.  In the provided example, the `console.log` statement is only executed once, after the initial render. This is because the dependency array is empty (`[]`).  To fix this, you need to include the `count` variable in the dependency array.