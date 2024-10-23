---
title: Design
has_children: false
nav_order: 4
---

<h1> Design </h1>

## Architecture 
<h5>Front-End:</h5>
<h6>HTML, CSS, and JavaScript:</h6>
<p> The front-end aspect of the Sixpack application leverages basic web technologies. HTML structures the content of each page, while CSS styles the interface with a clean design, ensuring a responsive layout for different screen sizes. JavaScript handles user interactions, such as dynamically loading and modifying training sessions, validating forms, and responding to events triggered by users.</p>

<h5>Back-End</h5>
<h6> Flask:</h6>
<p>Given its modularity and simplicity, it has been decided to use Flask as a back-end tool that guarantees the possibility to add new  functions and to perform actions by using a given interface. Flask routes are used to manage different endpoints, handle login and registration processes, and facilitate interactions between the client and server.</p>

<h5>Data Management</h5>
<h6>Local Storage and Server Communication:</h6>
<p>The project incorporates JavaScript's local storage for temporarily saving user data and loading it when is requested. Additionally, server communication is handled via fetch API calls that interact with the Flask back-end, allowing data persistence and updates to be saved on the server.</p>


## Modelling
<h5>Domain modelling:</h5>
<p>The domain model of "Six-pack" will be based on the Unified Modelling Language (UML) principles, so to ensure connections between the core business logic and the software development logic.
<h6>Class diagram:</h6>
<b>User:</b> <p> This class represents the person who wants to start using Six-pack. A user has a name, an e-mail and a password. User details are stored in the memory to authenticate and manage user-specific training sessions.
</p>
<br>
<b>Exercise:</b> <p> This class stands for a physical activity that a user wants to do during a training session. It can be repeated multiple times both consequently or after a short break.
An exercise has a name, number of reps, number of series, time break, a body part that is supposed to train and eventually a link to a video or an image if the user wants to add it
</p>
<b>Training session:</b> <p> Consists of a collection of exercises grouped under a session title. Each training session is linked to a user, allowing them to customize and manage their personal workout routines. The training session is divided by days of the week. The user can create a workout routine for each day of the week.
</p>



## Interaction
<h5>Create a new trainig session</h5>
After the registration and the login, the users will find themselves in the homepage of the app.
Here they have the possibility to manage existing workouts or create a new one
<h5>Add an exercise</h5>
<p>User: Once that the users have created or retrieved a past training session, they can modify the exercises or add a new exercises by clicking the "+" button and a ready-to-use grid will appear.
The spaces of the grid need to be filled out with the name of the exercise, the number of reps, the number of series, the time break and a link to whatever the users want (images or videos).
</p>

## Behaviour
<h3>Flowchart diagram</h3>
<b>Start:</b> After the first login, the app is empty, with no training sessions at all.<br>
<b>Training session creation:</b> The user decide to create his/her first training session.<br>
<b>Modification of a training sessions:</b> The user can modify the training session by inserting or removing one or more exercises <br>
<b>Modification of an exercise:</b> The user can modify also just an exercise by entering in a training session and perform changes on the various section of the exercise grid. <br>

## Data-related aspects

<b>User table:</b>Containing all the users'data <br>
<b>Training session table:</b>Containing all the training sessions created by a single user<br>
<b>Exercise table:</b> Containing all the exercises inserted in the various training session by the user.<br>
<b>Data Persistence:</b>Data is temporarily stored in the client’s local storage for seamless transitions between pages and is persisted to the server database using JavaScript’s fetch API with POST requests.<br>

