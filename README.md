# Node.js Server Crashing Under Load

This repository demonstrates a common issue in Node.js applications where the server crashes under a heavy load.  The problem is related to unhandled exceptions or memory leaks, often subtle and difficult to diagnose.

## Bug

The `server.js` file contains a simple HTTP server. While it functions correctly under light load, it crashes without error messages when subjected to a high volume of concurrent requests.  The exact cause is a lack of error handling and proper resource management.

## Solution

The `server-fixed.js` demonstrates how to address the stability issue. It includes comprehensive error handling using `try...catch` blocks and proper resource cleanup.