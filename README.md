# Unhandled Server Error in Node.js
This repository demonstrates a common error in Node.js server development: unhandled errors during request processing.  The example shows a basic HTTP server that lacks proper error handling, leading to potential crashes and unpredictable behavior.  The solution provides a more robust approach to error management.

## Problem
The provided `serverBug.js` file shows a basic HTTP server. However, it lacks robust error handling. If any error occurs during the request/response cycle (e.g., network issues, unexpected request data), the server will crash without providing any helpful information.

## Solution
The solution, `serverSolution.js`, demonstrates improved error handling.  It uses a `try...catch` block to wrap the crucial parts of the request handling logic and properly logs any errors that occur.