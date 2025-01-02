# Unnecessary Re-renders in React's useEffect Hook

This repository demonstrates a common React performance issue: unnecessary re-renders caused by an inefficient `useEffect` hook. The `useEffect` hook, while powerful, needs careful management to avoid performance problems.

## Problem

The provided `bug.js` shows an example of a `useEffect` hook that runs after every render. This leads to unnecessary logging and potential performance problems, especially with more complex state updates.

## Solution

The solution (`bugSolution.js`) demonstrates how to use the dependency array in `useEffect` to control when the effect runs. By only including `count` in the dependency array, the effect will only run when `count` changes, resolving the unnecessary re-renders.

## How to Run

1. Clone the repository.
2. Navigate to the repository's directory in your terminal.
3. Run `npm install` to install the necessary dependencies.
4. Run `npm start` to start the development server.
