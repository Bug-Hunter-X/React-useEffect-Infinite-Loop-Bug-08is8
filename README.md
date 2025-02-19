# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook: an infinite loop caused by an incorrect dependency array.

## The Bug
The `bug.js` file contains a `MyComponent` that uses the `useEffect` hook to log the current count to the console. However, the dependency array is missing, causing the effect to run on every render, leading to an infinite loop and potential performance issues.

## The Solution
The `bugSolution.js` file demonstrates the correct implementation. The dependency array `[count]` ensures that the effect runs only when the `count` value changes.