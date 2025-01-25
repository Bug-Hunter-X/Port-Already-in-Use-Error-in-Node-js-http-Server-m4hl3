# Node.js Port Already in Use Error

This repository demonstrates a common error encountered when developing Node.js applications: the `EADDRINUSE` error, which occurs when your server attempts to bind to a port that is already in use by another process.

The `bug.js` file contains the problematic code, and `bugSolution.js` provides a robust solution.

## Problem

The provided Node.js HTTP server attempts to bind to port 8080. If another application (like another Node.js server or a browser-based application) is already using this port, the server will fail to start and might throw an error that isn't always helpful in pinpointing the exact issue. 

## Solution

The `bugSolution.js` file presents a refined version of the server. It incorporates error handling to gracefully manage the `EADDRINUSE` error, allowing for retries or alternative actions.