---
title: Developer guide
has_children: false
nav_order: 11
---

# Developer Guide
- This section explains how to use the software (from a developer perspective)
    - For example, how to use the software API to build more software

# Developer Guide: Six-Pack Application API

API Endpoint Explanations
The "Six-Pack" application helps users organize their workout routines by allowing them to add, modify, and track their exercise sessions. The API provides functionality to manage workout sessions, user accounts, and other application features.

# Authentication Routes
POST /register
Description: Create a user account and save their credentials.
Parameters:
username (str): The user's chosen username.
password (str): The user's chosen password.
email (str): The user's email address.
Response: JSON message indicating success or failure.

POST /login
Description: Authenticate a user and return a session token.
Parameters:
username (str): The user's username.
password (str): The user's password.
Response: JSON message containing the session token.

# Workout Session Routes

POST /workout_sessions/
Description: Create a new workout session.
Parameters:
session_id (str): The unique ID of the workout session.
date (str): The date of the session.
title (str): The title of the workout session.
description (str): Detailed description of the workout session.
Response: JSON message indicating success.

PUT /workout_sessions/{session_id}/
Description: Update an existing workout session.
Parameters:
session_id (str): The unique ID of the workout session to be updated.
title (str, optional): Updated title of the session.
description (str, optional): Updated description of the session.
date (str, optional): Updated date for the session.
Response: JSON message indicating success.

DELETE /workout_sessions/{session_id}/
Description: Delete an existing workout session.
Parameters:
session_id (str): The ID of the workout session to be deleted.
Response: JSON message indicating success.

# Exercise Routes

POST /workout_sessions/{session_id}/exercises/
Description: Add an exercise to a workout session.
Parameters:
session_id (str): The ID of the workout session.
exercise_name (str): Name of the exercise.
reps (int): Number of repetitions for the exercise.
sets (int): Number of sets for the exercise.
weight (float, optional): Weight used for the exercise, if applicable.
Response: JSON message indicating success.

PUT /workout_sessions/{session_id}/exercises/{exercise_id}/
Description: Modify an existing exercise in a workout session.
Parameters:
session_id (str): The ID of the workout session.
exercise_id (str): The ID of the exercise to be modified.
exercise_name (str, optional): Updated name of the exercise.
reps (int, optional): Updated number of repetitions.
sets (int, optional): Updated number of sets.
weight (float, optional): Updated weight used for the exercise.
Response: JSON message indicating success.

DELETE /workout_sessions/{session_id}/exercises/{exercise_id}/
Description: Delete an exercise from a workout session.
Parameters:
session_id (str): The ID of the workout session.
exercise_id (str): The ID of the exercise to be deleted.
Response: JSON message indicating success.

# Account Management Routes

POST /accounts/
Description: Create a new user account.
Parameters:
email (str): The email of the user.
username (str): The username of the user.
password (str): The user's password.
Response: JSON message indicating success.

PUT /accounts/{email}/
Description: Update an existing user account.
Parameters:
email (str): The user's email.
username (str, optional): Updated username.
password (str, optional): Updated password.
Response: JSON message indicating success.

DELETE /accounts/{email}/
Description: Delete a user account.
Parameters:
email (str): The email of the account to be deleted.
Response: JSON message indicating success.

# Timer and Media (Optional Features)

If implemented, the following routes will be used for timer management and exercise media upload.

Timer Routes (Optional)

POST /workout_sessions/{session_id}/timer/: Start a timer for a session.
PUT /workout_sessions/{session_id}/timer/: Update or stop the session timer.
GET /workout_sessions/{session_id}/timer/: Get the current status of the session timer.
Media Routes (Optional)
POST /workout_sessions/{session_id}/exercises/{exercise_id}/media/: Upload a video or image for an exercise.
DELETE /workout_sessions/{session_id}/exercises/{exercise_id}/media/: Delete a video or image associated with an exercise.

This API structure ensures flexibility for managing user accounts, workout sessions, exercises, and optional features like media and timers, aligning with the goals of the "Six-Pack" application.

Here is a detailed description of the APIs and routes defined in the this code. 
Each endpoint, its purpose, the HTTP methods supported, and how to interact with them are described in the following text.


Home Page  (/)
Route: /
Methods: GET
Description:
It redirects to the login page (/loginpage), if a user is not logged in. Otherwise, it redirects it to the home page (/homepage) on logging into the account.
Behavior: The program examines for the cookie (user_id). If one is present and fits into the user_data, a user is directed to the homepage. Otherwise, to the login page.

Login Page (/loginpage)
Route: /loginpage
Methods: GET, POST
Description:
Operates with the login form (GET request) and accuracy of the supplied login information (POST request).
When user views a form (POST request), the system evaluates the credentials in the database. If found correct, then user is cookie noted as online as “user_id” and directed to their homepage. If the user is not yet a member of the system or provided the wrong access passwords for the system, and error will emerge.
Form Parameters (POST):
email: please put the retrieved email into this our form for the user.
password: The retrieved password will go into the password field of the user form.

3. Register Page (/register)
Route: /register
Methods: GET, POST
Description:
Shows the registration form (GET request) and processes the registration operation taken by the user (As in the POST method).
After that, the application checks if the passwords match and if the email is already in use when the form is posted. If all is well, the user_information table is updated with the new user and redirects user to the home page and also set a cookie for the user_id.
Form Parameters (POST):
username: please put the appropriate name in this perimeter of the user.
email: please put the email address of the user in the email field.
password: the password of the new user on this form should be entered here.
confirm-password: an exact copy of the password to enable confirmation is entered here.

4. Home Page (Logged In) (/homepage)
Route: /homepage
Methods: GET
Description:
Shows that a user is logged in and displays the user's home page for this situation. Otherwise, to the login page.

5. Profile Page (/profile)
Route: /profile
Methods: GET
Description:
Shows the details of the user profile. If the user tried to access his/her profile but he/she was not logged-in, redirected to the login page.

6. Logout (/logout)
Route: /logout
Methods: GET
Description:
Logs the user out by removing the user_id cookie and redirects him to 