# React useEffect Infinite Loop
This repository demonstrates a common React bug: an infinite loop caused by improperly using the `useEffect` hook.  The `useEffect` hook, while powerful, can easily lead to infinite renders if not handled correctly.

The `bug.js` file contains the buggy code, where the state variable `count` is updated within the `useEffect` hook which depends on the `count` variable itself.  This creates a cycle where every update to `count` triggers a re-render and another update, resulting in an infinite loop. 

The `bugSolution.js` file provides the corrected code by updating the state in a conditional way that avoids the infinite loop. 