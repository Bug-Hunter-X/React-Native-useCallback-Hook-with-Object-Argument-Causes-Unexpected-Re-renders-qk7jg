# React Native useCallback Hook with Object Argument Causes Unexpected Re-renders

This repository demonstrates a common issue when using the `useCallback` hook in React Native with functions that take objects as arguments.  Even if the object's content remains unchanged, React may treat it as a different object due to reference changes, leading to unnecessary re-renders.

The `useCallbackIssue.js` file showcases the problem, while `useCallbackSolution.js` provides a solution using `useMemo` to memoize the object, ensuring that `useCallback` receives the same object reference between renders. 

This approach prevents unnecessary re-renders and improves performance. Please refer to the solution file for a detailed explanation and implementation.
