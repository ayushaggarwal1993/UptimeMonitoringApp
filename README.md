# UptimeMonitoringApp
Allows users to enter URL they want to be monitored and receive alerts when they "go down" or "come back up"


API listens on a PORT and accepts incoming HTTP requests for GET,POST,PUT,DELETE and HEAD.
API allows a client to connect, create a new user then edit or delete it.
API allows a user to "sign in" which gives them a token theat they can use for subsequent authenticated requests.
API allows the user to "sign out" which invalidates their token
API allows a "signed in" user to create a new "check" using their token, edit the check or delete the check.
API restricts a user to create at max 5 checks
In the background, workers perform all the "checks" at appropriate time, and send alerts to the user when the url changes state.

