# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6. The catch-all route is intended to handle any unmatched routes, but in this case, it's incorrectly intercepting all requests, even those that match defined routes.

The problem stems from the order of routes and the behavior of the `/*` wildcard. By placing the `/*` route before more specific routes, it matches before other routes have the chance to. The solution involves reordering routes to place the catch-all route last.