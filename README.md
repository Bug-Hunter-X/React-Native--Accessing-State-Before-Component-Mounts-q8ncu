# React Native: Accessing State Before Component Mounts

This repository demonstrates a common error in React Native development: accessing a component's state or props before it has mounted.  The `Bug.js` file shows the problematic code, while `BugSolution.js` provides the corrected version.

## Problem

Attempting to use component state or props before the component has fully mounted leads to unexpected behavior, often resulting in `undefined` or `null` values causing app crashes or unexpected rendering.

## Solution

The solution involves leveraging the useEffect hook and making sure values are checked for null or undefined before use.