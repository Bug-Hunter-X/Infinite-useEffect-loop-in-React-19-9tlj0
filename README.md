# React 19 Infinite useEffect Loop Bug

This repository demonstrates a common bug in React 19 applications involving an infinite loop within a `useEffect` hook.  The bug is caused by improper use of the `useEffect` hook's dependency array, leading to unnecessary re-renders and potentially crashing the application.

## Bug Description
The provided code snippet uses `useEffect` without specifying a dependency array. This means the effect runs after every render, causing the `console.log` statement to execute continuously, which is not only inefficient but also can easily lead to browser slowdowns or crashes. The core issue lies in the absence of a dependency array to control when the effect should run.