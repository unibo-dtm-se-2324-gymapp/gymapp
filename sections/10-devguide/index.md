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
