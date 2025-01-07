# React useEffect Hook Missing Cleanup Function

This repository demonstrates a common error in React's `useEffect` hook: forgetting to include a return statement for cleanup.  This can lead to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a component with an `useEffect` hook that's missing a return statement.  This means that the cleanup function, which is crucial for tasks like event listeners or subscriptions, is not executed when the component unmounts or updates.

## Solution
The `bugSolution.js` file shows the corrected code.  A return statement is added to the `useEffect` hook, ensuring proper cleanup.

## How to reproduce
1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install`.
4. Run `npm start`.
5. Observe the console output and note the absence or presence of cleanup messages.
