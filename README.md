# React 19 useEffect Dependency Issue

This repository demonstrates a common error related to the `useEffect` hook in React 19.  Improper use of the dependency array can cause infinite loops or incorrect state updates.  The `bug.jsx` file shows the problematic code, while `bugSolution.jsx` provides a corrected version.

## Problem

The `useEffect` hook in React is powerful, but forgetting to add dependencies to the dependency array leads to unexpected behavior.  Specifically, the useEffect hook might run on every render, even if there are no changes in relevant data.