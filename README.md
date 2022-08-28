# Uptime Monitoring Node Application
This is a plane Node.js App which allows users to enter URLs they want monitored, & receive alerts when those resources "go down" or "come back".

## Features
 - SignIn
 - SignUp
 - SignOut
 - Edit there settings in addition to make uptime checks
 - Show users' their UpTime alerts(Up alerts & Down alerts of their URLs) via SMS.

 ## Follwoing are the Backend specs of the Uptime Monitoring Node Application
 1. The API listens on a PORT & accepts incoming HTTP requests for POST, GET, PUT, Delete & HEAD.
 2. The API allows a client to connect to the server, so that they can create a new user, edit that user or delete that user.
 3. The API allows a user to "sign in" which gives them a token so that they can use for subsequent authenticated requests.
 4. The API allows the user to "sign out" which invalidates their token.
 5. The API allows a signed-in user to use their token to create a new "check". Here check means a task a system to check a given URL to see of its up or down.
 6. The API allows a signed-in user to edit or delete any of their checks.
 7. In the background, workers perform all the "checks" at the appropriate times & send alerts to the users when a check changes its state from "up" to "down", or vice-versa.
