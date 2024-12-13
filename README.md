# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook causing an infinite loop.  The bug arises from incorrectly managing dependencies within the `useEffect`'s dependency array, leading to continuous re-renders and potential application crashes.

## Bug Description
The `MyComponent` component uses `useState` to track a count. The `useEffect` hook attempts to increment the count in every render, resulting in an infinite loop because `count` is included in the dependency array and changes during the render cycle.