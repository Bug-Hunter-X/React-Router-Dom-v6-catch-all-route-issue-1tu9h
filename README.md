# React Router Dom v6 Catch All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6. The catch-all route, intended to handle any unmatched routes, can unintentionally interfere with other routes, preventing them from matching correctly. 

## Problem Description

The `/*` route, while useful for handling 404 errors, can incorrectly catch other routes if it's placed incorrectly or if other routes are not structured properly. This can result in other defined routes not rendering, even if the path matches. 

## Solution

The issue can be resolved by ensuring that the catch-all route is placed as the last route defined in the `Routes` component. This allows other, more specific, routes to be matched first before the catch-all route is evaluated. 

## How to reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe that the `/about` route does not work correctly. 
5. Check the solution file to see how the issue is fixed. 

## Technologies Used

* React
* React Router Dom v6
