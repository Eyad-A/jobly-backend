# Jobly Backend
This is the backend for the "Jobly" project. Jobly is an app that allows users 
to search for and apply to different companies. The backend is built with Node, 
Express, and Postgresql. 

You can find the frontend here. 

## Features 
- This is a pure API app, taking values from the query string (GET requests) or 
from a JSON body, and returns JSON
- Uses JWT tokens for authentication/authorization 
- Ability to GET companies and filter by name, minimum/maximum number of employees
- Ability to GET jobs and filter by title, salary, and equity (boolean)
- Authorization: only users with isAdmin flag are able to create, update, or delete companies
- Getting information on a user, updating, or deleting a user should only be permitted either by an admin, or by that user.
- Allow users to apply for jobs by sending POST request to
/users/:username/jobs/:id 