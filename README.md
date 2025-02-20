# Missing Error Handling in Express.js Route Handler

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

## Bug

The `bug.js` file contains an Express.js route that fetches a user by ID.  However, it lacks error handling for cases where the provided ID is invalid or does not correspond to an existing user. This omission can lead to unexpected behavior or even crashes.

## Solution

The `bugSolution.js` file demonstrates the corrected code.  It includes error handling to gracefully manage cases where the user is not found, returning a 404 status code instead of crashing.