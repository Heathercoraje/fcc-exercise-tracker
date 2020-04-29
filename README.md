# Exercise Tracker REST API

This is based on one of microservice projects of Free Code Camp's server side curriculum. [See this project on FreeCodeCamp](https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/exercise-tracker). Compared to original requirements of user story, this application has a few added endpoints and UI for improving user experience of basic use of application. To read step-by-step article on how to write this project from scratch, click [here](https://url-to-article). 

---


### User Stories
 
- View and create an user 
  - I can get an array of all users by getting `api/exercise/users` with the same info as when creating a user.
   
  - I can see if an user is registered with username by posting form data with username to `api/users/user`. If user exist, it returns user data.
  - I can create a user by posting form data username to `/api/exercise/new-user` and returned will be an object with username and status of registering.

- Add exercise
  - I can add an exercise to any user by posting form data username(not _id), description, duration, and optionally date to `/api/exercise/add`. If no date supplied it will use current date. Returned will be the user object of username and exercises also with new exercise item added.

- Retrieve exercise log
  - I can retrieve a full exercise log of any user by getting `/api/exercise/log` with a parameter of username(not _id). Return will be the user object with added array log and count (total exercise count).
  - I can retrieve part of the log of any user by also passing along optional parameters of from & to or limit. (Date format yyyy-mm-dd, limit = int) If date parameters are not passed, From default to `new date(0)`, To defaults to `new date()` and limit defaults to 100 items
