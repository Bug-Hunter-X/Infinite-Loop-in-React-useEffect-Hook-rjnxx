# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` Hook.  The bug leads to an infinite rendering loop due to a missing dependency in the `useEffect` call.  The solution demonstrates the correct way to handle dependencies to prevent this issue.

## Bug Description
The `useEffect` Hook is used to perform side effects in functional components. When a dependency is missing from the dependency array, it causes the effect to run on every render, leading to an infinite loop.

## Solution
The solution adds the `count` state variable to the dependency array. This ensures that the effect runs only when the `count` value changes.