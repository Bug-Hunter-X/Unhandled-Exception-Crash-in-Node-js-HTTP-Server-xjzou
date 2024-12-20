# Unhandled Exception Crash in Node.js HTTP Server

This repository demonstrates a common error in Node.js where an unhandled exception can crash a server without providing useful error messages.  The `bug.js` file contains the problematic code, while `bugSolution.js` shows how to fix it by implementing proper error handling.

## Problem

The `bug.js` server lacks error handling.  If any unexpected exception occurs during request processing, the server will abruptly crash. This results in downtime and a lack of information about what went wrong.  Debugging such issues can be incredibly difficult.

## Solution

The `bugSolution.js` file demonstrates how to use `try...catch` blocks to gracefully handle exceptions.  This prevents server crashes and allows for logging errors or sending informative error responses to the client.