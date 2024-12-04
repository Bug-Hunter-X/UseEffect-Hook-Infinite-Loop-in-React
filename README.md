# useEffect Hook Infinite Loop in React

This repository demonstrates a common error in React applications involving the `useEffect` hook.  The issue arises when the `useEffect` hook is used without a dependency array, causing it to run after every render, potentially leading to an infinite loop or unexpected behavior. The solution shows how to correctly utilize the dependency array to control when the effect runs.

## Problem

The provided `bug.js` code snippet shows an `useEffect` hook without a dependency array. This results in the effect running after every render, logging the current `count` to the console. As the `setCount` function is called during each click event, this leads to an infinite loop.