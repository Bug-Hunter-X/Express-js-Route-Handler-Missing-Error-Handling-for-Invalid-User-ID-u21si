# Express.js Route Handler Missing Error Handling

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when dealing with user inputs.  The `bug.js` file shows a route that attempts to access a user by ID.  If the ID provided is not a valid integer, the application will crash.

The solution is provided in `bugSolution.js`.  It handles the potential `NaN` (Not a Number) error and returns a proper 400 Bad Request response in case of invalid input.