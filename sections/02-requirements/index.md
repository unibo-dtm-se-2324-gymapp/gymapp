---
title: Requirements
has_children: false
nav_order: 3
---

# Requirements

<h3>Goals</h3>
The goal of Six-pack is to provide an easy-to-use app where users can manage autonomously their training routine by deciding which exercises to do according to their needs.

<h3>User stories</h3>
<p>
    <ul>
        <li>As a potential fitness enthusiast, I want create my account and subscribe to the app; so that I can start to plan my training session and personalize the exercises, so that i can have a routine that suits my fitness goals. </li>
        <li>As a fitness beginner, I want to view video or image demonstrations for each exercise as instructions, so that I can perform them safely and effectively.</li>
        <li>As a busy worker, I want to save and load my workout sessions quickly, so that I can fit my training into my daily working schedule.</li>
        <li>As an experienced athlete, I want to customize the sets, reps, and rest times, so that my workouts are aligned with my training level.</li>
        <li>As a user, I want to log in and save my training data, so that I can access my workouts across multiple devices.
</li>
        <li>As a user, i want to save as many training sessions as possible, decide the number of series of the same exercises, how many reps so that i can get fit in a proper way.  </li></ul>
</p>

<h3>Functional Requirements</h3>
<h5>User Authentication</h5>
Requirement: Users must be able to create a profile and log in to the application.
<h7>Acceptance Criteria:</h7>
<ul>
    <li>Users can create an account using an email and password.</li>
    <li>After creating an account, users can use their email and password to log in and access to our app functionalities.</li>
    <li>On successful login, users are directed to the home page where they can start creating their training plans.</li>
</ul>

<h5>Creation of a training session</h5>
Requirement: Users must be able to create a personalized training session and insert as many exercises as they want by simply pushing a few buttons.
<h7>Acceptance Criteria:</h7>
<ul>
    <li>Users can start a new session by clicking on “New Training Session.”</li>
    <li>A page shows up, allowing users to add exercises, select the number of reps, sets, and rest intervals.</li>
    <li>Once saved, the session appears on the user’s main dashboard.</li>
</ul>

<h5>Exercise customization</h5>
Requirement:  Users must be able to set the number of reps, sets, and rest periods for each exercise.

<h7>Acceptance Criteria:</h7>

<ul>
    <li>In the exercise setup, users can specify the number of reps and sets for each exercise</li>
    <li>A field for setting the rest period between sets is recommended for a better training experience.</li>
    <li>The exercise is saved with all customization details visible in the session summary.</li>
</ul>

<h5>Multimedia Integration</h5>
Requirement:Users must be able to add image or video links to exercises for instructional purposes.

<h7>Acceptance Criteria:</h7>

<ul>
    <li>Users can insert a link to a video or image as part of each exercise.</li>
    <li>The app displays these visuals next to the exercise in the training session view.</li>
    <li>When clicked, the media opens in an external player or browser. Internet connection is needed</li>
</ul>

<h5>Session Management</h5>
Users can save, edit, or delete their training sessions.

<h7>Acceptance Criteria:</h7>

<ul>
    <li>Users can view saved sessions on their dashboard.</li>
    <li>Each session can be edited by selecting an “Edit” option, allowing modifications to exercises, reps, sets, and rest periods.</li>
    <li>Users can delete a session by selecting “Delete,” and a confirmation message appears.</li>
</ul>

<h3>Non-functional requirements</h3>

<h5>Usability</h5>
Requirement: The application must be easy to navigate, allowing users to complete tasks with minimal clicks. Users can complete common tasks in a short time span.
<h7>Acceptance Criteria:</h7>

<ul>
    <li>Any function (adding exercises, editing, deleting) must be accessible within 3 clicks.</li>
    <li>All buttons and icons are clearly labeled with intuitive visuals.</li>
</ul>

<h5> Performance</h5>
Requirement: The app should load each screen and execute actions (saving, editing, deleting sessions) with minimal delay.
<h7>Acceptance Criteria:</h7>

<ul>
    <li>Each page or action must load and execute within 2 seconds on standard network conditions.</li>
    <li>Video and image previews load without delays (within 1 second).</li>
</ul>
<h5> Security</h5>
Requirement: User data must be securely stored and protected, with data transfers encrypted.
<h7>Acceptance Criteria:</h7>

<ul>
    <li>User passwords and sensitive data are encrypted before storage.</li>
    <li>The app uses HTTPS for all data transmission to secure user interactions.</li>
    <li>Access to the app requires login after inactivity or logout, protecting user information.</li>

</ul>
<h5> Device Compatibility</h5>
Requirement: The application should be able to run on recent IOS and Android devices. 
<h7>Acceptance Criteria:</h7>

<ul>
    <li>The app works well perfectly on devices running iOS 13.0+ and Android 9.0+.</li>
    <li>The app uses HTTPS for all data transmission to secure user interactions.</li>
    <li>Access to the app requires login after inactivity or logout, protecting user information.</li>

</ul>

<h5> Data synchronization</h5>
Requirement: Data should sync seamlessly across devices for users logged into the same account.
<h7>Acceptance Criteria:</h7>

<ul>
    <li>When a user makes changes, updates to the training plan on the device, the data syncs to other devices within a few seconds of the change. </li>
    <li>The syn occurs in the background without effecting the overal performance of the application. </li>
</ul>

<h5>Customization</h5>
Requirement: The application is thought for being as much adaptable as possible to the users' desires and needs with neither limits concerning the number of exercises they can do during a session nor concerning the reps or the series.

<h3>Implementation requirements</h3>
<h5>1.Programming Language & Frameworks</h5>
REQUIREMENTS: The application should be developed using a modern framework compatible with mobile and desktop environments.
<h7>Acceptance Criteria:</h7>

<ul>
    <li>Frontend is implemented using HTML, CSS, and JavaScript for flexibility and responsiveness. </li>
    <li>Backend services are developed using Python with the Flask framework. </li>
</ul>

<h5>2.Database Management</h5>
REQUIREMENTS: User and training session data must be stored in our own database system so we can have an easier data management. 
<h7>Acceptance Criteria:</h7>

<ul>
    <li>The database must be SQL-based  </li>
    <li>The data model should include user accounts, training sessions, exercises, and multimedia links. </li>
</ul>
