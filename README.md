# Exercise Tracker REST API

#### A microservice project, part of Free Code Camp's curriculum

[See this project on FreeCodeCamp](https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/exercise-tracker)

### User Stories based on requirements from FreeCodeCamp

POST 
 
2. I can create a user by posting form data username to /api/exercise/new-user and returned will be an object with username and _id.

3. I can add an exercise to any user by posting form data userId(_id), description, duration, and optionally date to /api/exercise/add. If no date supplied it will use current date. Returned will be the user object with also with the exercise fields added.


GET 

3. I can get an array of all users by getting `api/exercise/users` with the same info as when creating a user.
   
4. I can retrieve a full exercise log of any user by getting `/api/exercise/log` with a parameter of userId(_id). Return will be the user object with added array log and count (total exercise count).
5. I can retrieve part of the log of any user by also passing along optional parameters of from & to or limit. (Date format yyyy-mm-dd, limit = int)


### User Stories of this application 


POST 
 
1. I can see if an user is register with username by posting form data with username 

2. I can create a user by posting form data username to /api/exercise/new-user and returned will be an object with username and username.

3. I can add an exercise to any user by posting form data username(not _id), description, duration, and optionally date to /api/exercise/add. If no date supplied it will use current date. Returned will be the user object with also with the exercise fields added.


GET 

3. I can get an array of all users by getting `api/exercise/users` with the same info as when creating a user.
   
4. I can retrieve a full exercise log of any user by getting `/api/exercise/log` with a parameter of username(not _id). Return will be the user object with added array log and count (total exercise count).

5. I can retrieve part of the log of any user by also passing along optional parameters of from & to or limit. (Date format yyyy-mm-dd, limit = int)
