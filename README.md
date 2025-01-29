# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  The `bug.js` file shows a route handler that attempts to parse a user ID from a request parameter.  If the ID is not a valid number, the code will throw an error, resulting in an unexpected 500 error.

The `bugSolution.js` file provides a corrected version with proper error handling, ensuring more robust and predictable behavior.

## How to reproduce

1. Clone the repository.
2. Run `npm install` to install Express.js.
3. Run `node bug.js`.  Make a request to `/users/abc` (invalid ID) and observe the error.
4. Run `node bugSolution.js`. Make the same request and observe the improved error handling.