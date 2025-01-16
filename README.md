# React useEffect setInterval Memory Leak

This repository demonstrates a common error in React applications: using `setInterval` within a `useEffect` hook without providing a cleanup function. This leads to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a React component that uses `setInterval` to update a counter every second. However, it fails to provide a cleanup function to clear the interval when the component unmounts, leading to a memory leak.

## Solution
The `bugSolution.js` file demonstrates the correct usage of `setInterval` within `useEffect`, including a cleanup function to stop the interval when the component unmounts.