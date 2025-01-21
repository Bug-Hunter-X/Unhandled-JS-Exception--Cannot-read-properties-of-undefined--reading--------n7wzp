# Unhandled JS Exception: Cannot read properties of undefined (reading '...') in React Native

This repository demonstrates a common error in React Native applications: attempting to access a state variable before it has been initialized.  The error typically manifests as `Unhandled JS Exception: Cannot read properties of undefined (reading '...')`. This often occurs when dealing with asynchronous operations like API calls or delayed state updates.

## Problem

The `bug.js` file shows an example of improper state access, leading to the error. The component attempts to render data from the state before the data has been fetched.

## Solution

The `bugSolution.js` file illustrates a corrected approach.  It utilizes a conditional rendering technique to ensure that the component only renders data after the state has been properly populated.  This prevents the `undefined` error.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` or `yarn install`.
4. Run the app using `npx react-native run-android` or `npx react-native run-ios`.
5. Observe the error in `bug.js` and the corrected behavior in `bugSolution.js`.