# React Native AsyncStorage TypeError: Cannot read properties of null (reading '...')

This repository demonstrates a common error in React Native when using AsyncStorage: TypeErrors resulting from accessing properties of null values.  The error arises when attempting to read data from AsyncStorage using `AsyncStorage.getItem()` where the key does not exist.  The lack of explicit error handling in the code makes it difficult to identify the root cause.

The solution in `bugSolution.js` shows how to properly handle the case where `AsyncStorage.getItem()` returns null, preventing TypeErrors and ensuring robust data handling.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`. 
4. Observe the error in the console in the original `bug.js` file
5. Observe the correct behavior in `bugSolution.js`