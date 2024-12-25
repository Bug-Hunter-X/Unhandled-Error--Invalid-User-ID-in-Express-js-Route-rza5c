# Express.js Route Error Handling Bug

This repository demonstrates a common error in Express.js route handlers:  lack of proper error handling for invalid input.  The `bug.js` file shows the faulty code, while `bugSolution.js` provides the corrected version.

**Bug:** The route handler `/users/:id` does not handle cases where the `id` parameter is not a valid integer. This can lead to runtime errors or unexpected responses.

**Solution:** The corrected code includes error handling to check if the `id` is a valid integer and returns a 404 status code if no user is found, providing a better user experience and preventing application crashes.