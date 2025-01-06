# React useEffect Hook Bug

This repository demonstrates a common bug in React's `useEffect` hook where missing dependencies lead to unexpected re-renders. The bug is explained and the solution is provided.

## Bug Description

The `useEffect` hook in the `bug.js` file is intended to log a message only once on component mount. However, due to a missing dependency, it runs after every render. This causes unnecessary logging and potentially performance issues. 

## Solution

The `bugSolution.js` file demonstrates the solution. The missing dependency is added to the dependency array, ensuring the effect runs only when the dependency changes.  This solves the unexpected re-renders.

## How to Reproduce

1. Clone the repository.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the React development server. Observe the console for the frequent logging in `bug.js` and the corrected behavior in `bugSolution.js`