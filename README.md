# Intermittent Node.js Server Crash

This repository demonstrates a bug causing intermittent crashes in a simple Node.js HTTP server. The server runs without throwing any errors, making debugging challenging.

## Bug Description

A Node.js server, built using the `http` module, occasionally crashes without any apparent reason. No error messages are logged to the console.

## How to Reproduce

1. Clone the repository.
2. Run `node bug.js`.
3. Send several requests to the server (e.g., using `curl`).
4. Observe that after some time, the server might crash without any error messages.

## Solution

The solution involves adding appropriate error handling to gracefully handle exceptions.