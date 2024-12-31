# React Native: Unhandled TypeError: Cannot read properties of undefined (reading 'property')

This repository demonstrates a common React Native error:  `TypeError: Cannot read properties of undefined (reading 'property')`.  This occurs when attempting to access a property of an object that's currently undefined or null. This is particularly prevalent when working with asynchronous data fetching.

The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version implementing optional chaining and nullish coalescing.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app (using a React Native simulator or device).
4. Observe the error in the console (in `bug.js`) and the corrected behavior in `bugSolution.js`.

## Solution

The primary solution involves using optional chaining (`?.`) and the nullish coalescing operator (`??`).  Optional chaining prevents errors when accessing nested properties on potentially nullish objects.  Nullish coalescing provides a default value if the property is null or undefined.  These techniques enhance robustness and prevent application crashes.