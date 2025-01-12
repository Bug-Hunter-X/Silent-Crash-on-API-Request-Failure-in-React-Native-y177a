# Silent Crash on API Request Failure in React Native

This repository demonstrates a common issue in React Native applications where an unhandled promise rejection occurs during API data fetching. The app crashes silently without displaying any error message to the user.

## Problem

The `DataFetch.js` file contains a component that fetches data from an API. If the API request fails, the application crashes silently due to an unhandled promise rejection.  This makes debugging and providing a good user experience difficult.

## Solution

The `DataFetchSolution.js` file provides a solution to this problem by using a `try...catch` block within the `useEffect` hook to handle potential errors during the API request.  This ensures that an error message is displayed to the user instead of a silent crash.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run the app (e.g., using Expo).
4. Observe the silent crash when the API request fails. (You'll need to modify the API URL to a failing endpoint to trigger this.)
5. Modify your project to use `DataFetchSolution.js` for a working solution.
