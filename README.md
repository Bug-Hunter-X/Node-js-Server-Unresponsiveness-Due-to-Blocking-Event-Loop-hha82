# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js applications: blocking the event loop, leading to server unresponsiveness.

## Problem

The `server.js` file contains a simple HTTP server that simulates a long-running task within the request handler. This task blocks the event loop, preventing the server from processing other requests for 5 seconds.

## Solution

The `serverSolution.js` file provides a solution using asynchronous operations to prevent blocking the event loop.  The solution showcases the use of `setTimeout` to handle long-running tasks without blocking.

## How to Run

1. Clone the repository.
2. Navigate to the repository's directory.
3. Run `node server.js` to see the unresponsive server behavior.
4. Run `node serverSolution.js` to observe the improved responsiveness.