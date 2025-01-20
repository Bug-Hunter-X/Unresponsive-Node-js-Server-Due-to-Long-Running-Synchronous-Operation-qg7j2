# Unresponsive Node.js Server

This repository demonstrates a common issue in Node.js applications: an unresponsive server caused by a long-running synchronous operation blocking the event loop.

The `bug.js` file contains a Node.js server that simulates a long-running task within the request handler. This blocks the event loop, preventing the server from responding to further requests.

The `bugSolution.js` file provides a solution using asynchronous operations to prevent the event loop from being blocked.  This allows the server to remain responsive even during long-running tasks.