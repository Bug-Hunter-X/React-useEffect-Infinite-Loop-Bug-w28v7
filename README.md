# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency.  The `bug.js` file shows the erroneous code, while `bugSolution.js` provides the corrected version.

The issue arises when the `useEffect` hook's dependency array is missing a value that changes within the component's scope.  This leads to the effect running repeatedly, often causing performance issues or crashes.  The solution involves adding all values used within the effect to the dependency array.