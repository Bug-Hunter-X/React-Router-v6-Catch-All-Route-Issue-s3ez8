# React Router v6 Catch All Route Issue

This repository demonstrates a common issue with catch-all routes (`/*`) in React Router v6.  The catch-all route unintentionally overrides other routes, causing the 404 component to always render. 

## Problem
The `/*` route in the provided `App.js` example is always triggered, regardless of whether more specific routes exist and match the URL.

## Solution
The `AppSolution.js` file shows the corrected code.  The order of routes matters. The catch-all route should be placed last.   In addition, more specific routes should be placed before less specific routes.