# React useEffect Runs After Every Render
This repository demonstrates a common React bug where the `useEffect` hook runs after every render, leading to performance issues and unexpected behavior.

## Bug Description
The `useEffect` hook in the provided code lacks a proper dependency array, causing it to execute after every render. This results in unnecessary re-renders and potential performance bottlenecks.  It can also lead to unexpected behavior in cases where asynchronous operations or side effects depend on the component's state.

## Solution
The solution involves correctly specifying the dependencies in the `useEffect` hook. This ensures that the effect only runs when a specific dependency changes. 