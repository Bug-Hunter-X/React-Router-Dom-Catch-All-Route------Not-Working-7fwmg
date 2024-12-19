# React Router Dom Catch-All Route Issue

This repository demonstrates a problem with the catch-all route `/*` in `react-router-dom`. The catch-all route is intended to match any route that doesn't match any other route, but in this case, it only matches the root path ('/') and not any other unexpected path.

## Problem Description:

The application uses `react-router-dom` to handle routing.  The `App.js` file includes a catch-all route `/*` to handle 404 errors. However, this route doesn't function as intended; only the root path ('/') works correctly.  Other paths, for example, '/contact', do not trigger the 404 page but rather cause a blank page or unpredictable behavior.

## Solution:

The solution demonstrates a correct implementation, utilizing the `useLocation` hook to provide more informative error messages and to ensure the catch-all route correctly handles all unmatched paths. The issue was resolved by fixing the route order and using a more robust error handling approach.