# Unhandled Promise Rejection in AsyncStorage

This repository demonstrates a common error in React Native applications involving unhandled promise rejections when using AsyncStorage.  Failure to properly handle rejected promises from AsyncStorage operations can lead to unexpected app behavior and crashes.

## Problem

The provided `bug.js` example shows how not handling rejected promises from AsyncStorage can result in silent failures.  If `setItem` or `getItem` fails, the application won't provide any indication of the error.

## Solution

The `bugSolution.js` file demonstrates the correct way to handle these rejections using `.catch()` to gracefully handle errors and provide informative feedback to the user.